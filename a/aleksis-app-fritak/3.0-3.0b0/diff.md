# Comparing `tmp/aleksis_app_fritak-3.0.tar.gz` & `tmp/aleksis_app_fritak-3.0b0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_fritak-3.0.tar", max compression
+gzip compressed data, was "aleksis_app_fritak-3.0b0.tar", max compression
```

## Comparing `aleksis_app_fritak-3.0.tar` & `aleksis_app_fritak-3.0b0.tar`

### file list

```diff
@@ -1,47 +1,41 @@
--rw-r--r--   0        0        0     1903 2023-05-28 14:52:04.354497 aleksis_app_fritak-3.0/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0/LICENCE.rst
--rw-r--r--   0        0        0     1505 2023-03-03 16:48:40.836487 aleksis_app_fritak-3.0/README.rst
--rw-r--r--   0        0        0      735 2023-03-03 16:46:52.752874 aleksis_app_fritak-3.0/aleksis/apps/fritak/README.md
--rw-r--r--   0        0        0      214 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0/aleksis/apps/fritak/__init__.py
--rw-r--r--   0        0        0      110 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0/aleksis/apps/fritak/admin.py
--rw-r--r--   0        0        0      628 2023-03-03 16:49:41.625049 aleksis_app_fritak-3.0/aleksis/apps/fritak/apps.py
--rw-r--r--   0        0        0      800 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0/aleksis/apps/fritak/decorators.py
--rw-r--r--   0        0        0      717 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0/aleksis/apps/fritak/filters.py
--rw-r--r--   0        0        0     4599 2023-03-03 16:46:52.752874 aleksis_app_fritak-3.0/aleksis/apps/fritak/forms.py
--rw-r--r--   0        0        0     3500 2023-03-03 16:46:52.752874 aleksis_app_fritak-3.0/aleksis/apps/fritak/frontend/index.js
--rw-r--r--   0        0        0      288 2023-04-19 14:44:43.058307 aleksis_app_fritak-3.0/aleksis/apps/fritak/frontend/messages/de.json
--rw-r--r--   0        0        0      290 2023-03-03 16:46:52.752874 aleksis_app_fritak-3.0/aleksis/apps/fritak/frontend/messages/en.json
--rw-r--r--   0        0        0      363 2023-04-19 14:44:43.058307 aleksis_app_fritak-3.0/aleksis/apps/fritak/frontend/messages/ru.json
--rw-r--r--   0        0        0      343 2023-04-19 14:44:43.058307 aleksis_app_fritak-3.0/aleksis/apps/fritak/frontend/messages/uk.json
--rw-r--r--   0        0        0      463 2023-05-28 16:09:22.685183 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7830 2023-03-03 16:46:50.304923 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     6360 2023-05-28 16:09:22.685183 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    10488 2023-03-03 16:46:50.304923 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-05-28 16:09:22.685183 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7746 2023-03-03 16:46:50.304923 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-28 16:09:22.689183 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7700 2023-03-03 16:46:50.304923 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-28 16:09:22.685183 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7700 2023-03-03 16:46:50.304923 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      862 2023-05-28 16:09:22.685183 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8083 2023-04-19 14:44:43.058307 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-05-28 16:09:22.689183 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     7700 2023-03-03 16:46:50.304923 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      929 2023-05-28 16:09:22.689183 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0     8153 2023-04-19 14:44:43.058307 aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     3539 2023-03-03 16:46:52.752874 aleksis_app_fritak-3.0/aleksis/apps/fritak/migrations/0001_initial.py
--rw-r--r--   0        0        0        0 2021-01-13 16:43:21.222483 aleksis_app_fritak-3.0/aleksis/apps/fritak/migrations/__init__.py
--rw-r--r--   0        0        0     3793 2022-04-10 14:41:01.548412 aleksis_app_fritak-3.0/aleksis/apps/fritak/models.py
--rw-r--r--   0        0        0     2279 2023-03-03 16:46:52.752874 aleksis_app_fritak-3.0/aleksis/apps/fritak/rules.py
--rw-r--r--   0        0        0     1071 2022-04-10 15:03:15.127405 aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/applied_for.html
--rw-r--r--   0        0        0     1130 2022-04-10 15:21:35.645007 aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/apply_for.html
--rw-r--r--   0        0        0     1937 2022-04-10 15:20:12.996354 aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/archive.html
--rw-r--r--   0        0        0     1533 2022-04-10 15:20:39.680575 aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/archive_print.html
--rw-r--r--   0        0        0     2715 2022-04-10 15:18:44.767548 aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/check.html
--rw-r--r--   0        0        0      342 2021-01-13 16:43:21.222483 aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/edit.html
--rw-r--r--   0        0        0     2855 2022-04-10 15:15:48.337509 aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/index.html
--rw-r--r--   0        0        0      666 2022-04-10 14:41:01.548412 aleksis_app_fritak-3.0/aleksis/apps/fritak/urls.py
--rw-r--r--   0        0        0     7662 2023-04-21 16:15:47.964024 aleksis_app_fritak-3.0/aleksis/apps/fritak/views.py
--rw-r--r--   0        0        0     1454 2023-05-28 16:07:33.096458 aleksis_app_fritak-3.0/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-03-03 16:46:52.756874 aleksis_app_fritak-3.0/tox.ini
--rw-r--r--   0        0        0     2493 1970-01-01 00:00:00.000000 aleksis_app_fritak-3.0/PKG-INFO
+-rw-r--r--   0        0        0     1447 2023-02-28 12:44:25.916196 aleksis_app_fritak-3.0b0/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0b0/LICENCE.rst
+-rw-r--r--   0        0        0     1487 2022-04-10 14:41:01.548412 aleksis_app_fritak-3.0b0/README.rst
+-rw-r--r--   0        0        0      735 2023-02-28 12:44:25.920196 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/README.md
+-rw-r--r--   0        0        0      214 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/__init__.py
+-rw-r--r--   0        0        0      110 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/admin.py
+-rw-r--r--   0        0        0      630 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/apps.py
+-rw-r--r--   0        0        0      800 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/decorators.py
+-rw-r--r--   0        0        0      717 2021-01-13 16:43:21.218483 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/filters.py
+-rw-r--r--   0        0        0     4599 2023-02-28 12:44:25.920196 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/forms.py
+-rw-r--r--   0        0        0     3500 2023-02-28 12:44:25.920196 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/frontend/index.js
+-rw-r--r--   0        0        0      290 2023-02-28 12:44:25.924197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/frontend/messages/en.json
+-rw-r--r--   0        0        0      463 2022-04-11 09:16:14.957116 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7830 2023-02-28 12:44:25.924197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     6360 2022-04-11 09:16:14.961117 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    10491 2023-02-28 12:44:25.924197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2022-04-11 09:16:14.957116 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7746 2023-02-28 12:44:25.924197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-04-11 09:16:14.961117 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7700 2023-02-28 12:44:25.928197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-04-11 09:16:14.957116 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7700 2023-02-28 12:44:25.928197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2022-04-11 09:16:14.957116 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0     7700 2023-02-28 12:44:25.928197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     3539 2023-02-28 12:44:25.928197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/migrations/0001_initial.py
+-rw-r--r--   0        0        0        0 2021-01-13 16:43:21.222483 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/migrations/__init__.py
+-rw-r--r--   0        0        0     3793 2022-04-10 14:41:01.548412 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/models.py
+-rw-r--r--   0        0        0     2279 2023-02-28 12:44:25.928197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/rules.py
+-rw-r--r--   0        0        0     1071 2022-04-10 15:03:15.127405 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/applied_for.html
+-rw-r--r--   0        0        0     1130 2022-04-10 15:21:35.645007 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/apply_for.html
+-rw-r--r--   0        0        0     1937 2022-04-10 15:20:12.996354 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/archive.html
+-rw-r--r--   0        0        0     1533 2022-04-10 15:20:39.680575 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/archive_print.html
+-rw-r--r--   0        0        0     2715 2022-04-10 15:18:44.767548 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/check.html
+-rw-r--r--   0        0        0      342 2021-01-13 16:43:21.222483 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/edit.html
+-rw-r--r--   0        0        0     2855 2022-04-10 15:15:48.337509 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/index.html
+-rw-r--r--   0        0        0      666 2022-04-10 14:41:01.548412 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/urls.py
+-rw-r--r--   0        0        0     7712 2023-02-28 12:44:25.928197 aleksis_app_fritak-3.0b0/aleksis/apps/fritak/views.py
+-rw-r--r--   0        0        0     1505 2023-02-28 12:44:25.928197 aleksis_app_fritak-3.0b0/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-02-28 12:44:25.932196 aleksis_app_fritak-3.0b0/tox.ini
+-rw-r--r--   0        0        0     2918 1970-01-01 00:00:00.000000 aleksis_app_fritak-3.0b0/setup.py
+-rw-r--r--   0        0        0     2463 1970-01-01 00:00:00.000000 aleksis_app_fritak-3.0b0/PKG-INFO
```

### Comparing `aleksis_app_fritak-3.0/CHANGELOG.rst` & `aleksis_app_fritak-3.0b0/CHANGELOG.rst`

 * *Files 13% similar despite different names*

```diff
@@ -2,39 +2,28 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`3.0`_ - 2022-05-28
--------------------
 
-Fixed
-~~~~~
+Unreleased
+----------
 
-* Add missing translations for new SPA frontend.
-* Exemption request archive was not available.
-* Submitting new requests wasn't working.
-
-`3.0b0` - 2022-02-28
---------------------
+Added
+~~~~~
 
-This version requires AlekSIS-Core 3.0. It is incompatible with any previous
-version.
+* Add support for new SPA
 
 Removed
 ~~~~~~~
 
-* Legacy menu integration for AlekSIS-Core pre-3.0
-
-Added
-~~~~~
+* Drop compatibility with AlekSIS-Core series 2.x
 
-* Add SPA support for AlekSIS-Core 3.0
 
 `2.0.1`_ - 2022-08-10
 ---------------------
 
 Fixed
 ~~~~~
 
@@ -83,9 +72,7 @@
 .. _Semantic Versioning: https://semver.org/spec/v2.0.0.html
 
 
 .. _2.0b0: https://edugit.org/Katharineum/AlekSIS-App-Fritak/-/tags/2.0b0
 .. _2.0b1: https://edugit.org/Katharineum/AlekSIS-App-Fritak/-/tags/2.0b1
 .. _2.0: https://edugit.org/Katharineum/AlekSIS-App-Fritak/-/tags/2.0
 .. _2.0.1: https://edugit.org/Katharineum/AlekSIS-App-Fritak/-/tags/2.0.1
-.. _3.0b0: https://edugit.org/Katharineum/AlekSIS-App-Fritak/-/tags/3.0b0
-.. _3.0: https://edugit.org/Katharineum/AlekSIS-App-Fritak/-/tags/3.0
```

### Comparing `aleksis_app_fritak-3.0/LICENCE.rst` & `aleksis_app_fritak-3.0b0/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/README.rst` & `aleksis_app_fritak-3.0b0/README.rst`

 * *Files 7% similar despite different names*

```diff
@@ -1,9 +1,9 @@
-Unofficial AlekSIS App Fritak (Management of exemption requests)
-================================================================
+AlekSIS — Unofficial App Fritak (exemption requests)
+====================================================
 
 AlekSIS
 -------
 
 This is an **unofficial** application for use with the `AlekSIS`_ platform.
 
 Features
```

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/README.md` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/README.md`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/apps.py` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/apps.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 from aleksis.core.util.apps import AppConfig
 
 
 class FritakConfig(AppConfig):
     name = "aleksis.apps.fritak"
-    verbose_name = "Fritak (Management of exemption requests)"
+    verbose_name = "AlekSIS — Fritak (Exemption requests)"
 
     urls = {
         "Repository": "https://edugit.org/katharineum/AlekSIS-App-Fritak",
     }
     licence = "EUPL-1.2+"
     copyright_info = (
         ([2017, 2018, 2019, 2020], "Frank Poetzsch-Heffter", "p-h@katharineum.de"),
```

#### encoding

```diff
@@ -1 +1 @@
-us-ascii
+utf-8
```

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/decorators.py` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/decorators.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/filters.py` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/forms.py` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/frontend/index.js` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/ar/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-28 12:07+0100\n"
+"POT-Creation-Date: 2022-04-10 17:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/de_DE/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,18 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-28 12:07+0100\n"
+"POT-Creation-Date: 2020-08-02 16:08+0200\n"
 "PO-Revision-Date: 2022-04-10 15:30+0000\n"
 "Last-Translator: Jonathan Weth <teckids@jonathanweth.de>\n"
-"Language-Team: German <https://translate.edugit.org/projects/katharineum-aleksis/aleksis-app-fritak/de/>\n"
+"Language-Team: German <https://translate.edugit.org/projects/"
+"katharineum-aleksis/aleksis-app-fritak/de/>\n"
 "Language: de_DE\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=n != 1;\n"
 "X-Generator: Weblate 4.8\n"
```

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-28 12:07+0100\n"
+"POT-Creation-Date: 2022-04-10 17:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/la/LC_MESSAGES/django.po` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/la/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-28 12:07+0100\n"
+"POT-Creation-Date: 2022-04-10 17:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
 #, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-28 12:07+0100\n"
+"POT-Creation-Date: 2022-04-10 17:27+0200\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language-Team: LANGUAGE <LL@li.org>\n"
 "Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
```

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files 3% similar despite different names*

```diff
@@ -1,29 +1,25 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
 # FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+#, fuzzy
 msgid ""
 msgstr ""
 "Project-Id-Version: PACKAGE VERSION\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2023-02-28 12:07+0100\n"
-"PO-Revision-Date: 2023-03-04 14:29+0000\n"
-"Last-Translator: Serhii Horichenko <m@sgg.im>\n"
-"Language-Team: Russian <https://translate.edugit.org/projects/"
-"katharineum-aleksis/aleksis-app-fritak/ru/>\n"
-"Language: ru\n"
+"POT-Creation-Date: 2022-04-10 17:27+0200\n"
+"PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
+"Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
+"Language-Team: LANGUAGE <LL@li.org>\n"
+"Language: \n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n"
-"%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n"
-"%100>=11 && n%100<=14)? 2 : 3);\n"
-"X-Generator: Weblate 4.12.1\n"
 
 #: aleksis/apps/fritak/filters.py:21 aleksis/apps/fritak/models.py:43
 msgid "Submitter"
 msgstr ""
 
 #: aleksis/apps/fritak/forms.py:51 aleksis/apps/fritak/forms.py:63
 #: aleksis/apps/fritak/templates/fritak/archive_print.html:34
@@ -128,15 +124,15 @@
 #: aleksis/apps/fritak/models.py:36
 msgid "End time"
 msgstr ""
 
 #: aleksis/apps/fritak/models.py:49
 #: aleksis/apps/fritak/templates/fritak/archive.html:46
 msgid "Status"
-msgstr "Состояние"
+msgstr ""
 
 #: aleksis/apps/fritak/models.py:65
 msgid "Your request for an exemption from teaching was approved"
 msgstr ""
 
 #: aleksis/apps/fritak/models.py:67
 msgid "Your request for an exemption from teaching from {}, {} to {}, {} was approved by the school management."
@@ -188,30 +184,30 @@
 
 #: aleksis/apps/fritak/templates/fritak/apply_for.html:9
 msgid "Submit new request for exemption from teaching"
 msgstr ""
 
 #: aleksis/apps/fritak/templates/fritak/apply_for.html:18
 msgid "Submit"
-msgstr "Отправить"
+msgstr ""
 
 #: aleksis/apps/fritak/templates/fritak/archive.html:5
 #: aleksis/apps/fritak/templates/fritak/archive.html:9
 #: aleksis/apps/fritak/templates/fritak/archive_print.html:8
 msgid "Archive of Exemption Requests"
 msgstr ""
 
 #: aleksis/apps/fritak/templates/fritak/archive.html:26
 msgid "Update filters"
 msgstr ""
 
 #: aleksis/apps/fritak/templates/fritak/archive.html:34
 #: aleksis/apps/fritak/templates/fritak/archive_print.html:24
 msgid "Person"
-msgstr "Физ.лицо"
+msgstr ""
 
 #: aleksis/apps/fritak/templates/fritak/archive.html:38
 msgid "Time Range"
 msgstr ""
 
 #: aleksis/apps/fritak/templates/fritak/archive.html:42
 msgid "Description"
@@ -265,23 +261,23 @@
 
 #: aleksis/apps/fritak/templates/fritak/index.html:15
 msgid "Make a new request"
 msgstr ""
 
 #: aleksis/apps/fritak/templates/fritak/index.html:37
 msgid "Edit"
-msgstr "Редактировать"
+msgstr ""
 
 #: aleksis/apps/fritak/templates/fritak/index.html:47
 msgid "Do you really want to delete the request?"
 msgstr ""
 
 #: aleksis/apps/fritak/templates/fritak/index.html:49
 msgid "Delete"
-msgstr "Удалить"
+msgstr ""
 
 #: aleksis/apps/fritak/views.py:35
 msgid "Request for exemption from teaching deleted"
 msgstr ""
 
 #: aleksis/apps/fritak/views.py:37
 msgid "You have deleted your request for class exemptionfor the period from {} to {}."
```

#### encoding

```diff
@@ -1 +1 @@
-utf-8
+us-ascii
```

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/migrations/0001_initial.py` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/models.py` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/models.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/rules.py` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/applied_for.html` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/applied_for.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/apply_for.html` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/apply_for.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/archive.html` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/archive.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/archive_print.html` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/archive_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/check.html` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/check.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/templates/fritak/index.html` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/templates/fritak/index.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/urls.py` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/aleksis/apps/fritak/views.py` & `aleksis_app_fritak-3.0b0/aleksis/apps/fritak/views.py`

 * *Files 5% similar despite different names*

```diff
@@ -79,20 +79,22 @@
                 from_time=from_time,
                 to_date=to_date,
                 to_time=to_time,
                 description=description,
                 submitter=request.user.person,
             )
             exemption_request.save()
-            assign_perm("fritak.view_exemptionrequest", request.user, exemption_request)
             assign_perm(
-                "fritak.change_exemptionrequest", request.user, exemption_request
+                "fritak.view_exemptionrequest_rule", request.user, exemption_request
             )
             assign_perm(
-                "fritak.delete_exemptionrequest", request.user, exemption_request
+                "fritak.change_exemptionrequest_rule", request.user, exemption_request
+            )
+            assign_perm(
+                "fritak.delete_exemptionrequest_rule", request.user, exemption_request
             )
             from_date = formats.date_format(from_date)
             to_date = formats.date_format(to_date)
 
             a = Activity(
                 user=request.user.person,
                 title=_("Application for exemption from teaching submitted"),
@@ -191,15 +193,15 @@
     if not is_print:
         exemption_list = ExemptionRequest.objects.filter(
             Q(status__exact=2) | Q(status__exact=3)
         ).order_by("-from_date")
     else:
         exemption_list = ExemptionRequest.objects.all().order_by("from_date")
     exemption_list = get_objects_for_user(
-        request.user, "fritak.view_exemptionrequest", exemption_list
+        request.user, "fritak.view_exemptionrequest_rule", exemption_list
     )
 
     if not is_print:
         exemption_filter = ExemptionFilter(request.GET, queryset=exemption_list)
         return render(request, "fritak/archive.html", {"filter": exemption_filter})
     else:
         return render_pdf(
```

### Comparing `aleksis_app_fritak-3.0/pyproject.toml` & `aleksis_app_fritak-3.0b0/pyproject.toml`

 * *Files 18% similar despite different names*

```diff
@@ -1,27 +1,28 @@
 [tool.poetry]
 name = "AlekSIS-App-Fritak"
-version = "3.0"
+version = "3.0b0"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
     { path = "docs/*", format = "sdist" },
     { path = "docs/**/*", format = "sdist" },
     { path = "conftest.py", format = "sdist" },
     { path = "tox.ini", format = "sdist" }
 ]
 
-description = "Unofficial AlekSIS App Fritak (Management of exemption requests)"
+description = "AlekSIS (School Information System) — App Fritak (application management)"
 authors = ["Julian Leucker <leuckeju@katharineum.de>", "Frank Poetzsch-Heffter <p-h@katharineum.de>", "Jonathan Weth <dev@jonathanweth.de>", "Hangzhi Yu <yuha@katharineum.de>"]
 maintainers = ["Frank Poetzsch-Heffter <p-h@katharineum.de>", "Jonathan Weth <dev@jonathanweth.de>"]
 license = "EUPL-1.2"
+homepage = "https://aleksis.org/"
 repository = "https://edugit.org/katharineum/AlekSIS-App-Fritak"
 classifiers = [
     "Development Status :: 5 - Production/Stable",
     "Environment :: Web Environment",
     "Intended Audience :: Education",
     "Topic :: Education"
 ]
@@ -29,15 +30,15 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = "^3.0"
+aleksis-core = "^3.0b0"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
 
 [tool.poetry.plugins."aleksis.app"]
 fritak = "aleksis.apps.fritak.apps:FritakConfig"
```

### Comparing `aleksis_app_fritak-3.0/tox.ini` & `aleksis_app_fritak-3.0b0/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_fritak-3.0/PKG-INFO` & `aleksis_app_fritak-3.0b0/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 Metadata-Version: 2.1
 Name: aleksis-app-fritak
-Version: 3.0
-Summary: Unofficial AlekSIS App Fritak (Management of exemption requests)
-Home-page: https://edugit.org/katharineum/AlekSIS-App-Fritak
+Version: 3.0b0
+Summary: AlekSIS (School Information System) — App Fritak (application management)
+Home-page: https://aleksis.org/
 License: EUPL-1.2
 Author: Julian Leucker
 Author-email: leuckeju@katharineum.de
 Maintainer: Frank Poetzsch-Heffter
 Maintainer-email: p-h@katharineum.de
 Requires-Python: >=3.9,<4.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -14,20 +14,20 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=3.0,<4.0)
+Requires-Dist: aleksis-core (>=3.0b0,<4.0)
 Project-URL: Repository, https://edugit.org/katharineum/AlekSIS-App-Fritak
 Description-Content-Type: text/x-rst
 
-Unofficial AlekSIS App Fritak (Management of exemption requests)
-================================================================
+AlekSIS — Unofficial App Fritak (exemption requests)
+====================================================
 
 AlekSIS
 -------
 
 This is an **unofficial** application for use with the `AlekSIS`_ platform.
 
 Features
```

