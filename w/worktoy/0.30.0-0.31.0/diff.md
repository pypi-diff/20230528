# Comparing `tmp/worktoy-0.30.0.tar.gz` & `tmp/worktoy-0.31.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "worktoy-0.30.0.tar", last modified: Thu May 18 22:43:08 2023, max compression
+gzip compressed data, was "worktoy-0.31.0.tar", last modified: Sun May 28 09:10:02 2023, max compression
```

## Comparing `worktoy-0.30.0.tar` & `worktoy-0.31.0.tar`

### file list

```diff
@@ -1,60 +1,75 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.642198 worktoy-0.30.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-18 22:42:59.000000 worktoy-0.30.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-18 22:43:08.642198 worktoy-0.30.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6497 2023-05-18 22:42:59.000000 worktoy-0.30.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-18 22:42:59.000000 worktoy-0.30.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-18 22:43:08.642198 worktoy-0.30.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.634198 worktoy-0.30.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.638198 worktoy-0.30.0/src/worktoy/
--rw-r--r--   0 runner    (1001) docker     (123)      792 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_anywayuwantit.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_argument.py
--rw-r--r--   0 runner    (1001) docker     (123)     4580 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     5748 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     8353 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_field.py
--rw-r--r--   0 runner    (1001) docker     (123)     2266 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_hereismynumber.py
--rw-r--r--   0 runner    (1001) docker     (123)      422 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_maybeType.py
--rw-r--r--   0 runner    (1001) docker     (123)      746 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_maybeTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     3547 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_monospace.py
--rw-r--r--   0 runner    (1001) docker     (123)      355 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_overload.py
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_overloadlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     4320 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_parameterlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     3773 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_parsify.py
--rw-r--r--   0 runner    (1001) docker     (123)     2419 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_parsifyerrors.py
--rw-r--r--   0 runner    (1001) docker     (123)     3194 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_searchKeys.py
--rw-r--r--   0 runner    (1001) docker     (123)      634 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_searchterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     2368 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_stringlist.py
--rw-r--r--   0 runner    (1001) docker     (123)     1378 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_textbetween.py
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_typenames.py
--rw-r--r--   0 runner    (1001) docker     (123)     5008 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_workdict.py
--rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_workdictmeta.py
--rw-r--r--   0 runner    (1001) docker     (123)      510 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/_workmeta.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.638198 worktoy-0.30.0/src/worktoy/mockdata/
--rw-r--r--   0 runner    (1001) docker     (123)      227 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/mockdata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/mockdata/_intfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/mockdata/_strfactory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.642198 worktoy-0.30.0/src/worktoy/sharperexceptions/
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/_argumenterror.py
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/_parsingerror.py
--rw-r--r--   0 runner    (1001) docker     (123)     6675 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/_readonlyerror.py
--rw-r--r--   0 runner    (1001) docker     (123)      949 2023-05-18 22:42:59.000000 worktoy-0.30.0/src/worktoy/sharperexceptions/_testexception.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.638198 worktoy-0.30.0/src/worktoy.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6990 2023-05-18 22:43:08.000000 worktoy-0.30.0/src/worktoy.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1468 2023-05-18 22:43:08.000000 worktoy-0.30.0/src/worktoy.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-18 22:43:08.000000 worktoy-0.30.0/src/worktoy.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-18 22:43:08.000000 worktoy-0.30.0/src/worktoy.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-18 22:43:08.642198 worktoy-0.30.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      619 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__ArgumentError.py
--rw-r--r--   0 runner    (1001) docker     (123)     3589 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__callmemaybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1128 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__intfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)      726 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__maybe.py
--rw-r--r--   0 runner    (1001) docker     (123)     1110 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__maybeType.py
--rw-r--r--   0 runner    (1001) docker     (123)     1677 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__maybeTypes.py
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__readonlyerror.py
--rw-r--r--   0 runner    (1001) docker     (123)     6084 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__searchKeys.py
--rw-r--r--   0 runner    (1001) docker     (123)     3212 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__searchterm.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__strfactory.py
--rw-r--r--   0 runner    (1001) docker     (123)     1830 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__stringlist.py
--rw-r--r--   0 runner    (1001) docker     (123)      740 2023-05-18 22:42:59.000000 worktoy-0.30.0/tests/test__textbetween.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.572964 worktoy-0.31.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1075 2023-05-28 09:09:53.000000 worktoy-0.31.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-28 09:10:02.572964 worktoy-0.31.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3551 2023-05-28 09:09:53.000000 worktoy-0.31.0/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-05-28 09:09:53.000000 worktoy-0.31.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      555 2023-05-28 09:10:02.572964 worktoy-0.31.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/worktoy/
+-rw-r--r--   0 runner    (1001) docker     (123)      315 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/worktoy/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      276 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1130 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/_empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1226 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/_maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/_plenty.py
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/core/_some.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/worktoy/dio/
+-rw-r--r--   0 runner    (1001) docker     (123)      211 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/dio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      230 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/dio/_fileaccess.py
+-rw-r--r--   0 runner    (1001) docker     (123)      143 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/dio/_filewalk.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1224 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/dio/_loadfile.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/field/
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/field/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2943 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/field/_basefield.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/parsing/
+-rw-r--r--   0 runner    (1001) docker     (123)      401 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1376 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/_extractarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      480 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/_maybetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)      754 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/_maybetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3559 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/parsing/_searchkeys.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/stringtools/
+-rw-r--r--   0 runner    (1001) docker     (123)      316 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      812 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/_camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1369 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/_justify.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2052 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/_monospace.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1700 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/stringtools/_stringlist.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/typetools/
+-rw-r--r--   0 runner    (1001) docker     (123)      279 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/_any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2111 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/_callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2464 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/_tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2557 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/typetools/_typebag.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.568964 worktoy-0.31.0/src/worktoy/waitaminute/
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1088 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_accesserror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      469 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_dioerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1438 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_exceptioncore.py
+-rw-r--r--   0 runner    (1001) docker     (123)      845 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_instantiationerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      738 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_manualinterrupt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      887 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_n00berror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1804 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_proceduralerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6791 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_readonlyerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      865 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_typeguarderror.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1474 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_unexpectedstateerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_validationerror.py
+-rw-r--r--   0 runner    (1001) docker     (123)      889 2023-05-28 09:09:53.000000 worktoy-0.31.0/src/worktoy/waitaminute/_valueguard.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.564964 worktoy-0.31.0/src/worktoy.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4044 2023-05-28 09:10:02.000000 worktoy-0.31.0/src/worktoy.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1920 2023-05-28 09:10:02.000000 worktoy-0.31.0/src/worktoy.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 09:10:02.000000 worktoy-0.31.0/src/worktoy.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-05-28 09:10:02.000000 worktoy-0.31.0/src/worktoy.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 09:10:02.572964 worktoy-0.31.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      614 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__any.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3369 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__basefield.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1418 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__callmemaybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1158 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__camelcase.py
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__empty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2306 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__extractarg.py
+-rw-r--r--   0 runner    (1001) docker     (123)      780 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__maybe.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1225 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__maybetype.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1568 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__maybetypes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__plenty.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6125 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__searchkeys.py
+-rw-r--r--   0 runner    (1001) docker     (123)      608 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__some.py
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__tuple.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1494 2023-05-28 09:09:53.000000 worktoy-0.31.0/tests/test__typebag.py
```

### Comparing `worktoy-0.30.0/LICENSE` & `worktoy-0.31.0/LICENSE`

 * *Files identical despite different names*

### Comparing `worktoy-0.30.0/pyproject.toml` & `worktoy-0.31.0/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 [build-system]
 requires = ['setuptools>=63.2']
 build-backend = 'setuptools.build_meta'
 
 
 [project]
 name = "worktoy"
-version = "0.30.0"
+version = "0.31.0"
 authors = [
     { name = "Asger Jon Vistisen", email = "asgerjon2@gmail.com" },
 ]
 description = "Collection of Utilities"
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
```

### Comparing `worktoy-0.30.0/setup.cfg` & `worktoy-0.31.0/setup.cfg`

 * *Files 19% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [METADATA]
 name = WorkToy
-version = 0.30.0
+version = 0.31.0
 author = Asger Jon Vistisen
 author_email = asgerjon2@gmail.com
 description = A Collection of Utilities
 long_description = file:README.md,LICENSE
 long_description_content_type = text/markdown
 url = 
 project_urls =
```

### Comparing `worktoy-0.30.0/src/worktoy/_maybeTypes.py` & `worktoy-0.31.0/src/worktoy/parsing/_maybetypes.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """The maybeTypes function finds all arguments of given type"""
-#  MIT License
 #  Copyright (c) 2023 Asger Jon Vistisen
+#  MIT Licence
 from __future__ import annotations
 
 from typing import Any
 
-from worktoy import searchKeys
+from worktoy.parsing import searchKeys
 
 
 def maybeTypes(type_, *args, **kwargs) -> list[Any]:
   """The maybeTypes function finds all arguments of given type"""
   #  MIT License
   #  Copyright (c) 2023 Asger Jon Vistisen
```

### Comparing `worktoy-0.30.0/src/worktoy/_monospace.py` & `worktoy-0.31.0/src/worktoy/stringtools/_monospace.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,55 +1,15 @@
 """Documentation: monoSpace
 Convert text to monospaced format with consistent spacing and line
-  breaks.
-
-  Args:
-    text (str): The input text to be modified.
-    newLine (str, optional):
-      The string representing the line break. If not provided,
-      the default value '<br>' is used. Defaults to None.
-
-  Returns:
-    str: The modified text with consistent spacing and line breaks.
-
-  Raises:
-    None
-
-  Examples:
-    >>> monoSpace('Hello   World!')
-    'Hello World!'
-    >>> monoSpace('Hello<br>World!', '<br>')
-    'Hello\nWorld!'
-
-  The `monoSpace` function takes a string `text` and an optional string
-  `newLine`, and returns a modified version of the input text with consistent
-  spacing and line breaks. If the `newLine` argument is not provided, the
-  default value '<br>' is used as the line break string.
-
-  The function performs the following steps:
-  1. Replaces all occurrences of '\n' and '\r' characters with a space ' ' in
-     the input `text`.
-  2. Repeatedly replaces multiple consecutive spaces with a single space
-     until no more consecutive spaces are found in the `text`.
-  3. Replaces the `newLine` string (or the default '<br>' if not provided)
-     with a line break '\n' character in the modified `text`.
-  4. Returns the modified `text`.
-
-  Note:
-  - The `newLine` string is treated as a literal string, so make sure to
-    provide the exact string to be replaced as the line break.
-  - The `newLine` string is case-sensitive. If the provided `newLine` string
-    does not match the exact case in the input `text`, it will not be
-    replaced with a line break.
-"""
-#  MIT License
+  breaks."""
 #  Copyright (c) 2023 Asger Jon Vistisen
+#  MIT Licence
 from __future__ import annotations
 
-from worktoy import maybe
+from worktoy.core import maybe
 
 
 def monoSpace(text: str, newLine: str = None) -> str:
   """Convert text to monospaced format with consistent spacing and line
   breaks.
 
   Args:
```

### Comparing `worktoy-0.30.0/src/worktoy/_parsify.py` & `worktoy-0.31.0/src/worktoy/parsing/_searchkeys.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,115 +1,124 @@
-"""Parsify is a class providing a systematic parsing of positional and
-keyword arguments for flexible use in functions and classes."""
-#  MIT License
+"""The searchKeys function provides a flexible way of extracting values
+from keyword arguments."""
 #  Copyright (c) 2023 Asger Jon Vistisen
+#  MIT Licence
 from __future__ import annotations
 
-from typing import Any, Never, NoReturn
+from typing import Any, NoReturn
 
-from worktoy import PositionalArgumentError, searchKeys, maybeType
-from worktoy.sharperexceptions import ReadOnlyError
+from worktoy.typetools import CallMeMaybe
 
 
-class Parsify:
-  """Parsify is a class providing a systematic parsing of positional and
-  keyword arguments for flexible use in functions and classes.
+class _SearchKeys:
+  """The searchKeys function provides a flexible way of extracting values
+  from keyword arguments.
   #  MIT License
   #  Copyright (c) 2023 Asger Jon Vistisen"""
 
-  def __init__(self, *args, **kwargs) -> None:
-    self._curInd = 0
-    self._posArgs = [*args]
-    self._keyArgs = kwargs
-
-  def _removePosArg(self, posArg: Any = None) -> Any:
-    """Arg must be in self._posArgs. This method removes it. This method
-    must be invoked by any methods which transmits a positional argument
-    to the outside, so that it does not get spent multiple times."""
-    if posArg is None:
+  @classmethod
+  def searchKeys(cls, *keys: str) -> _SearchKeys:
+    """Creates a new instance on the given keys"""
+    allKeys = []
+    for key in keys:
+      if isinstance(key, (list, tuple)):
+        allKeys = [*allKeys, *key]
+      else:
+        allKeys.append(key)
+    out = cls()
+    out._setKeys(*allKeys)
+    return out
+
+  def __init__(self, ) -> None:
+    self._keys = []
+    self._types = []
+    self._defVal = None
+
+  def _clearKeys(self) -> NoReturn:
+    """Deleter-function for the instance keys"""
+    while self._keys:
+      self._keys.pop()
+
+  def _setKeys(self, *keys: str) -> NoReturn:
+    """Setter-function for the instance keys"""
+    self._clearKeys()
+    for key in keys:
+      if isinstance(key, str):
+        self._keys.append(key)
+
+  def _clearTypes(self) -> NoReturn:
+    """Clears the type list"""
+    while self._types:
+      self._types.pop()
+
+  def _setType(self, *type_: type) -> NoReturn:
+    """Setter-function for type """
+    self._clearTypes()
+    for arg in type_:
+      if isinstance(arg, type):
+        self._types.append(arg)
+
+  def _resetDefaultValue(self) -> NoReturn:
+    """Deleter-function for default value"""
+    self._defVal = None
+
+  def _setDefaultValue(self, dV: Any) -> NoReturn:
+    """Setter-function for the default value"""
+    self._defVal = dV
+
+  def _getDefaultValue(self) -> Any:
+    """Getter-function for the default value"""
+    return self._defVal
+
+  def _validateByType(self, arg: Any) -> Any:
+    """Returns the argument if it matches instance type. If instance type
+    is None, any argument is returned."""
+    if arg is None:
       return None
-    for arg in self:
-      pass
+    if not self._types:
+      return arg
+    for type_ in self._types:
+      if isinstance(arg, type_):
+        return arg
+    return None
+
+  def _invoke(self, **kwargs) -> Any:
+    """Invokes the function"""
+    for key in self._keys:
+      val = self._validateByType(kwargs.get(key, None))
+      if val is not None:
+        return val
+      val = self._validateByType(kwargs.get(key.lower(), None))
+      if val is not None:
+        return val
+    return self._getDefaultValue()
+
+  def __matmul__(self, other: tuple[type, ...] | type) -> _SearchKeys:
+    """Sets the types for this instance"""
+    if other is None:
+      return self
+    if isinstance(other, type):
+      self._setType(other)
+      return self
+    if isinstance(other, (list, tuple)):
+      self._setType(*other)
+      return self
+    if other is CallMeMaybe:
+      self._setType(CallMeMaybe)
+      return self
+
+  def __rshift__(self, other: tuple[dict, Any] | dict) -> Any:
+    """Evaluates the keyword arguments given. If a tuple is given,
+    the first member of it are assumed to be the keyword argument
+    dictionary and the second member is the default value. If a dict is
+    given, no default value can be given, and the dict is processed
+    directly."""
+    self._resetDefaultValue()
+    if isinstance(other, tuple):
+      kwargs = other[0]
+      if len(other) > 1:
+        self._setDefaultValue(other[1])
+      return self._invoke(**kwargs)
+    return self._invoke(**other)
 
-  def _removeKeyArg(self, key: str = None) -> Any:
-    """The key maps to a member of kwarg which is then overwritten."""
-    val = searchKeys(key) >> self._keyArgs
-    if val is None:
-      return None
-    self._keyArgs |= {key: None}
-    return val
-
-  def _getPosType(self, type_: type) -> Any:
-    """Getter-function for the first positional argument of the given type"""
-
-  def __contains__(self, posArg: Any) -> bool:
-    """posArg in self checks if given argument is one of the positional
-    arguments"""
-    for arg in self:
-      if arg == posArg:
-        return True
-    return False
-
-  def __getitem__(self, index: int | str) -> NoReturn:
-    """Implementation of item getting"""
-    if isinstance(index, int):
-      return self._getByIndex(index, )
-    if isinstance(index, str):
-      return self._getByKey(index, )
-    msg = """Expected index to be one of %s or %s, but received: %s"""
-    raise TypeError(msg % (str, int, type(index)))
-
-  def __setitem__(self, index: int | str, val: Any = None) -> NoReturn:
-    """Implementation item setting."""
-    if isinstance(index, int):
-      return self._setByIndex(index, val)
-    if isinstance(index, str):
-      return self._setByKey(index, val)
-    msg = """Expected index to be one of %s or %s, but received: %s"""
-    raise TypeError(msg % (str, int, type(index)))
-
-  def _getByIndex(self, index: int) -> Any:
-    """Item getter by index"""
-    raise NotImplementedError
-
-  def _setByIndex(self, index: int, val: Any) -> NoReturn:
-    """Item getter by index"""
-    raise NotImplementedError
-
-  def _getByKey(self, key: str) -> Any:
-    """Item getter by index"""
-    raise NotImplementedError
-
-  def _setByKey(self, key: str, val: Any) -> Any:
-    """Item getter by index"""
-    raise NotImplementedError
-
-  def __len__(self) -> int:
-    """The length of the instance is understood to mean the number of
-    positional arguments"""
-    return len(self.posArgs)
-
-  def __iter__(self, ) -> Parsify:
-    """Implementation of iteration applies to the positional arguments"""
-    self._curInd = 0
-    return self
-
-  def __next__(self, ) -> Any:
-    """Implementation of iteration applies to the positional arguments"""
-    self._curInd += 1
-    if self._curInd > len(self):
-      raise StopIteration
-    return self.posArgs[self._curInd - 1]
-
-  def _getPosArgs(self) -> list[Any]:
-    """Getter-function for list of positional arguments"""
-    return self._posArgs
-
-  def _setPosArgs(self, *_) -> Never:
-    """Illegal setter-function"""
-    raise ReadOnlyError('posArgs')
-
-  def _delPosArgs(self, *_) -> Never:
-    """Illegal setter-function"""
-    raise ReadOnlyError('posArgs')
 
-  posArgs = property(_getPosArgs, _setPosArgs, _delPosArgs)
+searchKeys = _SearchKeys.searchKeys
```

### Comparing `worktoy-0.30.0/src/worktoy/_stringlist.py` & `worktoy-0.31.0/src/worktoy/stringtools/_stringlist.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 """The stringList function provides an easier way to write lists of
 strings. Instead of wrapping each item in ticks, write on long string with
 consistent separators, and stringList will convert it to a list of
 strings.
 Instead of: numbers = ['one', 'two', 'three', 'four']
 Use stringList: numbers = stringList('one, two, three, four')"""
-#  MIT License
 #  Copyright (c) 2023 Asger Jon Vistisen
+#  MIT Licence
 from __future__ import annotations
 
-from worktoy import searchKeys, maybeTypes, maybe
-from worktoy.mockdata import strFactory
+from worktoy.core import maybe
+from worktoy.parsing import maybeTypes, searchKeys
 
 
 def stringList(*args, **kwargs) -> list[str]:
   """The stringList function provides an easier way to write lists of
   strings. Instead of wrapping each item in ticks, write on long string with
   consistent separators, and stringList will convert it to a list of
   strings.
@@ -24,30 +24,16 @@
   separators on the same text.
   #  MIT License
   #  Copyright (c) 2023 Asger Jon Vistisen"""
 
   strArgs = maybeTypes(str, *args, padLen=3, padChar=None)
   sourceKwarg = searchKeys('source', 'src', 'txt') @ str >> kwargs
   separatorKwarg = searchKeys('separator', 'splitHere') @ str >> kwargs
-  ignoreKwarg = searchKeys('ignoreChar', 'ignore') @ str >> kwargs
   sourceArg, separatorArg, ignoreArg = strArgs
-  sourceDefault, separatorDefault, ignoreDefault = None, ', ', '@'
+  sourceDefault, separatorDefault = None, ', '
   source = maybe(sourceKwarg, sourceArg, sourceDefault)
   separator = maybe(separatorKwarg, separatorArg, separatorDefault, )
-  # separator = separator.replace(' ', '')
-  ignore = maybe(ignoreKwarg, ignoreArg, ignoreDefault)
   if source is None:
     msg = 'stringList received no string!'
     raise ValueError(msg)
-  # if ignore == 'LOL':
-  #   print(ignore)
-  ignoreSeparator = '%s%s' % (ignore, separator)
-  tempIgnore = '___%s___' % (strFactory(16))
-  source = source.replace(ignoreSeparator, tempIgnore)
-  # preSpace = ' %s' % separator
-  # postSpace = '%s ' % separator
-  # while preSpace in source:
-  #   source = source.replace(preSpace, separator)
-  # while postSpace in source:
-  #   source = source.replace(postSpace, separator)
   out = source.split(separator)
-  return [word.replace(tempIgnore, separator) for word in out]
+  return out
```

### Comparing `worktoy-0.30.0/src/worktoy/sharperexceptions/_readonlyerror.py` & `worktoy-0.31.0/src/worktoy/waitaminute/_readonlyerror.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,68 +1,78 @@
 """Documentation: ReadOnlyError"""
-#  MIT License
 #  Copyright (c) 2023 Asger Jon Vistisen
+#  MIT Licence
 from __future__ import annotations
+
 import inspect
 from typing import Never
+
 from icecream import ic
-from worktoy import monoSpace, searchKeys, maybe
+
+from worktoy.core import maybe
+from worktoy.parsing import searchKeys
+from worktoy.stringtools import monoSpace
+from worktoy.waitaminute import ExceptionCore
 
 ic.configureOutput(includeContext=True)
 
 
-class ReadOnlyError(Exception):
-  """Custom exception for read-only operations.
-  Attributes:
-      varName (str): Name of the variable.
-      function (str): Name of the function invoking the error.
-      fileName (str): Name of the file where the error occurred.
-      lineNumber (int): Line number where the error occurred.
-      insName (object): Instance where the error occurred.
-      insCls (class): Class of the instance where the error
-      occurred."""
+class ReadOnlyError(ExceptionCore):
+  """Custom exception for read-only operations."""
 
   @classmethod
-  def yoDawg(cls) -> Exception:
+  def Field(cls, Field) -> ReadOnlyError:
+    """Creates an instance of read only error based on a field"""
+    varName = Field.getName()
+    ownerName = Field.getOwner()
+    return ReadOnlyError(varName, ownerName, )
+
+  @classmethod
+  def yoDawg(cls) -> ExceptionCore:
     """Create an exception instance of ReadOnlyError."""
-    msg = "Heard you like read-only exceptions, so we put a read-only " \
-          "error in your read-only error!"
-    return Exception(msg)
+    msg = """Heard you like ReadOnlyError, so we put a ReadOnlyError
+          in your ReadOnlyError!"""
+    from worktoy.stringtools import monoSpace
+    return ExceptionCore(monoSpace(msg))
 
   def __init__(self, *args, **kwargs) -> None:
     """Initialize the ReadOnlyError exception.
     Args:
         *args: Variable arguments.
         **kwargs: Keyword arguments.
     Raises:
         None
     Returns:
         None"""
-    args = maybe(args, [None, ])
+    self._variableName = None
+    self._function = None
+    self._fileName = None
+    self._lineNumber = None
+    self._instance = None
+    self._instanceClass = None
+    ExceptionCore.__init__(self, *args, **kwargs)
+
+  def _createMsg(self, *args, **kwargs) -> str:
+    """Reimplementation"""
+    args = [*args, None]
     variableKwarg = searchKeys('variable', 'var') @ str >> kwargs
     variableArg = args[0]
     self._variableName = maybe(variableKwarg, variableArg, None)
     frame = inspect.currentframe().f_back
     code = frame.f_code
     self._function = inspect.getframeinfo(frame).function
     self._fileName = code.co_filename
     self._lineNumber = frame.f_lineno
     self._instance = frame.f_locals.get('self', )
     self._instanceClass = type(self._instance)
-    super().__init__(monoSpace(self.__str__()))
-
-  def __str__(self) -> str:
-    """Return a string representation of the exception.
-    Returns:
-        str: String representation of the exception."""
     msg = "Tried to access %s belonging to %s of class %s using %s, " \
           "which is not a permitted operation!"
-    msg = monoSpace(msg % (
+    self._msg = monoSpace(msg % (
       self.varName, self.insName, self.insCls, self.function))
-    return msg
+    return self._msg
 
   def _getVariable(self) -> str:
     """Getter-function for the name of the variable.
     Returns:
         str: Name of the variable."""
     return maybe(self._variableName, 'unnamed')
```

### Comparing `worktoy-0.30.0/src/worktoy.egg-info/SOURCES.txt` & `worktoy-0.31.0/src/worktoy.egg-info/SOURCES.txt`

 * *Files 14% similar despite different names*

```diff
@@ -1,52 +1,62 @@
 LICENSE
 README.md
 pyproject.toml
 setup.cfg
 src/worktoy/__init__.py
-src/worktoy/_anywayuwantit.py
-src/worktoy/_argument.py
-src/worktoy/_callmemaybe.py
-src/worktoy/_core.py
-src/worktoy/_field.py
-src/worktoy/_hereismynumber.py
-src/worktoy/_maybe.py
-src/worktoy/_maybeType.py
-src/worktoy/_maybeTypes.py
-src/worktoy/_monospace.py
-src/worktoy/_overload.py
-src/worktoy/_overloadlist.py
-src/worktoy/_parameterlist.py
-src/worktoy/_parsify.py
-src/worktoy/_parsifyerrors.py
-src/worktoy/_searchKeys.py
-src/worktoy/_searchterm.py
-src/worktoy/_stringlist.py
-src/worktoy/_textbetween.py
-src/worktoy/_typenames.py
-src/worktoy/_workdict.py
-src/worktoy/_workdictmeta.py
-src/worktoy/_workmeta.py
 src/worktoy.egg-info/PKG-INFO
 src/worktoy.egg-info/SOURCES.txt
 src/worktoy.egg-info/dependency_links.txt
 src/worktoy.egg-info/top_level.txt
-src/worktoy/mockdata/__init__.py
-src/worktoy/mockdata/_intfactory.py
-src/worktoy/mockdata/_strfactory.py
-src/worktoy/sharperexceptions/__init__.py
-src/worktoy/sharperexceptions/_argumenterror.py
-src/worktoy/sharperexceptions/_parsingerror.py
-src/worktoy/sharperexceptions/_readonlyerror.py
-src/worktoy/sharperexceptions/_testexception.py
-tests/test__ArgumentError.py
+src/worktoy/core/__init__.py
+src/worktoy/core/_empty.py
+src/worktoy/core/_maybe.py
+src/worktoy/core/_plenty.py
+src/worktoy/core/_some.py
+src/worktoy/dio/__init__.py
+src/worktoy/dio/_fileaccess.py
+src/worktoy/dio/_filewalk.py
+src/worktoy/dio/_loadfile.py
+src/worktoy/field/__init__.py
+src/worktoy/field/_basefield.py
+src/worktoy/parsing/__init__.py
+src/worktoy/parsing/_extractarg.py
+src/worktoy/parsing/_maybetype.py
+src/worktoy/parsing/_maybetypes.py
+src/worktoy/parsing/_searchkeys.py
+src/worktoy/stringtools/__init__.py
+src/worktoy/stringtools/_camelcase.py
+src/worktoy/stringtools/_justify.py
+src/worktoy/stringtools/_monospace.py
+src/worktoy/stringtools/_stringlist.py
+src/worktoy/typetools/__init__.py
+src/worktoy/typetools/_any.py
+src/worktoy/typetools/_callmemaybe.py
+src/worktoy/typetools/_tuple.py
+src/worktoy/typetools/_typebag.py
+src/worktoy/waitaminute/__init__.py
+src/worktoy/waitaminute/_accesserror.py
+src/worktoy/waitaminute/_dioerror.py
+src/worktoy/waitaminute/_exceptioncore.py
+src/worktoy/waitaminute/_instantiationerror.py
+src/worktoy/waitaminute/_manualinterrupt.py
+src/worktoy/waitaminute/_n00berror.py
+src/worktoy/waitaminute/_proceduralerror.py
+src/worktoy/waitaminute/_readonlyerror.py
+src/worktoy/waitaminute/_typeguarderror.py
+src/worktoy/waitaminute/_unexpectedstateerror.py
+src/worktoy/waitaminute/_validationerror.py
+src/worktoy/waitaminute/_valueguard.py
+tests/test__any.py
+tests/test__basefield.py
 tests/test__callmemaybe.py
-tests/test__intfactory.py
+tests/test__camelcase.py
+tests/test__empty.py
+tests/test__extractarg.py
 tests/test__maybe.py
-tests/test__maybeType.py
-tests/test__maybeTypes.py
-tests/test__readonlyerror.py
-tests/test__searchKeys.py
-tests/test__searchterm.py
-tests/test__strfactory.py
-tests/test__stringlist.py
-tests/test__textbetween.py
+tests/test__maybetype.py
+tests/test__maybetypes.py
+tests/test__plenty.py
+tests/test__searchkeys.py
+tests/test__some.py
+tests/test__tuple.py
+tests/test__typebag.py
```

### Comparing `worktoy-0.30.0/tests/test__readonlyerror.py` & `worktoy-0.31.0/src/worktoy/field/_basefield.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,84 +1,91 @@
-"""Testing ReadOnlyError"""
-#  MIT License
+"""BaseField decorates classes with fields"""
 #  Copyright (c) 2023 Asger Jon Vistisen
+#  MIT Licence
 from __future__ import annotations
+from typing import Any, NoReturn
 
-import unittest
-from typing import Any
+from icecream import ic
 
-from worktoy import monoSpace
+from worktoy.core import maybe
+from worktoy.parsing import searchKeys
+from worktoy.stringtools import stringList
+from worktoy.waitaminute import ReadOnlyError, ProceduralError
 
+ic.configureOutput(includeContext=True)
 
-class ReadOnlyError(Exception):
-  """Custom exception for read-only operations."""
 
-  def __init__(self, var_name: str, function: str) -> None:
-    """Initialize the ReadOnlyError exception.
+class BaseField:
+  """field decorates a class a with a field
+  #  Copyright (c) 2023 Asger Jon Vistisen
+  #  MIT Licence"""
 
-    Args:
-        var_name (str): Name of the variable.
-        function (str): Name of the function invoking the error.
-    """
-    self.var_name = var_name
-    self.function = function
-    super().__init__(self.__str__())
-
-  def __str__(self) -> str:
-    """Return a string representation of the exception.
-
-    Returns:
-        str: String representation of the exception.
-    """
-    return monoSpace(
-      f"Tried to access {self.var_name} using {self.function}, which is "
-      f"not a permitted operation!"
-    )
-
-
-class MyClass:
-  """Example class that raises ReadOnlyError exceptions."""
-
-  def __init__(self, value: Any) -> None:
+  def __init__(self, name: str, value: Any, **kwargs) -> None:
+    self._name = name
     self._value = value
+    self._defVal = value
+    typeArg = None if self._value is None else type(self._value)
+    readOnlyKeys = stringList('readOnly, noSet, lock, writeProtect')
+    readOnly = searchKeys(*readOnlyKeys) @ bool >> kwargs
+    self._readOnly = True if readOnly else False
+    typeKeys = stringList('type, type_, class, class_')
+    typeKwarg = searchKeys(typeKeys) >> kwargs
+    self._type = maybe(typeArg, typeKwarg, None)
+    if self._type is None:
+      raise ProceduralError('_type', type, None)
+    self._owner = None
+    self._instance = None
 
-  @property
-  def value(self) -> Any:
-    """Getter for the value property."""
+  def __get__(self, *args) -> Any:
+    """Implementation of getter"""
     return self._value
 
-  @value.setter
-  def value(self, new_value: Any) -> None:
-    """Setter for the value property."""
-    raise ReadOnlyError("value", "setter")
-
-  @value.deleter
-  def value(self) -> None:
-    """Deleter for the value property."""
-    raise ReadOnlyError("value", "deleter")
-
-
-class TestReadOnlyError(unittest.TestCase):
-  """Unit tests for ReadOnlyError"""
-
-  def setUp(self) -> None:
-    """Set up test fixtures"""
-    pass
-
-  def tearDown(self) -> None:
-    """Tear down test fixtures"""
-    pass
-
-  def test_read_only_exception(self) -> None:
-    """Test ReadOnlyError exception"""
-    my_obj = MyClass("initial_value")
-
-    # Accessing the value property should not raise an exception
-    self.assertEqual(my_obj.value, "initial_value")
-
-    # Attempting to set the value property should raise ReadOnlyError
-    with self.assertRaises(ReadOnlyError):
-      my_obj.value = "new_value"
-
-    # Attempting to delete the value property should raise ReadOnlyError
-    with self.assertRaises(ReadOnlyError):
-      del my_obj.value
+  def __set__(self, *args, ) -> NoReturn:
+    """Implementation of setter"""
+    if self._readOnly:
+      raise ReadOnlyError.Field(self)
+    if self._instance is None:
+      self._instance = args[0]
+    self._value = args[1]
+
+  def __call__(self, cls: type) -> type:
+    """Decorates the class"""
+    fields = getattr(cls, '__fields__', None)
+    if fields is None:
+      fields = {}
+    fields |= {self.getName(): self}
+    setattr(cls, '__fields__', fields)
+    self._owner = cls
+    setattr(cls, self._name, self)
+    return cls
+
+  def getName(self) -> str:
+    """Getter-function for the name of the field"""
+    return self._name
+
+  def getOwner(self) -> type:
+    """Getter-function for the owner class"""
+    if self._owner is None:
+      raise ProceduralError('_owner', type, None)
+    return self._owner
+
+  def getInstance(self, ) -> Any:
+    """Getter-function for the owner instance"""
+    return self._instance
+
+  def __str__(self, ) -> str:
+    """String Representation"""
+    msg = """BaseField %s on class %s and instance %s."""
+    return msg % (self.getName(), self.getOwner(), self.getInstance())
+
+  def __repr__(self) -> str:
+    """Code Representation"""
+    className = self.__class__.__name__
+    if self._readOnly:
+      if self._defVal is None:
+        msg = '%s(%s, type_=%s, readOnly=True)'
+        return msg % (className, self.getName(), self._type)
+      msg = """%s(%s, %s, readOnly=True)"""
+      return msg % (className, self.getName(), self._defVal,)
+    if self._defVal is None:
+      return '%s(%s, type_=%s)' % (className, self.getName(), self._type)
+    return '%s(%s, %s)' % (className, self.getName(), self._defVal)
```

### Comparing `worktoy-0.30.0/tests/test__searchKeys.py` & `worktoy-0.31.0/tests/test__searchkeys.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 """Testing the searchKeys"""
-#  MIT License
 #  Copyright (c) 2023 Asger Jon Vistisen
+#  MIT Licence
 from __future__ import annotations
 
 from random import randint, sample, choice, random
 import string
 from typing import NoReturn, Callable, Any
 from unittest import TestCase
 
-from worktoy import searchKeys, CallMeMaybe
+from worktoy.typetools import CallMeMaybe
+from worktoy.parsing import searchKeys
 
 
 def _someFunc() -> NoReturn:
   """Hi there, I'm a function!"""
   return None
 
 
@@ -109,17 +110,17 @@
     self.valueDicts = {}
     for (key, (type_, val)) in zip(self.goodKeys,
                                    zip(self.types, self.values)):
       self.typeDicts |= {key: type_}
       self.valueDicts |= {key: val}
     self.defVal = {
       tuple: self.newTuple(3),
-      int  : 69420,
+      int: 69420,
       float: .1337,
-      str  : 'lol',
+      str: 'lol',
     }
 
   def testCallMeMaybe(self) -> NoReturn:
     """Testing if searchKeys can handle searching for callables"""
     testKwarg = {'here': _someFunc, 'lol': 77777, 'blabla': 777777777}
     res = searchKeys('here', 'there') @ CallMeMaybe >> testKwarg
     self.assertEqual(res, _someFunc)
@@ -143,15 +144,15 @@
     intVal = searchKeys(*self.goodKeys) @ int >> self.valueDicts
     self.assertIsInstance(intVal, int)
     tupleVal = searchKeys(*self.goodKeys) @ tuple >> self.valueDicts
     self.assertIsInstance(tupleVal, tuple)
     floatVal = searchKeys(*self.goodKeys) @ float >> self.valueDicts
     self.assertIsInstance(floatVal, float)
     strVal = searchKeys(*self.goodKeys) @ str >> self.valueDicts
-    self.assertIsInstance(strVal, str)
+    self.assertIsInstance(strVal, str, strVal)
 
   def testSingleTypeMultiKey(self) -> NoReturn:
     """Testing good keys, but bad combinations of types"""
     for k1 in self.goodKeys:
       for k2 in [key for key in self.goodKeys if key != k1]:
         for (type_, defVal) in self.defVal.items():
           t1, t2 = [self.typeDicts.get(k, None) for k in [k1, k2]]
```

### Comparing `worktoy-0.30.0/tests/test__textbetween.py` & `worktoy-0.31.0/tests/test__maybe.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,26 +1,28 @@
-"""Unit tests for the textBetween function."""
-#  MIT License
 #  Copyright (c) 2023 Asger Jon Vistisen
-from __future__ import annotations
-
+#  MIT Licence
+from random import shuffle
 from typing import NoReturn
 from unittest import TestCase
 
-from loremify import lorem
-
-from worktoy import textBetween
+from worktoy.core import maybe
 
 
-class TextBetweenTestCase(TestCase):
-  """Unit tests for the textBetween function."""
+class TestMaybe(TestCase):
+  """Testing the 'maybe' function"""
 
   def setUp(self) -> NoReturn:
-    """Sets up the classes"""
-    self.sample = """This is a <b>test</b> for bold fonts! <p>and this is 
-    a paragraph</p>. This should not found. <b>bla</b>___"""
-
-  def testSimple(self) -> NoReturn:
-    """Testing simple case"""
-    prediction = ['test', 'bla']
-    reality = textBetween(self.sample, '<b>', '</b>')
-    self.assertEqual(prediction, reality)
+    """Setting up each test"""
+    self.someFalse = [0, 0j, False, dict(), set(), tuple(), list(), '']
+
+  def testNoArgs(self) -> NoReturn:
+    """Testing the case with no arguments"""
+    self.assertIsNone(maybe())
+
+  def testingEach(self) -> NoReturn:
+    """For each type in someFalse, we check if is extracted from a pile of
+    None"""
+    pile = [None for _ in range(255)]
+    for val in self.someFalse:
+      draw = [*pile, val]
+      shuffle(draw)
+      self.assertIsInstance(maybe(*draw), type(val))
```

