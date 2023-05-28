# Comparing `tmp/tuack-0.1.5.1.1.tar.gz` & `tmp/tuack-0.1.5.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tuack-0.1.5.1.1.tar", last modified: Thu May 18 04:25:50 2023, max compression
+gzip compressed data, was "tuack-0.1.5.1.2.tar", last modified: Sun May 28 15:37:45 2023, max compression
```

## Comparing `tuack-0.1.5.1.1.tar` & `tuack-0.1.5.1.2.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:50.007295 tuack-0.1.5.1.1/
--rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/LICENSE
--rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/MANIFEST.in
--rw-rw-rw-   0        0        0      522 2023-05-18 04:25:50.006298 tuack-0.1.5.1.1/PKG-INFO
--rw-rw-rw-   0        0        0     1717 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/README.md
--rw-rw-rw-   0        0        0       42 2023-05-18 04:25:50.007295 tuack-0.1.5.1.1/setup.cfg
--rw-rw-rw-   0        0        0     1930 2023-05-18 04:25:25.000000 tuack-0.1.5.1.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.639522 tuack-0.1.5.1.1/tuack/
--rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/__init__.py
--rw-rw-rw-   0        0        0    34993 2023-05-18 04:24:36.000000 tuack-0.1.5.1.1/tuack/base.py
--rw-rw-rw-   0        0        0    13348 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/doc.py
--rw-rw-rw-   0        0        0    27596 2023-05-16 13:23:14.000000 tuack-0.1.5.1.1/tuack/dump.py
--rw-rw-rw-   0        0        0    14486 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/gen.py
--rw-rw-rw-   0        0        0     2334 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/install.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.770818 tuack-0.1.5.1.1/tuack/lex/
--rw-rw-rw-   0        0        0        0 2018-09-07 13:38:42.000000 tuack-0.1.5.1.1/tuack/lex/compile.log
--rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/compile.pyinc
--rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/format-linux
--rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/format-mac
--rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/format-win.exe
--rw-rw-rw-   0        0        0      320 2018-08-27 16:45:44.000000 tuack-0.1.5.1.1/tuack/lex/hehe.log
--rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/lex.l
--rw-rw-rw-   0        0        0    94066 2018-09-07 13:38:44.000000 tuack-0.1.5.1.1/tuack/lex/lex.yy.c
--rw-rw-rw-   0        0        0    36942 2018-06-11 12:35:42.000000 tuack-0.1.5.1.1/tuack/lex/lex.yy.o
--rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/main.h
--rw-rw-rw-   0        0        0    42594 2018-09-07 13:38:44.000000 tuack-0.1.5.1.1/tuack/lex/yacc.tab.c
--rw-rw-rw-   0        0        0     1906 2018-09-07 13:38:44.000000 tuack-0.1.5.1.1/tuack/lex/yacc.tab.h
--rw-rw-rw-   0        0        0     9007 2018-06-11 12:35:42.000000 tuack-0.1.5.1.1/tuack/lex/yacc.tab.o
--rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/lex/yacc.y
--rw-rw-rw-   0        0        0    12225 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/load.py
--rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/num2chinese.py
--rw-rw-rw-   0        0        0    13010 2023-05-16 13:23:14.000000 tuack-0.1.5.1.1/tuack/packer.py
--rw-rw-rw-   0        0        0    24468 2023-05-13 04:24:01.000000 tuack-0.1.5.1.1/tuack/ren.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.836571 tuack-0.1.5.1.1/tuack/sample/
--rw-rw-rw-   0        0        0     7909 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/arbiter_e.noi_linux1.sample
--rw-rw-rw-   0        0        0    23576 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/arbiter_e.sample
--rw-rw-rw-   0        0        0     5586 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/chk.cpp
--rw-rw-rw-   0        0        0      195 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/contest.gitignore
--rw-rw-rw-   0        0        0      266 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/contest.json
--rw-rw-rw-   0        0        0      186 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/day.gitignore
--rw-rw-rw-   0        0        0      207 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/day.json
--rw-rw-rw-   0        0        0      351 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/empty.gitattributes
--rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/empty.gitignore
--rw-rw-rw-   0        0        0      435 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/empty.json
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.891887 tuack-0.1.5.1.1/tuack/sample/precautions/
--rw-rw-rw-   0        0        0       60 2022-08-12 11:20:32.000000 tuack-0.1.5.1.1/tuack/sample/precautions/zh-cn.md
--rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/sample/problem.gitattributes
--rw-rw-rw-   0        0        0      254 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/problem.gitignore
--rw-rw-rw-   0        0        0      466 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample/problem.json
--rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/sample/uoj.json
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.571838 tuack-0.1.5.1.1/tuack/sample-empty/
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.836571 tuack-0.1.5.1.1/tuack/sample-empty/statement/
--rw-rw-rw-   0        0        0      411 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-empty/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.571838 tuack-0.1.5.1.1/tuack/sample-problem/
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.846552 tuack-0.1.5.1.1/tuack/sample-problem/data/
--rw-rw-rw-   0        0        0       44 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/data/1.ans
--rw-rw-rw-   0        0        0       43 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/data/1.in
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.856917 tuack-0.1.5.1.1/tuack/sample-problem/down/
--rw-rw-rw-   0        0        0       79 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/down/1.ans
--rw-rw-rw-   0        0        0       77 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/down/1.in
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.866375 tuack-0.1.5.1.1/tuack/sample-problem/pre/
--rw-rw-rw-   0        0        0       80 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/pre/1.ans
--rw-rw-rw-   0        0        0       78 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/pre/1.in
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.873787 tuack-0.1.5.1.1/tuack/sample-problem/resources/
--rw-rw-rw-   0        0        0  3293583 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/resources/sample.png
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.876780 tuack-0.1.5.1.1/tuack/sample-problem/solution/
--rw-rw-rw-   0        0        0     1968 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/solution/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.877777 tuack-0.1.5.1.1/tuack/sample-problem/statement/
--rw-rw-rw-   0        0        0     6819 2023-05-13 04:24:01.000000 tuack-0.1.5.1.1/tuack/sample-problem/statement/zh-cn.md
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.890900 tuack-0.1.5.1.1/tuack/sample-problem/tables/
--rw-rw-rw-   0        0        0     1062 2023-03-28 10:24:11.000000 tuack-0.1.5.1.1/tuack/sample-problem/tables/data.pyinc
--rw-rw-rw-   0        0        0     1227 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/tables/json_data.json
--rw-rw-rw-   0        0        0      205 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/sample-problem/tables/table.json
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.982673 tuack-0.1.5.1.1/tuack/templates/
--rw-rw-rw-   0        0        0      911 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/ccc.tex.jinja
--rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/templates/ccpc.png
--rw-rw-rw-   0        0        0     1240 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/ccpc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.571838 tuack-0.1.5.1.1/tuack/templates/en/
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.993341 tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/
--rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/font.html.jinja
--rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/font.tex.jinja
--rw-rw-rw-   0        0        0      670 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/hand.tex.jinja
--rw-rw-rw-   0        0        0      144 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/image.html.jinja
--rw-rw-rw-   0        0        0      530 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/image.tex.jinja
--rw-rw-rw-   0        0        0     5116 2023-05-13 04:24:01.000000 tuack-0.1.5.1.1/tuack/templates/problem_base.md.jinja
--rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/table.html.jinja
--rw-rw-rw-   0        0        0      402 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/table.md.jinja
--rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5.1.1/tuack/templates/table.tex.jinja
--rw-rw-rw-   0        0        0     2125 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/template_base.tex.jinja
--rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5.1.1/tuack/templates/template_base.tex.jinja.tex
--rw-rw-rw-   0        0        0     4756 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/tuack.cls
--rw-rw-rw-   0        0        0     8743 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/tuoi.tex.jinja
--rw-rw-rw-   0        0        0     1443 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/tupc.tex.jinja
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.571838 tuack-0.1.5.1.1/tuack/templates/zh-cn/
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:50.004314 tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/
--rw-rw-rw-   0        0        0     3139 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
--rw-rw-rw-   0        0        0     3543 2023-01-09 01:26:59.000000 tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po
--rw-rw-rw-   0        0        0    17497 2023-05-18 04:24:36.000000 tuack-0.1.5.1.1/tuack/test.py
--rw-rw-rw-   0        0        0     3777 2023-02-22 09:36:20.000000 tuack-0.1.5.1.1/tuack/tools.py
-drwxrwxrwx   0        0        0        0 2023-05-18 04:25:49.645500 tuack-0.1.5.1.1/tuack.egg-info/
--rw-rw-rw-   0        0        0      522 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     2261 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       77 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-05-18 04:25:49.000000 tuack-0.1.5.1.1/tuack.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.843270 tuack-0.1.5.1.2/
+-rw-rw-rw-   0        0        0    35055 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/LICENSE
+-rw-rw-rw-   0        0        0       17 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/MANIFEST.in
+-rw-rw-rw-   0        0        0      522 2023-05-28 15:37:45.841838 tuack-0.1.5.1.2/PKG-INFO
+-rw-rw-rw-   0        0        0     1717 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/README.md
+-rw-rw-rw-   0        0        0       42 2023-05-28 15:37:45.843270 tuack-0.1.5.1.2/setup.cfg
+-rw-rw-rw-   0        0        0     1930 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.771806 tuack-0.1.5.1.2/tuack/
+-rw-rw-rw-   0        0        0      116 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/__init__.py
+-rw-rw-rw-   0        0        0    34950 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/tuack/base.py
+-rw-rw-rw-   0        0        0    13348 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/doc.py
+-rw-rw-rw-   0        0        0    27596 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/dump.py
+-rw-rw-rw-   0        0        0    14486 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/gen.py
+-rw-rw-rw-   0        0        0     2334 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/install.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.801724 tuack-0.1.5.1.2/tuack/lex/
+-rw-rw-rw-   0        0        0        0 2018-09-07 13:38:42.000000 tuack-0.1.5.1.2/tuack/lex/compile.log
+-rw-rw-rw-   0        0        0      971 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/compile.pyinc
+-rw-rw-rw-   0        0        0  2295192 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/format-linux
+-rw-rw-rw-   0        0        0    61896 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/format-mac
+-rwxrwxrwx   0        0        0  2178321 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/format-win.exe
+-rw-rw-rw-   0        0        0      320 2018-08-27 16:45:44.000000 tuack-0.1.5.1.2/tuack/lex/hehe.log
+-rw-rw-rw-   0        0        0    11191 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/lex.l
+-rw-rw-rw-   0        0        0    94066 2018-09-07 13:38:44.000000 tuack-0.1.5.1.2/tuack/lex/lex.yy.c
+-rw-rw-rw-   0        0        0    36942 2018-06-11 12:35:42.000000 tuack-0.1.5.1.2/tuack/lex/lex.yy.o
+-rw-rw-rw-   0        0        0      185 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/main.h
+-rw-rw-rw-   0        0        0    42594 2018-09-07 13:38:44.000000 tuack-0.1.5.1.2/tuack/lex/yacc.tab.c
+-rw-rw-rw-   0        0        0     1906 2018-09-07 13:38:44.000000 tuack-0.1.5.1.2/tuack/lex/yacc.tab.h
+-rw-rw-rw-   0        0        0     9007 2018-06-11 12:35:42.000000 tuack-0.1.5.1.2/tuack/lex/yacc.tab.o
+-rw-rw-rw-   0        0        0      388 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/lex/yacc.y
+-rw-rw-rw-   0        0        0    12217 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/tuack/load.py
+-rw-rw-rw-   0        0        0     3605 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/num2chinese.py
+-rw-rw-rw-   0        0        0    13010 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/packer.py
+-rw-rw-rw-   0        0        0    24499 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/tuack/ren.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.812000 tuack-0.1.5.1.2/tuack/sample/
+-rw-rw-rw-   0        0        0     7909 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/arbiter_e.noi_linux1.sample
+-rw-rw-rw-   0        0        0    23576 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/arbiter_e.sample
+-rw-rw-rw-   0        0        0     5586 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/chk.cpp
+-rw-rw-rw-   0        0        0      195 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/contest.gitignore
+-rw-rw-rw-   0        0        0      266 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/contest.json
+-rw-rw-rw-   0        0        0      186 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/day.gitignore
+-rw-rw-rw-   0        0        0      207 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/day.json
+-rw-rw-rw-   0        0        0      351 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/empty.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/empty.gitignore
+-rw-rw-rw-   0        0        0      435 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/empty.json
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.827125 tuack-0.1.5.1.2/tuack/sample/precautions/
+-rw-rw-rw-   0        0        0       60 2023-05-18 04:27:16.000000 tuack-0.1.5.1.2/tuack/sample/precautions/zh-cn.md
+-rw-rw-rw-   0        0        0      342 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/sample/problem.gitattributes
+-rw-rw-rw-   0        0        0      254 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/problem.gitignore
+-rw-rw-rw-   0        0        0      466 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample/problem.json
+-rw-rw-rw-   0        0        0       76 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/sample/uoj.json
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.704238 tuack-0.1.5.1.2/tuack/sample-empty/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.812996 tuack-0.1.5.1.2/tuack/sample-empty/statement/
+-rw-rw-rw-   0        0        0      411 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-empty/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.748398 tuack-0.1.5.1.2/tuack/sample-problem/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.814487 tuack-0.1.5.1.2/tuack/sample-problem/data/
+-rw-rw-rw-   0        0        0       44 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/data/1.ans
+-rw-rw-rw-   0        0        0       43 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/data/1.in
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.815846 tuack-0.1.5.1.2/tuack/sample-problem/down/
+-rw-rw-rw-   0        0        0       79 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/down/1.ans
+-rw-rw-rw-   0        0        0       77 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/down/1.in
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.815846 tuack-0.1.5.1.2/tuack/sample-problem/pre/
+-rw-rw-rw-   0        0        0       80 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/pre/1.ans
+-rw-rw-rw-   0        0        0       78 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/pre/1.in
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.817337 tuack-0.1.5.1.2/tuack/sample-problem/resources/
+-rw-rw-rw-   0        0        0  3293583 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/resources/sample.png
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.822657 tuack-0.1.5.1.2/tuack/sample-problem/solution/
+-rw-rw-rw-   0        0        0     1968 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/solution/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.822657 tuack-0.1.5.1.2/tuack/sample-problem/statement/
+-rw-rw-rw-   0        0        0     6819 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/statement/zh-cn.md
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.825129 tuack-0.1.5.1.2/tuack/sample-problem/tables/
+-rw-rw-rw-   0        0        0     1062 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/tables/data.pyinc
+-rw-rw-rw-   0        0        0     1227 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/tables/json_data.json
+-rw-rw-rw-   0        0        0      205 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/sample-problem/tables/table.json
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.838401 tuack-0.1.5.1.2/tuack/templates/
+-rw-rw-rw-   0        0        0      911 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/ccc.tex.jinja
+-rw-rw-rw-   0        0        0    71170 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/templates/ccpc.png
+-rw-rw-rw-   0        0        0     1240 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/ccpc.tex.jinja
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.751611 tuack-0.1.5.1.2/tuack/templates/en/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.839397 tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     2978 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3681 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0       77 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/font.html.jinja
+-rw-rw-rw-   0        0        0       70 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/font.tex.jinja
+-rw-rw-rw-   0        0        0      670 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/hand.tex.jinja
+-rw-rw-rw-   0        0        0      144 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/image.html.jinja
+-rw-rw-rw-   0        0        0      530 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/image.tex.jinja
+-rw-rw-rw-   0        0        0     5116 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/problem_base.md.jinja
+-rw-rw-rw-   0        0        0     1051 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/table.html.jinja
+-rw-rw-rw-   0        0        0      402 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/table.md.jinja
+-rw-rw-rw-   0        0        0     2295 2018-03-03 08:40:20.000000 tuack-0.1.5.1.2/tuack/templates/table.tex.jinja
+-rw-rw-rw-   0        0        0     2125 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/template_base.tex.jinja
+-rw-rw-rw-   0        0        0      182 2019-01-19 08:45:12.000000 tuack-0.1.5.1.2/tuack/templates/template_base.tex.jinja.tex
+-rw-rw-rw-   0        0        0     4756 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/tuack.cls
+-rw-rw-rw-   0        0        0     8743 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/tuoi.tex.jinja
+-rw-rw-rw-   0        0        0     1443 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/tupc.tex.jinja
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.752802 tuack-0.1.5.1.2/tuack/templates/zh-cn/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.840485 tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/
+-rw-rw-rw-   0        0        0     3139 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/lang.mo
+-rw-rw-rw-   0        0        0     3543 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/lang.po
+-rw-rw-rw-   0        0        0    17556 2023-05-20 05:40:17.000000 tuack-0.1.5.1.2/tuack/test.py
+-rw-rw-rw-   0        0        0     3777 2023-05-18 04:27:25.000000 tuack-0.1.5.1.2/tuack/tools.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:37:45.783624 tuack-0.1.5.1.2/tuack.egg-info/
+-rw-rw-rw-   0        0        0      522 2023-05-28 15:37:44.000000 tuack-0.1.5.1.2/tuack.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     2261 2023-05-28 15:37:45.000000 tuack-0.1.5.1.2/tuack.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 15:37:44.000000 tuack-0.1.5.1.2/tuack.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       77 2023-05-28 15:37:45.000000 tuack-0.1.5.1.2/tuack.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 15:37:45.000000 tuack-0.1.5.1.2/tuack.egg-info/top_level.txt
```

### Comparing `tuack-0.1.5.1.1/LICENSE` & `tuack-0.1.5.1.2/LICENSE`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/PKG-INFO` & `tuack-0.1.5.1.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5.1.1
+Version: 0.1.5.1.2
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5.1.1/README.md` & `tuack-0.1.5.1.2/README.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/setup.py` & `tuack-0.1.5.1.2/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -34,15 +34,15 @@
 	'pyyaml >= 5.1',
 	'rarfile >= 3.0',
 	'requests_toolbelt >= 0.9.1'
 ]
 
 setup(
 	name = 'tuack',
-	version = '0.1.5.1.1',
+	version = '0.1.5.1.2',
 	packages = find_packages(),
 	author = 'Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan',
 	author_email = 'chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn',
 	url = '',
 	license = 'https://git.thusaac.com/publish/tuack/blob/master/LICENSE',
 	description = 'Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.',
 	cmdclass={
```

### Comparing `tuack-0.1.5.1.1/tuack/base.py` & `tuack-0.1.5.1.2/tuack/base.py`

 * *Files 1% similar despite different names*

```diff
@@ -571,26 +571,14 @@
 			return 2
 	return 0
 
 def mkdir(name):
 	if not os.path.exists(name):
 		os.makedirs(name)
 
-def remkdir(name):
-	while True:
-		try:
-			shutil.rmtree(name, ignore_errors = True)
-			time.sleep(0.1)
-			if not os.path.exists(name):
-				os.makedirs(name)
-			break
-		except Exception as e:
-			log.warning('Can\'t delete %s' % name)
-			log.warning(e)
-
 def copy(source, name, target):
 	full_source = pjoin(source, name)
 	if not os.path.exists(full_source):
 		raise NoFileException('No such file or path `%s`.' % full_source)
 	copied_data.add(full_source)
 	if os.path.isdir(full_source):
 		if full_source.endswith('.dir') or no_compiling:
@@ -1009,20 +997,20 @@
 	try:
 		return (True, func())
 	except Exception as e:
 		log.error(e)
 		log.info(traceback.format_exc())
 		return (False, None)
 
-def rmtree(path):
+def rmtree(path, ignore_errors = True):
 	if os.path.exists(path):
 		if system == 'Windows':
 			os.system(f'rmdir /s /q "{path}"')
 		else:
-			shutil.rmtree(path)
+			shutil.rmtree(path, ignore_errors = ignore_errors)
 
 def repeat(func):
 	las = None
 	for i in range(10):
 		try:
 			func()
 		except Exception as e:
@@ -1030,7 +1018,15 @@
 			time.sleep(1e-2)
 			log.warning(f'执行该函数第{i + 1}次：' + func.__qualname__)
 		else:
 			return
 	log.error('重复执行该函数多次失败：' + func.__qualname__)
 	log.info(getsource(func))
 	raise las
+
+def remkdir(name):
+	try:
+		repeat(lambda : rmtree(name))
+		os.makedirs(name)
+	except Exception as e:
+		log.warning('Can\'t delete %s' % name)
+		log.warning(e)
```

### Comparing `tuack-0.1.5.1.1/tuack/doc.py` & `tuack-0.1.5.1.2/tuack/doc.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/dump.py` & `tuack-0.1.5.1.2/tuack/dump.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/gen.py` & `tuack-0.1.5.1.2/tuack/gen.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/install.py` & `tuack-0.1.5.1.2/tuack/install.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/compile.pyinc` & `tuack-0.1.5.1.2/tuack/lex/compile.pyinc`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/format-linux` & `tuack-0.1.5.1.2/tuack/lex/format-linux`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/format-mac` & `tuack-0.1.5.1.2/tuack/lex/format-mac`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/format-win.exe` & `tuack-0.1.5.1.2/tuack/lex/format-win.exe`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/lex.l` & `tuack-0.1.5.1.2/tuack/lex/lex.l`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/lex.yy.c` & `tuack-0.1.5.1.2/tuack/lex/lex.yy.c`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/lex.yy.o` & `tuack-0.1.5.1.2/tuack/lex/lex.yy.o`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/yacc.tab.c` & `tuack-0.1.5.1.2/tuack/lex/yacc.tab.c`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/yacc.tab.h` & `tuack-0.1.5.1.2/tuack/lex/yacc.tab.h`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/lex/yacc.tab.o` & `tuack-0.1.5.1.2/tuack/lex/yacc.tab.o`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/load.py` & `tuack-0.1.5.1.2/tuack/load.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
 	class Checkers(File):
 		fname = ('data', 'chk', 'chk.cpp')
 		def __init__(self):
 			super(Checkers, self).__init__(*Checkers.fname)
 		def close(self):
 			super(Checkers, self).close()
 			if os.path.getsize(base.pjoin(*Checkers.fname)) < 10:
-				shutil.rmtree(base.pjoin(*Checkers.fname[:2]), ignore_errors = True)
+				base.rmtree(base.pjoin(*Checkers.fname[:2]), ignore_errors = True)
 	import re
 	key_re = re.compile('(\w*)\((\w*)\)')
 
 	if base.conf.folder != 'problem':
 		log.error(u'只能导入到一个problem的工程中。')
 		return
 	status = None
@@ -245,18 +245,18 @@
 					time.sleep(.1)
 				os.rename(pjoin('data', name), pjoin('data', name[:-4] + '.ans'))
 	if data.get('have_additional_file'):
 		download_file(base.args[0] + '/download/additional_file', 'down.zip')
 		with zipfile.ZipFile('down.zip', 'r') as z:
 			z.extractall('down')
 	else:
-		shutil.rmtree('down')
+		base.rmtree('down')
 		time.sleep(.1)
 		os.makedirs('down')
-	shutil.rmtree('pre')
+	base.rmtree('pre')
 	time.sleep(.1)
 	os.makedirs('pre')
 	base.save_json(base.conf)
 	from . import gen
 	base.run_exc(gen.work_list['auto'])
 
 def ipuoj():
@@ -323,15 +323,15 @@
 		return
 	if bpath is None:
 		bpath = base.args[0]
 	with packer(bpath) as z:
 		z.extractall('tmp')
 	data_folder('tmp')
 	time.sleep(.1)
-	shutil.rmtree('tmp')
+	base.rmtree('tmp')
 
 def data(bpath = None):
 	if base.conf.folder != 'problem':
 		log.error(u'只能导入到一个problem的工程中。')
 		return
 	if bpath is None:
 		bpath = base.args[0]
```

### Comparing `tuack-0.1.5.1.1/tuack/num2chinese.py` & `tuack-0.1.5.1.2/tuack/num2chinese.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/packer.py` & `tuack-0.1.5.1.2/tuack/packer.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/ren.py` & `tuack-0.1.5.1.2/tuack/ren.py`

 * *Files 2% similar despite different names*

```diff
@@ -78,20 +78,20 @@
 pandoc_version = None
 
 def detect_pandoc_version():
 	global pandoc_version
 	if pandoc_version is not None:
 		return
 	cp = subprocess.Popen(['pandoc', '-v'], stdout = subprocess.PIPE)
-	line = cp.stdout.read().decode().splitlines()[0]
-	pandoc_version = line.split()[-1]
+	line = cp.stdout.read().decode("utf-8", "ignore").splitlines()[0]
+	pandoc_version = tuple(map(int, line.split()[-1].split('.')))
 
 def get_pandoc_option():
 	detect_pandoc_version()
-	if pandoc_version.startswith('2.'):
+	if pandoc_version >= (2, ):
 		option = '--listings -f markdown-smart -t latex-smart'
 	else:
 		option = '--no-tex-ligatures --listings -t latex'
 	return option
 
 def get_template(fname, lang = None):
 	global env
@@ -401,28 +401,28 @@
 		time.sleep(0.1)
 
 	def check_install(self):
 		pass
 
 	def before(self):
 		base.mkdir('statements')
-		shutil.rmtree('tmp', ignore_errors = True)
+		base.rmtree('tmp', ignore_errors = True)
 		time.sleep(0.1)
 		shutil.copytree(pjoin(base.path, 'templates'), 'tmp')
 		base.mkdir(pjoin('statements', self.comp))
 		if self.conf.folder == 'contest':
 			self.contest = self.conf
 		elif self.conf.folder == 'day':
 			self.day = self.conf
 		elif self.conf.folder == 'problem':
 			self.prob = self.conf
 
 	def move_resource(self):
 		if os.path.exists(pjoin(self.prob.path, 'resources')):
-			shutil.rmtree(self.path, ignore_errors = True)
+			base.rmtree(self.path, ignore_errors = True)
 			time.sleep(0.1)
 			shutil.copytree(pjoin(self.prob.path, 'resources'), (self.path if self.prob.route != '' else pjoin(self.path, self.prob['name'])))
 
 	def gen_paths(self):
 		self.path = pjoin('statements', self.comp)
 		if self.prob.route != '':
 			self.path = pjoin(self.path, self.prob.route)
@@ -442,15 +442,15 @@
 			self.gen_paths()
 			self.move_resource()
 			self.ren_prob_md_j()
 			self.ren_prob_rest()
 			self.start_file()
 
 	def final(self):
-		shutil.rmtree('tmp', ignore_errors = True)
+		base.rmtree('tmp', ignore_errors = True)
 
 	def run(self):
 		self.check_install()
 		self.before()
 		self.main()
 		self.final()
```

### Comparing `tuack-0.1.5.1.1/tuack/sample/arbiter_e.noi_linux1.sample` & `tuack-0.1.5.1.2/tuack/sample/arbiter_e.noi_linux1.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/sample/arbiter_e.sample` & `tuack-0.1.5.1.2/tuack/sample/arbiter_e.sample`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/sample/chk.cpp` & `tuack-0.1.5.1.2/tuack/sample/chk.cpp`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/sample-problem/resources/sample.png` & `tuack-0.1.5.1.2/tuack/sample-problem/resources/sample.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/sample-problem/solution/zh-cn.md` & `tuack-0.1.5.1.2/tuack/sample-problem/solution/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/sample-problem/statement/zh-cn.md` & `tuack-0.1.5.1.2/tuack/sample-problem/statement/zh-cn.md`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/sample-problem/tables/data.pyinc` & `tuack-0.1.5.1.2/tuack/sample-problem/tables/data.pyinc`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/sample-problem/tables/json_data.json` & `tuack-0.1.5.1.2/tuack/sample-problem/tables/json_data.json`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/ccc.tex.jinja` & `tuack-0.1.5.1.2/tuack/templates/ccc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/ccpc.png` & `tuack-0.1.5.1.2/tuack/templates/ccpc.png`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/ccpc.tex.jinja` & `tuack-0.1.5.1.2/tuack/templates/ccpc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/lang.mo` & `tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/en/LC_MESSAGES/lang.po` & `tuack-0.1.5.1.2/tuack/templates/en/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/hand.tex.jinja` & `tuack-0.1.5.1.2/tuack/templates/hand.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/image.tex.jinja` & `tuack-0.1.5.1.2/tuack/templates/image.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/problem_base.md.jinja` & `tuack-0.1.5.1.2/tuack/templates/problem_base.md.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/table.html.jinja` & `tuack-0.1.5.1.2/tuack/templates/table.html.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/table.tex.jinja` & `tuack-0.1.5.1.2/tuack/templates/table.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/template_base.tex.jinja` & `tuack-0.1.5.1.2/tuack/templates/template_base.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/tuack.cls` & `tuack-0.1.5.1.2/tuack/templates/tuack.cls`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/tuoi.tex.jinja` & `tuack-0.1.5.1.2/tuack/templates/tuoi.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/tupc.tex.jinja` & `tuack-0.1.5.1.2/tuack/templates/tupc.tex.jinja`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/lang.mo` & `tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/lang.mo`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/templates/zh-cn/LC_MESSAGES/lang.po` & `tuack-0.1.5.1.2/tuack/templates/zh-cn/LC_MESSAGES/lang.po`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack/test.py` & `tuack-0.1.5.1.2/tuack/test.py`

 * *Files 0% similar despite different names*

```diff
@@ -352,15 +352,15 @@
 		(u'（共%d个包）' % len(prob.data) if len(prob.data) != 1 else u'（看样子是一个包的CPC赛制）') if prob.packed else ''
 	))
 
 	prob_failed = False
 
 	case_features = [[] for i in range(len(prob.data))]
 
-	with open(pjoin('result', prob.route) + '.csv', 'w') as fres:
+	with open(pjoin('result', prob.route) + '.csv', 'w', encoding = 'gbk' if base.system == 'Windows' else 'utf-8') as fres:
 		fres.write('%s,%s%s,summary,sample%s,pre%s\n' % (
 			prob['name'],
 			','.join(prob.test_cases),
 			',' + ','.join(map(lambda datum : '{' + ';'.join(map(str, datum['cases'])) + '}', prob.data)) \
 				if prob.packed else '',
 			','.join(prob.sample_cases),
 			','.join(prob.pre_cases)
```

### Comparing `tuack-0.1.5.1.1/tuack/tools.py` & `tuack-0.1.5.1.2/tuack/tools.py`

 * *Files identical despite different names*

### Comparing `tuack-0.1.5.1.1/tuack.egg-info/PKG-INFO` & `tuack-0.1.5.1.2/tuack.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: tuack
-Version: 0.1.5.1.1
+Version: 0.1.5.1.2
 Summary: Tools for generating an Tsinghua/OI/ICPC-styled problem or contest for multiple judges.
 Home-page: 
 Author: Chenxu Min, Zhang Ruizhe, Liu Xiaoyi, Chen Junkun, Chen Shengqi, Luo Lingxiao, Cheng Yuxuan
 Author-email: chen.xm.mu@gmail.com, 657228726@qq.com, circuitcoder0@gmail.com, 1261954105@qq.com, i@harrychen.xyz, 0.0@pku.edu.cn
 License: https://git.thusaac.com/publish/tuack/blob/master/LICENSE
 Platform: UNKNOWN
 License-File: LICENSE
```

### Comparing `tuack-0.1.5.1.1/tuack.egg-info/SOURCES.txt` & `tuack-0.1.5.1.2/tuack.egg-info/SOURCES.txt`

 * *Files identical despite different names*

