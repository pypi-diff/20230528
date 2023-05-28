# Comparing `tmp/loutilities-3.8.2.tar.gz` & `tmp/loutilities-3.8.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "loutilities-3.8.2.tar", last modified: Wed May 10 10:10:17 2023, max compression
+gzip compressed data, was "loutilities-3.8.3.tar", last modified: Sun May 28 11:12:27 2023, max compression
```

## Comparing `loutilities-3.8.2.tar` & `loutilities-3.8.3.tar`

### file list

```diff
@@ -1,128 +1,128 @@
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.485629 loutilities-3.8.2/
--rw-rw-rw-   0        0        0      483 2012-11-11 22:51:42.000000 loutilities-3.8.2/.gitattributes
--rw-rw-rw-   0        0        0     1709 2020-09-24 11:16:31.000000 loutilities-3.8.2/.gitignore
--rw-rw-rw-   0        0        0     2073 2023-05-10 10:10:17.484629 loutilities-3.8.2/PKG-INFO
--rw-rw-rw-   0        0        0     1811 2020-05-28 21:02:31.000000 loutilities-3.8.2/README.md
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.017130 loutilities-3.8.2/loutilities/
--rw-rw-rw-   0        0        0     1248 2013-01-15 19:29:28.000000 loutilities-3.8.2/loutilities/__init__.py
--rw-rw-rw-   0        0        0    16727 2023-01-21 20:20:08.000000 loutilities-3.8.2/loutilities/agegrade.py
--rw-rw-rw-   0        0        0     5767 2019-11-21 10:01:11.000000 loutilities-3.8.2/loutilities/apikey.py
--rw-rw-rw-   0        0        0     5329 2021-12-03 11:20:03.000000 loutilities-3.8.2/loutilities/applytemplate.py
--rw-rw-rw-   0        0        0    31804 2019-11-20 17:25:22.000000 loutilities-3.8.2/loutilities/bfile.py
--rw-rw-rw-   0        0        0     1809 2019-11-20 17:48:38.000000 loutilities-3.8.2/loutilities/boolexpr.py
--rw-rw-rw-   0        0        0     1597 2019-11-21 10:16:04.000000 loutilities-3.8.2/loutilities/config.py
--rw-rw-rw-   0        0        0     1577 2019-11-25 21:48:03.000000 loutilities-3.8.2/loutilities/configparser.py
--rw-rw-rw-   0        0        0     2726 2019-11-20 19:29:11.000000 loutilities-3.8.2/loutilities/csvu.py
--rw-rw-rw-   0        0        0    16776 2021-12-02 12:11:45.000000 loutilities-3.8.2/loutilities/csvwt.py
--rw-rw-rw-   0        0        0    10771 2019-11-25 21:46:41.000000 loutilities-3.8.2/loutilities/extconfigparser.py
--rw-rw-rw-   0        0        0     8147 2019-11-25 21:48:03.000000 loutilities-3.8.2/loutilities/filetrigger.py
--rw-rw-rw-   0        0        0     4592 2019-11-25 21:48:13.000000 loutilities-3.8.2/loutilities/filtercsv.py
--rw-rw-rw-   0        0        0     3315 2022-12-05 19:41:06.000000 loutilities-3.8.2/loutilities/filters.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.066628 loutilities-3.8.2/loutilities/flask/
--rw-rw-rw-   0        0        0       34 2021-02-23 18:59:56.000000 loutilities-3.8.2/loutilities/flask/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.097636 loutilities-3.8.2/loutilities/flask/user/
--rw-rw-rw-   0        0        0       37 2021-02-23 18:59:56.000000 loutilities-3.8.2/loutilities/flask/user/__init__.py
--rw-rw-rw-   0        0        0     4390 2021-03-01 13:08:41.000000 loutilities-3.8.2/loutilities/flask/user/views.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.128628 loutilities-3.8.2/loutilities/flask_helpers/
--rw-rw-rw-   0        0        0        0 2018-07-18 20:55:43.000000 loutilities-3.8.2/loutilities/flask_helpers/__init__.py
--rw-rw-rw-   0        0        0     1631 2019-11-20 17:25:25.000000 loutilities-3.8.2/loutilities/flask_helpers/as_blueprint.py
--rw-rw-rw-   0        0        0     2976 2019-11-20 17:46:54.000000 loutilities-3.8.2/loutilities/flask_helpers/blueprints.py
--rw-rw-rw-   0        0        0     2756 2020-07-14 16:48:05.000000 loutilities-3.8.2/loutilities/flask_helpers/decorators.py
--rw-rw-rw-   0        0        0     2270 2023-05-10 10:01:07.000000 loutilities-3.8.2/loutilities/flask_helpers/mailer.py
--rw-rw-rw-   0        0        0    10781 2017-12-24 09:46:57.000000 loutilities-3.8.2/loutilities/geo.py
--rw-rw-rw-   0        0        0    12067 2022-04-02 22:20:21.000000 loutilities-3.8.2/loutilities/googleauth.py
--rw-rw-rw-   0        0        0    10705 2019-11-27 11:58:53.000000 loutilities-3.8.2/loutilities/kmlutils.py
--rw-rw-rw-   0        0        0     2448 2019-11-20 19:39:19.000000 loutilities-3.8.2/loutilities/makerst.py
--rw-rw-rw-   0        0        0     8990 2019-11-20 17:25:23.000000 loutilities-3.8.2/loutilities/namesplitter.py
--rw-rw-rw-   0        0        0     6267 2020-09-27 19:23:54.000000 loutilities-3.8.2/loutilities/nesteddict.py
--rw-rw-rw-   0        0        0    22227 2020-05-27 10:57:20.000000 loutilities-3.8.2/loutilities/nicknames.csv
--rw-rw-rw-   0        0        0     1557 2020-05-27 11:34:23.000000 loutilities-3.8.2/loutilities/nicknames.py
--rw-rw-rw-   0        0        0     6266 2021-04-11 17:38:17.000000 loutilities-3.8.2/loutilities/renderrun.py
--rw-rw-rw-   0        0        0     4057 2019-11-20 19:41:28.000000 loutilities-3.8.2/loutilities/sqlalchemy_helpers.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.131629 loutilities-3.8.2/loutilities/tables-assets/
--rw-rw-rw-   0        0        0     1154 2019-06-27 16:58:21.000000 loutilities-3.8.2/loutilities/tables-assets/readme.md
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.265629 loutilities-3.8.2/loutilities/tables-assets/static/
--rw-rw-rw-   0        0        0     7595 2021-05-27 19:24:36.000000 loutilities-3.8.2/loutilities/tables-assets/static/background-post-data-manager.js
--rw-rw-rw-   0        0        0      168 2019-06-15 15:35:48.000000 loutilities-3.8.2/loutilities/tables-assets/static/branding.css
--rw-rw-rw-   0        0        0      927 2017-12-06 20:12:04.000000 loutilities-3.8.2/loutilities/tables-assets/static/buttons.colvis.js
--rw-rw-rw-   0        0        0      521 2019-05-12 00:41:26.000000 loutilities-3.8.2/loutilities/tables-assets/static/charts.css
--rw-rw-rw-   0        0        0    19829 2022-04-15 19:49:44.000000 loutilities-3.8.2/loutilities/tables-assets/static/charts.js
--rw-rw-rw-   0        0        0    30498 2021-04-05 11:19:07.000000 loutilities-3.8.2/loutilities/tables-assets/static/datatables-childrow.js
--rw-rw-rw-   0        0        0     3581 2021-07-12 16:09:36.000000 loutilities-3.8.2/loutilities/tables-assets/static/datatables.css
--rw-rw-rw-   0        0        0     1413 2020-04-03 11:12:13.000000 loutilities-3.8.2/loutilities/tables-assets/static/datatables.dataRender.datetime.js
--rw-rw-rw-   0        0        0     1141 2019-07-16 17:38:55.000000 loutilities-3.8.2/loutilities/tables-assets/static/datatables.dataRender.ellipsis.js
--rw-rw-rw-   0        0        0      700 2021-02-16 21:49:34.000000 loutilities-3.8.2/loutilities/tables-assets/static/datatables.dataRender.googledoc.js
--rw-rw-rw-   0        0        0    22430 2021-07-16 21:09:07.000000 loutilities-3.8.2/loutilities/tables-assets/static/datatables.js
--rw-rw-rw-   0        0        0     5340 2021-07-17 16:33:30.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor-saeditor.js
--rw-rw-rw-   0        0        0     2329 2020-10-28 19:15:54.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor.buttons.editchildrowrefresh.js
--rw-rw-rw-   0        0        0     1977 2020-08-03 13:49:06.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor.buttons.editrefresh.js
--rw-rw-rw-   0        0        0      190 2021-03-30 19:14:25.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor.buttons.separator.js
--rw-rw-rw-   0        0        0     3517 2020-07-01 18:34:03.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor.ckeditor5.js
--rw-rw-rw-   0        0        0      185 2019-07-13 20:36:24.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor.css
--rw-rw-rw-   0        0        0     2144 2020-07-13 11:15:00.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor.displayController.onPage.js
--rw-rw-rw-   0        0        0     1265 2020-03-23 14:12:29.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor.fieldType.display.js
--rw-rw-rw-   0        0        0     1757 2020-09-29 18:49:14.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor.googledoc.js
--rw-rw-rw-   0        0        0     1993 2020-04-16 19:38:46.000000 loutilities-3.8.2/loutilities/tables-assets/static/editor.select2.mymethods.js
--rw-rw-rw-   0        0        0     2088 2019-02-16 21:05:41.000000 loutilities-3.8.2/loutilities/tables-assets/static/eventscalendar.css
--rw-rw-rw-   0        0        0      381 2019-06-30 18:16:58.000000 loutilities-3.8.2/loutilities/tables-assets/static/filters.css
--rw-rw-rw-   0        0        0     3697 2020-04-07 18:55:39.000000 loutilities-3.8.2/loutilities/tables-assets/static/filters.js
--rw-rw-rw-   0        0        0     2254 2017-12-11 10:45:42.000000 loutilities-3.8.2/loutilities/tables-assets/static/jquery.ui.dialog-clickoutside.js
--rw-rw-rw-   0        0        0      331 2021-04-13 21:51:31.000000 loutilities-3.8.2/loutilities/tables-assets/static/jqueryui.theme.adjust.css
--rw-rw-rw-   0        0        0      454 2018-12-15 20:43:56.000000 loutilities-3.8.2/loutilities/tables-assets/static/legend.js
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:16.772044 loutilities-3.8.2/loutilities/tables-assets/static/user/
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.271627 loutilities-3.8.2/loutilities/tables-assets/static/user/admin/
--rw-rw-rw-   0        0        0      646 2022-05-09 20:13:08.000000 loutilities-3.8.2/loutilities/tables-assets/static/user/admin/beforedatatables.js
--rw-rw-rw-   0        0        0     7208 2021-02-24 20:30:38.000000 loutilities-3.8.2/loutilities/tables-assets/static/user/admin/groups.js
--rw-rw-rw-   0        0        0     4391 2021-07-16 21:09:23.000000 loutilities-3.8.2/loutilities/tables-assets/static/utils.js
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.299630 loutilities-3.8.2/loutilities/tables-assets/templates/
--rw-rw-rw-   0        0        0       36 2019-12-09 22:56:02.000000 loutilities-3.8.2/loutilities/tables-assets/templates/bare-layout.jinja2
--rw-rw-rw-   0        0        0      142 2019-06-14 14:56:28.000000 loutilities-3.8.2/loutilities/tables-assets/templates/datatables.html
--rw-rw-rw-   0        0        0     3720 2020-06-25 18:51:11.000000 loutilities-3.8.2/loutilities/tables-assets/templates/datatables.jinja2
--rw-rw-rw-   0        0        0     4243 2022-05-13 20:20:15.000000 loutilities-3.8.2/loutilities/tables-assets/templates/layout-base.jinja2
--rw-rw-rw-   0        0        0      130 2019-06-14 14:55:29.000000 loutilities-3.8.2/loutilities/tables-assets/templates/layout.html
--rw-rw-rw-   0        0        0      837 2019-06-21 21:28:23.000000 loutilities-3.8.2/loutilities/tables-assets/templates/layout.jinja2
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.334629 loutilities-3.8.2/loutilities/tables-assets/templates/security/
--rw-rw-rw-   0        0        0      860 2022-09-25 00:43:58.000000 loutilities-3.8.2/loutilities/tables-assets/templates/security/change_password.jinja2
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.385630 loutilities-3.8.2/loutilities/tables-assets/templates/security/email/
--rw-rw-rw-   0        0        0      514 2022-09-25 00:43:58.000000 loutilities-3.8.2/loutilities/tables-assets/templates/security/email/reset_instructions.html
--rw-rw-rw-   0        0        0      454 2022-09-25 00:43:58.000000 loutilities-3.8.2/loutilities/tables-assets/templates/security/email/reset_instructions.txt
--rw-rw-rw-   0        0        0      614 2022-09-25 00:43:58.000000 loutilities-3.8.2/loutilities/tables-assets/templates/security/forgot_password.jinja2
--rw-rw-rw-   0        0        0     1601 2022-09-25 00:43:58.000000 loutilities-3.8.2/loutilities/tables-assets/templates/security/login_user.jinja2
--rw-rw-rw-   0        0        0      698 2022-09-25 00:43:58.000000 loutilities-3.8.2/loutilities/tables-assets/templates/security/reset_password.jinja2
--rw-rw-rw-   0        0        0     1455 2021-03-01 17:16:14.000000 loutilities-3.8.2/loutilities/tables-assets/templates/select-view.jinja2
--rw-rw-rw-   0        0        0   150885 2023-01-04 19:40:01.000000 loutilities-3.8.2/loutilities/tables.py
--rw-rw-rw-   0        0        0    20360 2021-12-03 18:46:39.000000 loutilities-3.8.2/loutilities/textreader.py
--rw-rw-rw-   0        0        0     7657 2021-04-16 18:58:16.000000 loutilities-3.8.2/loutilities/timeu.py
--rw-rw-rw-   0        0        0     2410 2021-03-12 20:12:30.000000 loutilities-3.8.2/loutilities/transform.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.454636 loutilities-3.8.2/loutilities/user/
--rw-rw-rw-   0        0        0     4439 2023-05-04 16:45:05.000000 loutilities-3.8.2/loutilities/user/__init__.py
--rw-rw-rw-   0        0        0     4085 2021-10-23 20:08:52.000000 loutilities-3.8.2/loutilities/user/applogging.py
--rw-rw-rw-   0        0        0     1641 2020-03-12 20:37:30.000000 loutilities-3.8.2/loutilities/user/audit_mixin.py
--rw-rw-rw-   0        0        0    12730 2023-04-25 16:10:29.000000 loutilities-3.8.2/loutilities/user/model.py
--rw-rw-rw-   0        0        0     3194 2022-02-01 18:24:58.000000 loutilities-3.8.2/loutilities/user/roles.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.461632 loutilities-3.8.2/loutilities/user/scripts/
--rw-rw-rw-   0        0        0        0 2020-01-02 18:24:31.000000 loutilities-3.8.2/loutilities/user/scripts/__init__.py
--rw-rw-rw-   0        0        0     4768 2021-01-23 19:25:09.000000 loutilities-3.8.2/loutilities/user/scripts/users_init.py
--rw-rw-rw-   0        0        0     2883 2020-03-06 21:27:20.000000 loutilities-3.8.2/loutilities/user/settings.py
--rw-rw-rw-   0        0        0     8323 2020-05-02 15:41:47.000000 loutilities-3.8.2/loutilities/user/tablefiles.py
--rw-rw-rw-   0        0        0    23503 2021-03-29 20:03:03.000000 loutilities-3.8.2/loutilities/user/tables.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.466627 loutilities-3.8.2/loutilities/user/views/
--rw-rw-rw-   0        0        0      612 2020-03-06 10:51:08.000000 loutilities-3.8.2/loutilities/user/views/__init__.py
--rw-rw-rw-   0        0        0    22789 2022-01-31 19:41:13.000000 loutilities-3.8.2/loutilities/user/views/userrole.py
--rw-rw-rw-   0        0        0      110 2023-05-10 10:09:06.000000 loutilities-3.8.2/loutilities/version.py
--rw-rw-rw-   0        0        0    13429 2019-11-27 20:15:01.000000 loutilities-3.8.2/loutilities/wxextensions.py
--rw-rw-rw-   0        0        0     5040 2019-11-20 20:09:06.000000 loutilities-3.8.2/loutilities/xmldict.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.063631 loutilities-3.8.2/loutilities.egg-info/
--rw-rw-rw-   0        0        0     2073 2023-05-10 10:10:11.000000 loutilities-3.8.2/loutilities.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     4270 2023-05-10 10:10:11.000000 loutilities-3.8.2/loutilities.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-10 10:10:11.000000 loutilities-3.8.2/loutilities.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0      210 2023-05-10 10:10:11.000000 loutilities-3.8.2/loutilities.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0        2 2018-12-17 13:25:37.000000 loutilities-3.8.2/loutilities.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       26 2023-05-10 10:10:11.000000 loutilities-3.8.2/loutilities.egg-info/requires.txt
--rw-rw-rw-   0        0        0       18 2023-05-10 10:10:11.000000 loutilities-3.8.2/loutilities.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-10 10:10:17.485629 loutilities-3.8.2/setup.cfg
--rw-rw-rw-   0        0        0     2468 2022-10-05 20:49:08.000000 loutilities-3.8.2/setup.py
-drwxrwxrwx   0        0        0        0 2023-05-10 10:10:17.481630 loutilities-3.8.2/tests/
--rw-rw-rw-   0        0        0        0 2018-07-03 19:25:32.000000 loutilities-3.8.2/tests/__init__.py
--rw-rw-rw-   0        0        0     2701 2018-07-03 20:23:03.000000 loutilities-3.8.2/tests/models.py
--rw-rw-rw-   0        0        0     6547 2018-07-04 09:49:12.000000 loutilities-3.8.2/tests/test_sqlalchemy_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.493832 loutilities-3.8.3/
+-rw-rw-rw-   0        0        0      483 2012-11-11 22:51:42.000000 loutilities-3.8.3/.gitattributes
+-rw-rw-rw-   0        0        0     1709 2020-09-24 11:16:31.000000 loutilities-3.8.3/.gitignore
+-rw-rw-rw-   0        0        0     2073 2023-05-28 11:12:27.486832 loutilities-3.8.3/PKG-INFO
+-rw-rw-rw-   0        0        0     1811 2020-05-28 21:02:31.000000 loutilities-3.8.3/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.105149 loutilities-3.8.3/loutilities/
+-rw-rw-rw-   0        0        0     1248 2013-01-15 19:29:28.000000 loutilities-3.8.3/loutilities/__init__.py
+-rw-rw-rw-   0        0        0    16727 2023-01-21 20:20:08.000000 loutilities-3.8.3/loutilities/agegrade.py
+-rw-rw-rw-   0        0        0     5767 2019-11-21 10:01:11.000000 loutilities-3.8.3/loutilities/apikey.py
+-rw-rw-rw-   0        0        0     5329 2021-12-03 11:20:03.000000 loutilities-3.8.3/loutilities/applytemplate.py
+-rw-rw-rw-   0        0        0    31804 2019-11-20 17:25:22.000000 loutilities-3.8.3/loutilities/bfile.py
+-rw-rw-rw-   0        0        0     1809 2019-11-20 17:48:38.000000 loutilities-3.8.3/loutilities/boolexpr.py
+-rw-rw-rw-   0        0        0     1597 2019-11-21 10:16:04.000000 loutilities-3.8.3/loutilities/config.py
+-rw-rw-rw-   0        0        0     1577 2019-11-25 21:48:03.000000 loutilities-3.8.3/loutilities/configparser.py
+-rw-rw-rw-   0        0        0     2726 2019-11-20 19:29:11.000000 loutilities-3.8.3/loutilities/csvu.py
+-rw-rw-rw-   0        0        0    16776 2021-12-02 12:11:45.000000 loutilities-3.8.3/loutilities/csvwt.py
+-rw-rw-rw-   0        0        0    10771 2019-11-25 21:46:41.000000 loutilities-3.8.3/loutilities/extconfigparser.py
+-rw-rw-rw-   0        0        0     8147 2019-11-25 21:48:03.000000 loutilities-3.8.3/loutilities/filetrigger.py
+-rw-rw-rw-   0        0        0     4592 2019-11-25 21:48:13.000000 loutilities-3.8.3/loutilities/filtercsv.py
+-rw-rw-rw-   0        0        0     3315 2022-12-05 19:41:06.000000 loutilities-3.8.3/loutilities/filters.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.166149 loutilities-3.8.3/loutilities/flask/
+-rw-rw-rw-   0        0        0       34 2021-02-23 18:59:56.000000 loutilities-3.8.3/loutilities/flask/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.173150 loutilities-3.8.3/loutilities/flask/user/
+-rw-rw-rw-   0        0        0       37 2021-02-23 18:59:56.000000 loutilities-3.8.3/loutilities/flask/user/__init__.py
+-rw-rw-rw-   0        0        0     4390 2021-03-01 13:08:41.000000 loutilities-3.8.3/loutilities/flask/user/views.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.199148 loutilities-3.8.3/loutilities/flask_helpers/
+-rw-rw-rw-   0        0        0        0 2018-07-18 20:55:43.000000 loutilities-3.8.3/loutilities/flask_helpers/__init__.py
+-rw-rw-rw-   0        0        0     1631 2019-11-20 17:25:25.000000 loutilities-3.8.3/loutilities/flask_helpers/as_blueprint.py
+-rw-rw-rw-   0        0        0     2976 2019-11-20 17:46:54.000000 loutilities-3.8.3/loutilities/flask_helpers/blueprints.py
+-rw-rw-rw-   0        0        0     2756 2020-07-14 16:48:05.000000 loutilities-3.8.3/loutilities/flask_helpers/decorators.py
+-rw-rw-rw-   0        0        0     2270 2023-05-10 10:01:07.000000 loutilities-3.8.3/loutilities/flask_helpers/mailer.py
+-rw-rw-rw-   0        0        0    10781 2017-12-24 09:46:57.000000 loutilities-3.8.3/loutilities/geo.py
+-rw-rw-rw-   0        0        0    12067 2022-04-02 22:20:21.000000 loutilities-3.8.3/loutilities/googleauth.py
+-rw-rw-rw-   0        0        0    10705 2019-11-27 11:58:53.000000 loutilities-3.8.3/loutilities/kmlutils.py
+-rw-rw-rw-   0        0        0     2448 2019-11-20 19:39:19.000000 loutilities-3.8.3/loutilities/makerst.py
+-rw-rw-rw-   0        0        0     8990 2019-11-20 17:25:23.000000 loutilities-3.8.3/loutilities/namesplitter.py
+-rw-rw-rw-   0        0        0     6267 2020-09-27 19:23:54.000000 loutilities-3.8.3/loutilities/nesteddict.py
+-rw-rw-rw-   0        0        0    22227 2020-05-27 10:57:20.000000 loutilities-3.8.3/loutilities/nicknames.csv
+-rw-rw-rw-   0        0        0     1557 2020-05-27 11:34:23.000000 loutilities-3.8.3/loutilities/nicknames.py
+-rw-rw-rw-   0        0        0     6266 2021-04-11 17:38:17.000000 loutilities-3.8.3/loutilities/renderrun.py
+-rw-rw-rw-   0        0        0     4057 2019-11-20 19:41:28.000000 loutilities-3.8.3/loutilities/sqlalchemy_helpers.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.207148 loutilities-3.8.3/loutilities/tables-assets/
+-rw-rw-rw-   0        0        0     1154 2019-06-27 16:58:21.000000 loutilities-3.8.3/loutilities/tables-assets/readme.md
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.361147 loutilities-3.8.3/loutilities/tables-assets/static/
+-rw-rw-rw-   0        0        0     7595 2021-05-27 19:24:36.000000 loutilities-3.8.3/loutilities/tables-assets/static/background-post-data-manager.js
+-rw-rw-rw-   0        0        0      168 2019-06-15 15:35:48.000000 loutilities-3.8.3/loutilities/tables-assets/static/branding.css
+-rw-rw-rw-   0        0        0      927 2017-12-06 20:12:04.000000 loutilities-3.8.3/loutilities/tables-assets/static/buttons.colvis.js
+-rw-rw-rw-   0        0        0      521 2019-05-12 00:41:26.000000 loutilities-3.8.3/loutilities/tables-assets/static/charts.css
+-rw-rw-rw-   0        0        0    19829 2022-04-15 19:49:44.000000 loutilities-3.8.3/loutilities/tables-assets/static/charts.js
+-rw-rw-rw-   0        0        0    30498 2021-04-05 11:19:07.000000 loutilities-3.8.3/loutilities/tables-assets/static/datatables-childrow.js
+-rw-rw-rw-   0        0        0     3581 2021-07-12 16:09:36.000000 loutilities-3.8.3/loutilities/tables-assets/static/datatables.css
+-rw-rw-rw-   0        0        0     1413 2020-04-03 11:12:13.000000 loutilities-3.8.3/loutilities/tables-assets/static/datatables.dataRender.datetime.js
+-rw-rw-rw-   0        0        0     1141 2019-07-16 17:38:55.000000 loutilities-3.8.3/loutilities/tables-assets/static/datatables.dataRender.ellipsis.js
+-rw-rw-rw-   0        0        0      700 2021-02-16 21:49:34.000000 loutilities-3.8.3/loutilities/tables-assets/static/datatables.dataRender.googledoc.js
+-rw-rw-rw-   0        0        0    22430 2021-07-16 21:09:07.000000 loutilities-3.8.3/loutilities/tables-assets/static/datatables.js
+-rw-rw-rw-   0        0        0     5340 2021-07-17 16:33:30.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor-saeditor.js
+-rw-rw-rw-   0        0        0     2329 2020-10-28 19:15:54.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor.buttons.editchildrowrefresh.js
+-rw-rw-rw-   0        0        0     1977 2020-08-03 13:49:06.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor.buttons.editrefresh.js
+-rw-rw-rw-   0        0        0      190 2021-03-30 19:14:25.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor.buttons.separator.js
+-rw-rw-rw-   0        0        0     3517 2020-07-01 18:34:03.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor.ckeditor5.js
+-rw-rw-rw-   0        0        0      185 2019-07-13 20:36:24.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor.css
+-rw-rw-rw-   0        0        0     2144 2020-07-13 11:15:00.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor.displayController.onPage.js
+-rw-rw-rw-   0        0        0     1265 2020-03-23 14:12:29.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor.fieldType.display.js
+-rw-rw-rw-   0        0        0     1757 2020-09-29 18:49:14.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor.googledoc.js
+-rw-rw-rw-   0        0        0     1993 2020-04-16 19:38:46.000000 loutilities-3.8.3/loutilities/tables-assets/static/editor.select2.mymethods.js
+-rw-rw-rw-   0        0        0     2088 2019-02-16 21:05:41.000000 loutilities-3.8.3/loutilities/tables-assets/static/eventscalendar.css
+-rw-rw-rw-   0        0        0      381 2019-06-30 18:16:58.000000 loutilities-3.8.3/loutilities/tables-assets/static/filters.css
+-rw-rw-rw-   0        0        0     3697 2020-04-07 18:55:39.000000 loutilities-3.8.3/loutilities/tables-assets/static/filters.js
+-rw-rw-rw-   0        0        0     2254 2017-12-11 10:45:42.000000 loutilities-3.8.3/loutilities/tables-assets/static/jquery.ui.dialog-clickoutside.js
+-rw-rw-rw-   0        0        0      331 2021-04-13 21:51:31.000000 loutilities-3.8.3/loutilities/tables-assets/static/jqueryui.theme.adjust.css
+-rw-rw-rw-   0        0        0      454 2018-12-15 20:43:56.000000 loutilities-3.8.3/loutilities/tables-assets/static/legend.js
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:26.878325 loutilities-3.8.3/loutilities/tables-assets/static/user/
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.371147 loutilities-3.8.3/loutilities/tables-assets/static/user/admin/
+-rw-rw-rw-   0        0        0      646 2022-05-09 20:13:08.000000 loutilities-3.8.3/loutilities/tables-assets/static/user/admin/beforedatatables.js
+-rw-rw-rw-   0        0        0     7208 2021-02-24 20:30:38.000000 loutilities-3.8.3/loutilities/tables-assets/static/user/admin/groups.js
+-rw-rw-rw-   0        0        0     4391 2021-07-16 21:09:23.000000 loutilities-3.8.3/loutilities/tables-assets/static/utils.js
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.402147 loutilities-3.8.3/loutilities/tables-assets/templates/
+-rw-rw-rw-   0        0        0       36 2019-12-09 22:56:02.000000 loutilities-3.8.3/loutilities/tables-assets/templates/bare-layout.jinja2
+-rw-rw-rw-   0        0        0      142 2019-06-14 14:56:28.000000 loutilities-3.8.3/loutilities/tables-assets/templates/datatables.html
+-rw-rw-rw-   0        0        0     3720 2020-06-25 18:51:11.000000 loutilities-3.8.3/loutilities/tables-assets/templates/datatables.jinja2
+-rw-rw-rw-   0        0        0     4243 2022-05-13 20:20:15.000000 loutilities-3.8.3/loutilities/tables-assets/templates/layout-base.jinja2
+-rw-rw-rw-   0        0        0      130 2019-06-14 14:55:29.000000 loutilities-3.8.3/loutilities/tables-assets/templates/layout.html
+-rw-rw-rw-   0        0        0      837 2019-06-21 21:28:23.000000 loutilities-3.8.3/loutilities/tables-assets/templates/layout.jinja2
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.415148 loutilities-3.8.3/loutilities/tables-assets/templates/security/
+-rw-rw-rw-   0        0        0      860 2022-09-25 00:43:58.000000 loutilities-3.8.3/loutilities/tables-assets/templates/security/change_password.jinja2
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.422146 loutilities-3.8.3/loutilities/tables-assets/templates/security/email/
+-rw-rw-rw-   0        0        0      514 2022-09-25 00:43:58.000000 loutilities-3.8.3/loutilities/tables-assets/templates/security/email/reset_instructions.html
+-rw-rw-rw-   0        0        0      454 2022-09-25 00:43:58.000000 loutilities-3.8.3/loutilities/tables-assets/templates/security/email/reset_instructions.txt
+-rw-rw-rw-   0        0        0      614 2022-09-25 00:43:58.000000 loutilities-3.8.3/loutilities/tables-assets/templates/security/forgot_password.jinja2
+-rw-rw-rw-   0        0        0     1601 2022-09-25 00:43:58.000000 loutilities-3.8.3/loutilities/tables-assets/templates/security/login_user.jinja2
+-rw-rw-rw-   0        0        0      698 2022-09-25 00:43:58.000000 loutilities-3.8.3/loutilities/tables-assets/templates/security/reset_password.jinja2
+-rw-rw-rw-   0        0        0     1455 2021-03-01 17:16:14.000000 loutilities-3.8.3/loutilities/tables-assets/templates/select-view.jinja2
+-rw-rw-rw-   0        0        0   150885 2023-01-04 19:40:01.000000 loutilities-3.8.3/loutilities/tables.py
+-rw-rw-rw-   0        0        0    20360 2021-12-03 18:46:39.000000 loutilities-3.8.3/loutilities/textreader.py
+-rw-rw-rw-   0        0        0     7657 2021-04-16 18:58:16.000000 loutilities-3.8.3/loutilities/timeu.py
+-rw-rw-rw-   0        0        0     2410 2021-03-12 20:12:30.000000 loutilities-3.8.3/loutilities/transform.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.451832 loutilities-3.8.3/loutilities/user/
+-rw-rw-rw-   0        0        0     4439 2023-05-04 16:45:05.000000 loutilities-3.8.3/loutilities/user/__init__.py
+-rw-rw-rw-   0        0        0     4261 2023-05-18 10:47:07.000000 loutilities-3.8.3/loutilities/user/applogging.py
+-rw-rw-rw-   0        0        0     1641 2020-03-12 20:37:30.000000 loutilities-3.8.3/loutilities/user/audit_mixin.py
+-rw-rw-rw-   0        0        0    13047 2023-05-21 18:49:15.000000 loutilities-3.8.3/loutilities/user/model.py
+-rw-rw-rw-   0        0        0     3194 2022-02-01 18:24:58.000000 loutilities-3.8.3/loutilities/user/roles.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.457830 loutilities-3.8.3/loutilities/user/scripts/
+-rw-rw-rw-   0        0        0        0 2020-01-02 18:24:31.000000 loutilities-3.8.3/loutilities/user/scripts/__init__.py
+-rw-rw-rw-   0        0        0     4768 2021-01-23 19:25:09.000000 loutilities-3.8.3/loutilities/user/scripts/users_init.py
+-rw-rw-rw-   0        0        0     2883 2020-03-06 21:27:20.000000 loutilities-3.8.3/loutilities/user/settings.py
+-rw-rw-rw-   0        0        0     8323 2020-05-02 15:41:47.000000 loutilities-3.8.3/loutilities/user/tablefiles.py
+-rw-rw-rw-   0        0        0    23503 2021-03-29 20:03:03.000000 loutilities-3.8.3/loutilities/user/tables.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.464838 loutilities-3.8.3/loutilities/user/views/
+-rw-rw-rw-   0        0        0      612 2020-03-06 10:51:08.000000 loutilities-3.8.3/loutilities/user/views/__init__.py
+-rw-rw-rw-   0        0        0    22778 2023-05-23 19:57:24.000000 loutilities-3.8.3/loutilities/user/views/userrole.py
+-rw-rw-rw-   0        0        0      110 2023-05-28 11:08:27.000000 loutilities-3.8.3/loutilities/version.py
+-rw-rw-rw-   0        0        0    13429 2019-11-27 20:15:01.000000 loutilities-3.8.3/loutilities/wxextensions.py
+-rw-rw-rw-   0        0        0     5040 2019-11-20 20:09:06.000000 loutilities-3.8.3/loutilities/xmldict.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.142145 loutilities-3.8.3/loutilities.egg-info/
+-rw-rw-rw-   0        0        0     2073 2023-05-28 11:12:23.000000 loutilities-3.8.3/loutilities.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     4270 2023-05-28 11:12:23.000000 loutilities-3.8.3/loutilities.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 11:12:23.000000 loutilities-3.8.3/loutilities.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0      210 2023-05-28 11:12:23.000000 loutilities-3.8.3/loutilities.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0        2 2018-12-17 13:25:37.000000 loutilities-3.8.3/loutilities.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       26 2023-05-28 11:12:23.000000 loutilities-3.8.3/loutilities.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       18 2023-05-28 11:12:23.000000 loutilities-3.8.3/loutilities.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 11:12:27.493832 loutilities-3.8.3/setup.cfg
+-rw-rw-rw-   0        0        0     2468 2022-10-05 20:49:08.000000 loutilities-3.8.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 11:12:27.482830 loutilities-3.8.3/tests/
+-rw-rw-rw-   0        0        0        0 2018-07-03 19:25:32.000000 loutilities-3.8.3/tests/__init__.py
+-rw-rw-rw-   0        0        0     2701 2018-07-03 20:23:03.000000 loutilities-3.8.3/tests/models.py
+-rw-rw-rw-   0        0        0     6547 2018-07-04 09:49:12.000000 loutilities-3.8.3/tests/test_sqlalchemy_helpers.py
```

### Comparing `loutilities-3.8.2/.gitignore` & `loutilities-3.8.3/.gitignore`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/PKG-INFO` & `loutilities-3.8.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loutilities
-Version: 3.8.2
+Version: 3.8.3
 Summary: some hopefully useful utilities
 Home-page: http://github.com/louking/loutilities
 Author: Lou King
 Author-email: lking@pobox.com
 License: Apache License, Version 2.0
 Platform: UNKNOWN
```

### Comparing `loutilities-3.8.2/README.md` & `loutilities-3.8.3/README.md`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/__init__.py` & `loutilities-3.8.3/loutilities/__init__.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/agegrade.py` & `loutilities-3.8.3/loutilities/agegrade.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/apikey.py` & `loutilities-3.8.3/loutilities/apikey.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/applytemplate.py` & `loutilities-3.8.3/loutilities/applytemplate.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/bfile.py` & `loutilities-3.8.3/loutilities/bfile.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/boolexpr.py` & `loutilities-3.8.3/loutilities/boolexpr.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/config.py` & `loutilities-3.8.3/loutilities/config.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/configparser.py` & `loutilities-3.8.3/loutilities/configparser.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/csvu.py` & `loutilities-3.8.3/loutilities/csvu.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/csvwt.py` & `loutilities-3.8.3/loutilities/csvwt.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/extconfigparser.py` & `loutilities-3.8.3/loutilities/extconfigparser.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/filetrigger.py` & `loutilities-3.8.3/loutilities/filetrigger.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/filtercsv.py` & `loutilities-3.8.3/loutilities/filtercsv.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/filters.py` & `loutilities-3.8.3/loutilities/filters.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/flask/user/views.py` & `loutilities-3.8.3/loutilities/flask/user/views.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/flask_helpers/as_blueprint.py` & `loutilities-3.8.3/loutilities/flask_helpers/as_blueprint.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/flask_helpers/blueprints.py` & `loutilities-3.8.3/loutilities/flask_helpers/blueprints.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/flask_helpers/decorators.py` & `loutilities-3.8.3/loutilities/flask_helpers/decorators.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/flask_helpers/mailer.py` & `loutilities-3.8.3/loutilities/flask_helpers/mailer.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/geo.py` & `loutilities-3.8.3/loutilities/geo.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/googleauth.py` & `loutilities-3.8.3/loutilities/googleauth.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/kmlutils.py` & `loutilities-3.8.3/loutilities/kmlutils.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/makerst.py` & `loutilities-3.8.3/loutilities/makerst.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/namesplitter.py` & `loutilities-3.8.3/loutilities/namesplitter.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/nesteddict.py` & `loutilities-3.8.3/loutilities/nesteddict.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/nicknames.csv` & `loutilities-3.8.3/loutilities/nicknames.csv`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/nicknames.py` & `loutilities-3.8.3/loutilities/nicknames.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/renderrun.py` & `loutilities-3.8.3/loutilities/renderrun.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/sqlalchemy_helpers.py` & `loutilities-3.8.3/loutilities/sqlalchemy_helpers.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/readme.md` & `loutilities-3.8.3/loutilities/tables-assets/readme.md`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/background-post-data-manager.js` & `loutilities-3.8.3/loutilities/tables-assets/static/background-post-data-manager.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/buttons.colvis.js` & `loutilities-3.8.3/loutilities/tables-assets/static/buttons.colvis.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/charts.css` & `loutilities-3.8.3/loutilities/tables-assets/static/charts.css`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/charts.js` & `loutilities-3.8.3/loutilities/tables-assets/static/charts.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/datatables-childrow.js` & `loutilities-3.8.3/loutilities/tables-assets/static/datatables-childrow.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/datatables.css` & `loutilities-3.8.3/loutilities/tables-assets/static/datatables.css`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/datatables.dataRender.datetime.js` & `loutilities-3.8.3/loutilities/tables-assets/static/datatables.dataRender.datetime.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/datatables.dataRender.ellipsis.js` & `loutilities-3.8.3/loutilities/tables-assets/static/datatables.dataRender.ellipsis.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/datatables.dataRender.googledoc.js` & `loutilities-3.8.3/loutilities/tables-assets/static/datatables.dataRender.googledoc.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/datatables.js` & `loutilities-3.8.3/loutilities/tables-assets/static/datatables.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/editor-saeditor.js` & `loutilities-3.8.3/loutilities/tables-assets/static/editor-saeditor.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/editor.buttons.editchildrowrefresh.js` & `loutilities-3.8.3/loutilities/tables-assets/static/editor.buttons.editchildrowrefresh.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/editor.buttons.editrefresh.js` & `loutilities-3.8.3/loutilities/tables-assets/static/editor.buttons.editrefresh.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/editor.ckeditor5.js` & `loutilities-3.8.3/loutilities/tables-assets/static/editor.ckeditor5.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/editor.displayController.onPage.js` & `loutilities-3.8.3/loutilities/tables-assets/static/editor.displayController.onPage.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/editor.fieldType.display.js` & `loutilities-3.8.3/loutilities/tables-assets/static/editor.fieldType.display.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/editor.googledoc.js` & `loutilities-3.8.3/loutilities/tables-assets/static/editor.googledoc.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/editor.select2.mymethods.js` & `loutilities-3.8.3/loutilities/tables-assets/static/editor.select2.mymethods.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/eventscalendar.css` & `loutilities-3.8.3/loutilities/tables-assets/static/eventscalendar.css`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/filters.js` & `loutilities-3.8.3/loutilities/tables-assets/static/filters.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/jquery.ui.dialog-clickoutside.js` & `loutilities-3.8.3/loutilities/tables-assets/static/jquery.ui.dialog-clickoutside.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/user/admin/beforedatatables.js` & `loutilities-3.8.3/loutilities/tables-assets/static/user/admin/beforedatatables.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/user/admin/groups.js` & `loutilities-3.8.3/loutilities/tables-assets/static/user/admin/groups.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/static/utils.js` & `loutilities-3.8.3/loutilities/tables-assets/static/utils.js`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/templates/datatables.jinja2` & `loutilities-3.8.3/loutilities/tables-assets/templates/datatables.jinja2`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/templates/layout-base.jinja2` & `loutilities-3.8.3/loutilities/tables-assets/templates/layout-base.jinja2`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/templates/layout.jinja2` & `loutilities-3.8.3/loutilities/tables-assets/templates/layout.jinja2`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/templates/security/change_password.jinja2` & `loutilities-3.8.3/loutilities/tables-assets/templates/security/change_password.jinja2`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/templates/security/email/reset_instructions.html` & `loutilities-3.8.3/loutilities/tables-assets/templates/security/email/reset_instructions.html`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/templates/security/forgot_password.jinja2` & `loutilities-3.8.3/loutilities/tables-assets/templates/security/forgot_password.jinja2`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/templates/security/login_user.jinja2` & `loutilities-3.8.3/loutilities/tables-assets/templates/security/login_user.jinja2`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/templates/security/reset_password.jinja2` & `loutilities-3.8.3/loutilities/tables-assets/templates/security/reset_password.jinja2`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables-assets/templates/select-view.jinja2` & `loutilities-3.8.3/loutilities/tables-assets/templates/select-view.jinja2`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/tables.py` & `loutilities-3.8.3/loutilities/tables.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/textreader.py` & `loutilities-3.8.3/loutilities/textreader.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/timeu.py` & `loutilities-3.8.3/loutilities/timeu.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/transform.py` & `loutilities-3.8.3/loutilities/transform.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/user/__init__.py` & `loutilities-3.8.3/loutilities/user/__init__.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/user/applogging.py` & `loutilities-3.8.3/loutilities/user/applogging.py`

 * *Files 12% similar despite different names*

```diff
@@ -38,28 +38,32 @@
     # *** for some reason the following code caused debug pin not to be shown, see https://github.com/louking/rrwebapp/issues/300
     # werkzeug_logger = logging.getLogger('werkzeug')
     # werkzeug_logger.setLevel(logging.INFO)
 
     # set up logging
     ADMINS = current_app.config['EXCEPTION_EMAIL']
     application = current_app.config['APP_LOUTILITY']
+    
+    # support backwards compatibility
+    fromaddr = current_app.config['EXCEPTION_EMAIL_SENDER'] if 'EXCEPTION_EMAIL_SENDER' in current_app.config else 'noreply@steeplechasers.org'
+    
     # to test, set if to True, and change run environment to production
     # if True:
     if not current_app.debug:
         if 'MAIL_SERVER' in current_app.config and 'MAIL_PORT' in current_app.config:
             mailhost = (current_app.config['MAIL_SERVER'], current_app.config['MAIL_PORT'])
         elif 'MAIL_SERVER' in current_app.config:
             mailhost = current_app.config['MAIL_SERVER']
         else:
             mailhost = 'localhost'
         credentials = None
         if 'MAIL_USERNAME' in current_app.config and 'MAIL_PASSWORD' in current_app.config:
             credentials = (current_app.config['MAIL_USERNAME'], current_app.config['MAIL_PASSWORD'])
         mail_handler = SMTPHandler(mailhost,
-                                   'noreply@steeplechasers.org',
+                                   fromaddr,
                                    ADMINS, f'{application} exception encountered',
                                    credentials = credentials)
         if 'LOGGING_LEVEL_MAIL' in current_app.config:
             mailloglevel = current_app.config['LOGGING_LEVEL_MAIL']
         else:
             mailloglevel = logging.ERROR
         mail_handler.setLevel(mailloglevel)
```

### Comparing `loutilities-3.8.2/loutilities/user/audit_mixin.py` & `loutilities-3.8.3/loutilities/user/audit_mixin.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/user/model.py` & `loutilities-3.8.3/loutilities/user/model.py`

 * *Files 5% similar despite different names*

```diff
@@ -198,15 +198,18 @@
         # don't try to update before table exists
         if not db.engine.has_table(self.localusertable): return
 
         # alllocal will be used to determine what localuser model rows need to be deactivated
         # this detects deletions in User table
 
         alllocal = {}
-        for localuser in self.localusermodel.query.all():
+        # only worry about active entries. corner case exists where interest is deleted, and leaves an
+        # active=False entry with interest_id=None. For that case, later query by user_id, interest_id returns
+        # more than one row, and causes exception. See louking/webmodules#44
+        for localuser in self.localusermodel.query.filter_by(active=True).all():
             alllocal[localuser.user_id, localuser.interest_id] = localuser
 
         for user in User.query.all():
             for interest in Interest.query.all():
                 # if this interest isn't for this application, ignore
                 if self.application not in interest.applications: continue
```

### Comparing `loutilities-3.8.2/loutilities/user/roles.py` & `loutilities-3.8.3/loutilities/user/roles.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/user/scripts/users_init.py` & `loutilities-3.8.3/loutilities/user/scripts/users_init.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/user/settings.py` & `loutilities-3.8.3/loutilities/user/settings.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/user/tablefiles.py` & `loutilities-3.8.3/loutilities/user/tablefiles.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/user/tables.py` & `loutilities-3.8.3/loutilities/user/tables.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/user/views/__init__.py` & `loutilities-3.8.3/loutilities/user/views/__init__.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/user/views/userrole.py` & `loutilities-3.8.3/loutilities/user/views/userrole.py`

 * *Files 0% similar despite different names*

```diff
@@ -409,15 +409,15 @@
         '''
         self.kwargs = kwargs
         args = dict(
             app=bp,  # use blueprint instead of app
             db=db,
             model=Interest,
             version_id_col='version_id',  # optimistic concurrency control
-            interests_accepted=ROLE_SUPER_ADMIN,
+            roles_accepted=ROLE_SUPER_ADMIN,
             template='datatables.jinja2',
             pagename='interests',
             endpoint='userrole.interests',
             rule='/interests',
             dbmapping=interest_dbmapping,
             formmapping=interest_formmapping,
             clientcolumns=[
@@ -475,15 +475,15 @@
     return results
 
 application_view = DbCrudApiRolePermissions(
                     app = bp,   # use blueprint instead of app
                     db = db,
                     model = Application,
                     version_id_col = 'version_id',  # optimistic concurrency control
-                    applications_accepted = ROLE_SUPER_ADMIN,
+                    roles_accepted = ROLE_SUPER_ADMIN,
                     template = 'datatables.jinja2',
                     pagename = 'applications', 
                     endpoint = 'userrole.applications',
                     rule = '/applications',
                     dbmapping = application_dbmapping, 
                     formmapping = application_formmapping, 
                     clientcolumns = [
```

### Comparing `loutilities-3.8.2/loutilities/wxextensions.py` & `loutilities-3.8.3/loutilities/wxextensions.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities/xmldict.py` & `loutilities-3.8.3/loutilities/xmldict.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/loutilities.egg-info/PKG-INFO` & `loutilities-3.8.3/loutilities.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: loutilities
-Version: 3.8.2
+Version: 3.8.3
 Summary: some hopefully useful utilities
 Home-page: http://github.com/louking/loutilities
 Author: Lou King
 Author-email: lking@pobox.com
 License: Apache License, Version 2.0
 Platform: UNKNOWN
```

### Comparing `loutilities-3.8.2/loutilities.egg-info/SOURCES.txt` & `loutilities-3.8.3/loutilities.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/setup.py` & `loutilities-3.8.3/setup.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/tests/models.py` & `loutilities-3.8.3/tests/models.py`

 * *Files identical despite different names*

### Comparing `loutilities-3.8.2/tests/test_sqlalchemy_helpers.py` & `loutilities-3.8.3/tests/test_sqlalchemy_helpers.py`

 * *Files identical despite different names*

