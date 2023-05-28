# Comparing `tmp/django-adminfilters-2.1.0.tar.gz` & `tmp/django-adminfilters-2.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-adminfilters-2.1.0.tar", last modified: Thu Mar 23 18:49:59 2023, max compression
+gzip compressed data, was "django-adminfilters-2.2.0.tar", last modified: Sun May 28 18:40:55 2023, max compression
```

## Comparing `django-adminfilters-2.1.0.tar` & `django-adminfilters-2.2.0.tar`

### file list

```diff
@@ -1,136 +1,137 @@
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.582408 django-adminfilters-2.1.0/
--rw-r--r--   0 sax        (501) staff       (20)      154 2016-01-01 21:03:36.000000 django-adminfilters-2.1.0/AUTHORS
--rw-r--r--   0 sax        (501) staff       (20)     2734 2023-03-23 18:04:52.000000 django-adminfilters-2.1.0/CHANGES.md
--rw-r--r--   0 sax        (501) staff       (20)     1163 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/LICENSE
--rw-r--r--   0 sax        (501) staff       (20)      589 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/MANIFEST.in
--rw-r--r--   0 sax        (501) staff       (20)     3947 2023-03-23 18:49:59.582539 django-adminfilters-2.1.0/PKG-INFO
--rw-r--r--   0 sax        (501) staff       (20)     3045 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/README.md
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.551904 django-adminfilters-2.1.0/docs/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.552673 django-adminfilters-2.1.0/docs/_ext/
--rw-r--r--   0 sax        (501) staff       (20)     7072 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/docs/_ext/djangodocs.py
--rw-r--r--   0 sax        (501) staff       (20)     5231 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/docs/_ext/github.py
--rw-r--r--   0 sax        (501) staff       (20)     2281 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/docs/_ext/version.py
--rw-r--r--   0 sax        (501) staff       (20)     8650 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/docs/conf.py
--rw-r--r--   0 sax        (501) staff       (20)      660 2023-03-23 18:49:59.583177 django-adminfilters-2.1.0/setup.cfg
--rwxr-xr-x   0 sax        (501) staff       (20)     1999 2022-03-04 11:26:00.000000 django-adminfilters-2.1.0/setup.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.547881 django-adminfilters-2.1.0/src/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.557913 django-adminfilters-2.1.0/src/adminfilters/
--rw-r--r--   0 sax        (501) staff       (20)       80 2023-03-23 18:01:33.000000 django-adminfilters-2.1.0/src/adminfilters/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)      146 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/apps.py
--rw-r--r--   0 sax        (501) staff       (20)     3289 2023-03-23 17:16:51.000000 django-adminfilters-2.1.0/src/adminfilters/autocomplete.py
--rw-r--r--   0 sax        (501) staff       (20)     3316 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/checkbox.py
--rw-r--r--   0 sax        (501) staff       (20)     1221 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/checks.py
--rw-r--r--   0 sax        (501) staff       (20)      582 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/combo.py
--rw-r--r--   0 sax        (501) staff       (20)     2364 2023-03-23 17:14:09.000000 django-adminfilters-2.1.0/src/adminfilters/dates.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.559754 django-adminfilters-2.1.0/src/adminfilters/depot/
--rw-r--r--   0 sax        (501) staff       (20)        0 2023-03-23 18:01:33.000000 django-adminfilters-2.1.0/src/adminfilters/depot/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)      412 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/depot/admin.py
--rw-r--r--   0 sax        (501) staff       (20)       93 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/depot/apps.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.560551 django-adminfilters-2.1.0/src/adminfilters/depot/migrations/
--rw-r--r--   0 sax        (501) staff       (20)     1020 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/depot/migrations/0001_initial.py
--rw-r--r--   0 sax        (501) staff       (20)      564 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/src/adminfilters/depot/migrations/0002_migration.py
--rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/depot/migrations/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)      550 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/depot/models.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.546477 django-adminfilters-2.1.0/src/adminfilters/depot/templates/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.560764 django-adminfilters-2.1.0/src/adminfilters/depot/templates/adminfilters/
--rw-r--r--   0 sax        (501) staff       (20)     2063 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/depot/templates/adminfilters/widget.html
--rw-r--r--   0 sax        (501) staff       (20)     3465 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/depot/widget.py
--rw-r--r--   0 sax        (501) staff       (20)     3849 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/src/adminfilters/dj.py
--rw-r--r--   0 sax        (501) staff       (20)      944 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/extra.py
--rw-r--r--   0 sax        (501) staff       (20)      666 2022-11-22 04:49:29.000000 django-adminfilters-2.1.0/src/adminfilters/filters.py
--rw-r--r--   0 sax        (501) staff       (20)     3901 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/json.py
--rw-r--r--   0 sax        (501) staff       (20)     2283 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/mixin.py
--rw-r--r--   0 sax        (501) staff       (20)     4205 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/src/adminfilters/multiselect.py
--rw-r--r--   0 sax        (501) staff       (20)     3345 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/src/adminfilters/numbers.py
--rw-r--r--   0 sax        (501) staff       (20)     4334 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/src/adminfilters/querystring.py
--rw-r--r--   0 sax        (501) staff       (20)      747 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/radio.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.546794 django-adminfilters-2.1.0/src/adminfilters/static/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.564283 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/
--rw-r--r--   0 sax        (501) staff       (20)     8980 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/adminfilters.css
--rw-r--r--   0 sax        (501) staff       (20)      445 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/autocomplete.js
--rw-r--r--   0 sax        (501) staff       (20)      285 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/autocomplete.min.js
--rw-r--r--   0 sax        (501) staff       (20)     1483 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/depot.js
--rw-r--r--   0 sax        (501) staff       (20)     1058 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/depot.min.js
--rw-r--r--   0 sax        (501) staff       (20)     2499 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/dj.js
--rw-r--r--   0 sax        (501) staff       (20)     1817 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/dj.min.js
--rw-r--r--   0 sax        (501) staff       (20)     3316 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/jsonfilter.js
--rw-r--r--   0 sax        (501) staff       (20)     2433 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/jsonfilter.min.js
--rw-r--r--   0 sax        (501) staff       (20)     2329 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/querystring.js
--rw-r--r--   0 sax        (501) staff       (20)     1693 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/querystring.min.js
--rw-r--r--   0 sax        (501) staff       (20)     2565 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/value.js
--rw-r--r--   0 sax        (501) staff       (20)     1872 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/value.min.js
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.547332 django-adminfilters-2.1.0/src/adminfilters/templates/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.567619 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/
--rw-r--r--   0 sax        (501) staff       (20)      176 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/_attrs.html
--rw-r--r--   0 sax        (501) staff       (20)      428 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/_wrapper.html
--rw-r--r--   0 sax        (501) staff       (20)     1104 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/autocomplete.html
--rw-r--r--   0 sax        (501) staff       (20)     2306 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/checkbox.html
--rw-r--r--   0 sax        (501) staff       (20)      468 2018-08-16 14:14:55.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/combobox.html
--rw-r--r--   0 sax        (501) staff       (20)     2470 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/dj.html
--rw-r--r--   0 sax        (501) staff       (20)     3669 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/json.html
--rw-r--r--   0 sax        (501) staff       (20)     1639 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/querystring.html
--rw-r--r--   0 sax        (501) staff       (20)      525 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/radio.html
--rw-r--r--   0 sax        (501) staff       (20)     1741 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/value.html
--rw-r--r--   0 sax        (501) staff       (20)     1717 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/value_multi.html
--rw-r--r--   0 sax        (501) staff       (20)     4057 2023-02-28 13:36:49.000000 django-adminfilters-2.1.0/src/adminfilters/utils.py
--rw-r--r--   0 sax        (501) staff       (20)     5015 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/src/adminfilters/value.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.570115 django-adminfilters-2.1.0/src/django_adminfilters.egg-info/
--rw-r--r--   0 sax        (501) staff       (20)     3947 2023-03-23 18:49:59.000000 django-adminfilters-2.1.0/src/django_adminfilters.egg-info/PKG-INFO
--rw-r--r--   0 sax        (501) staff       (20)     3763 2023-03-23 18:49:59.000000 django-adminfilters-2.1.0/src/django_adminfilters.egg-info/SOURCES.txt
--rw-r--r--   0 sax        (501) staff       (20)        1 2023-03-23 18:49:59.000000 django-adminfilters-2.1.0/src/django_adminfilters.egg-info/dependency_links.txt
--rw-r--r--   0 sax        (501) staff       (20)      384 2023-03-23 18:49:59.000000 django-adminfilters-2.1.0/src/django_adminfilters.egg-info/requires.txt
--rw-r--r--   0 sax        (501) staff       (20)       13 2023-03-23 18:49:59.000000 django-adminfilters-2.1.0/src/django_adminfilters.egg-info/top_level.txt
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.571061 django-adminfilters-2.1.0/src/requirements/
--rw-r--r--   0 sax        (501) staff       (20)       86 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/requirements/develop.pip
--rw-r--r--   0 sax        (501) staff       (20)        0 2018-02-21 17:01:55.000000 django-adminfilters-2.1.0/src/requirements/install.pip
--rw-r--r--   0 sax        (501) staff       (20)      159 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/src/requirements/testing.pip
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.575161 django-adminfilters-2.1.0/tests/
--rw-r--r--   0 sax        (501) staff       (20)      648 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/.coveragerc
--rw-r--r--   0 sax        (501) staff       (20)     1065 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/conftest.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.575422 django-adminfilters-2.1.0/tests/demoapp/
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.578458 django-adminfilters-2.1.0/tests/demoapp/demo/
--rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)     3793 2022-11-22 07:53:27.000000 django-adminfilters-2.1.0/tests/demoapp/demo/admin.py
--rw-r--r--   0 sax        (501) staff       (20)     1207 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/backends.py
--rw-r--r--   0 sax        (501) staff       (20)     3231 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/factories.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.578753 django-adminfilters-2.1.0/tests/demoapp/demo/management/
--rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/management/__init__.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.579177 django-adminfilters-2.1.0/tests/demoapp/demo/management/commands/
--rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/management/commands/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)     3372 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/management/commands/init_demo.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.579722 django-adminfilters-2.1.0/tests/demoapp/demo/migrations/
--rw-r--r--   0 sax        (501) staff       (20)     4921 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/migrations/0001_initial.py
--rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/migrations/__init__.py
--rw-r--r--   0 sax        (501) staff       (20)     3614 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/models.py
--rw-r--r--   0 sax        (501) staff       (20)     2759 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/settings.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.579925 django-adminfilters-2.1.0/tests/demoapp/demo/static/
--rw-r--r--   0 sax        (501) staff       (20)     1150 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/static/favicon.ico
--rw-r--r--   0 sax        (501) staff       (20)     1703 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/urls.py
--rw-r--r--   0 sax        (501) staff       (20)     6969 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/utils.py
--rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/views.py
--rw-r--r--   0 sax        (501) staff       (20)     1131 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/demo/wsgi.py
--rwxr-xr-x   0 sax        (501) staff       (20)      331 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/demoapp/manage.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.580453 django-adminfilters-2.1.0/tests/depot/
--rw-r--r--   0 sax        (501) staff       (20)      121 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/depot/test_models.py
--rw-r--r--   0 sax        (501) staff       (20)     1833 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/depot/test_widget.py
-drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-03-23 18:49:59.582189 django-adminfilters-2.1.0/tests/functional/
--rw-r--r--   0 sax        (501) staff       (20)     3310 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/functional/conftest.py
--rw-r--r--   0 sax        (501) staff       (20)      934 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/functional/test_f_automplete.py
--rw-r--r--   0 sax        (501) staff       (20)     1846 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/functional/test_f_depot.py
--rw-r--r--   0 sax        (501) staff       (20)     1708 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/functional/test_f_lookup.py
--rw-r--r--   0 sax        (501) staff       (20)     1476 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/functional/test_f_number.py
--rw-r--r--   0 sax        (501) staff       (20)     2773 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/functional/test_f_querystring.py
--rw-r--r--   0 sax        (501) staff       (20)     1980 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/functional/test_f_value.py
--rw-r--r--   0 sax        (501) staff       (20)      912 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_automplete.py
--rw-r--r--   0 sax        (501) staff       (20)     1859 2023-03-23 17:14:09.000000 django-adminfilters-2.1.0/tests/test_dates.py
--rw-r--r--   0 sax        (501) staff       (20)     1633 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_dj.py
--rw-r--r--   0 sax        (501) staff       (20)     1048 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_django_check.py
--rw-r--r--   0 sax        (501) staff       (20)      815 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_extra.py
--rw-r--r--   0 sax        (501) staff       (20)     3571 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_json.py
--rw-r--r--   0 sax        (501) staff       (20)     3021 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_multiselect.py
--rw-r--r--   0 sax        (501) staff       (20)     1449 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_number.py
--rw-r--r--   0 sax        (501) staff       (20)     1594 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_querystring.py
--rw-r--r--   0 sax        (501) staff       (20)     2203 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_related.py
--rw-r--r--   0 sax        (501) staff       (20)      823 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_utils.py
--rw-r--r--   0 sax        (501) staff       (20)     2152 2022-02-22 22:03:36.000000 django-adminfilters-2.1.0/tests/test_value.py
--rw-r--r--   0 sax        (501) staff       (20)     1281 2023-03-23 18:49:36.000000 django-adminfilters-2.1.0/tox.ini
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.468931 django-adminfilters-2.2.0/
+-rw-r--r--   0 sax        (501) staff       (20)      154 2016-01-01 21:03:36.000000 django-adminfilters-2.2.0/AUTHORS
+-rw-r--r--   0 sax        (501) staff       (20)     2840 2023-05-26 18:02:19.000000 django-adminfilters-2.2.0/CHANGES.md
+-rw-r--r--   0 sax        (501) staff       (20)     1163 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/LICENSE
+-rw-r--r--   0 sax        (501) staff       (20)      589 2022-11-22 07:53:27.000000 django-adminfilters-2.2.0/MANIFEST.in
+-rw-r--r--   0 sax        (501) staff       (20)     3975 2023-05-28 18:40:55.469061 django-adminfilters-2.2.0/PKG-INFO
+-rw-r--r--   0 sax        (501) staff       (20)     3073 2023-05-26 18:02:19.000000 django-adminfilters-2.2.0/README.md
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.428574 django-adminfilters-2.2.0/docs/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.429572 django-adminfilters-2.2.0/docs/_ext/
+-rw-r--r--   0 sax        (501) staff       (20)     7174 2023-05-28 18:01:51.000000 django-adminfilters-2.2.0/docs/_ext/djangodocs.py
+-rw-r--r--   0 sax        (501) staff       (20)     5294 2023-05-28 10:15:26.000000 django-adminfilters-2.2.0/docs/_ext/github.py
+-rw-r--r--   0 sax        (501) staff       (20)     2278 2023-05-28 10:15:26.000000 django-adminfilters-2.2.0/docs/_ext/version.py
+-rw-r--r--   0 sax        (501) staff       (20)     8609 2023-05-28 10:15:26.000000 django-adminfilters-2.2.0/docs/conf.py
+-rw-r--r--   0 sax        (501) staff       (20)      201 2023-05-28 18:40:55.469743 django-adminfilters-2.2.0/setup.cfg
+-rwxr-xr-x   0 sax        (501) staff       (20)     1924 2023-05-28 10:15:26.000000 django-adminfilters-2.2.0/setup.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.423009 django-adminfilters-2.2.0/src/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.435092 django-adminfilters-2.2.0/src/adminfilters/
+-rw-r--r--   0 sax        (501) staff       (20)       80 2023-05-28 18:39:44.000000 django-adminfilters-2.2.0/src/adminfilters/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)      146 2023-05-28 10:29:27.000000 django-adminfilters-2.2.0/src/adminfilters/apps.py
+-rw-r--r--   0 sax        (501) staff       (20)     3369 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/autocomplete.py
+-rw-r--r--   0 sax        (501) staff       (20)     3511 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/checkbox.py
+-rw-r--r--   0 sax        (501) staff       (20)     1372 2023-05-28 10:02:11.000000 django-adminfilters-2.2.0/src/adminfilters/checks.py
+-rw-r--r--   0 sax        (501) staff       (20)      495 2023-05-28 17:58:22.000000 django-adminfilters-2.2.0/src/adminfilters/combo.py
+-rw-r--r--   0 sax        (501) staff       (20)     2328 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/dates.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.436738 django-adminfilters-2.2.0/src/adminfilters/depot/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2023-03-23 18:50:50.000000 django-adminfilters-2.2.0/src/adminfilters/depot/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)      414 2023-05-28 10:29:27.000000 django-adminfilters-2.2.0/src/adminfilters/depot/admin.py
+-rw-r--r--   0 sax        (501) staff       (20)       93 2023-05-28 10:29:27.000000 django-adminfilters-2.2.0/src/adminfilters/depot/apps.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.438396 django-adminfilters-2.2.0/src/adminfilters/depot/migrations/
+-rw-r--r--   0 sax        (501) staff       (20)     1457 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/depot/migrations/0001_initial.py
+-rw-r--r--   0 sax        (501) staff       (20)      593 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/depot/migrations/0002_migration.py
+-rw-r--r--   0 sax        (501) staff       (20)      464 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/depot/migrations/0003_alter_storedfilter_id.py
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/depot/migrations/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)      550 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/depot/models.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.422145 django-adminfilters-2.2.0/src/adminfilters/depot/templates/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.438720 django-adminfilters-2.2.0/src/adminfilters/depot/templates/adminfilters/
+-rw-r--r--   0 sax        (501) staff       (20)     2063 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/depot/templates/adminfilters/widget.html
+-rw-r--r--   0 sax        (501) staff       (20)     3388 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/depot/widget.py
+-rw-r--r--   0 sax        (501) staff       (20)     3952 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/dj.py
+-rw-r--r--   0 sax        (501) staff       (20)      927 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/extra.py
+-rw-r--r--   0 sax        (501) staff       (20)      620 2023-05-28 17:58:22.000000 django-adminfilters-2.2.0/src/adminfilters/filters.py
+-rw-r--r--   0 sax        (501) staff       (20)     4056 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/json.py
+-rw-r--r--   0 sax        (501) staff       (20)     2361 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/mixin.py
+-rw-r--r--   0 sax        (501) staff       (20)     4097 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/multiselect.py
+-rw-r--r--   0 sax        (501) staff       (20)     3384 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/numbers.py
+-rw-r--r--   0 sax        (501) staff       (20)     4715 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/querystring.py
+-rw-r--r--   0 sax        (501) staff       (20)      639 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/radio.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.422421 django-adminfilters-2.2.0/src/adminfilters/static/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.444037 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/
+-rw-r--r--   0 sax        (501) staff       (20)     8980 2022-11-22 07:53:27.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/adminfilters.css
+-rw-r--r--   0 sax        (501) staff       (20)      445 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/autocomplete.js
+-rw-r--r--   0 sax        (501) staff       (20)      285 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/autocomplete.min.js
+-rw-r--r--   0 sax        (501) staff       (20)     1483 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/depot.js
+-rw-r--r--   0 sax        (501) staff       (20)     1058 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/depot.min.js
+-rw-r--r--   0 sax        (501) staff       (20)     2499 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/dj.js
+-rw-r--r--   0 sax        (501) staff       (20)     1817 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/dj.min.js
+-rw-r--r--   0 sax        (501) staff       (20)     3316 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/jsonfilter.js
+-rw-r--r--   0 sax        (501) staff       (20)     2433 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/jsonfilter.min.js
+-rw-r--r--   0 sax        (501) staff       (20)     2329 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/querystring.js
+-rw-r--r--   0 sax        (501) staff       (20)     1693 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/querystring.min.js
+-rw-r--r--   0 sax        (501) staff       (20)     2565 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/value.js
+-rw-r--r--   0 sax        (501) staff       (20)     1872 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/value.min.js
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.422692 django-adminfilters-2.2.0/src/adminfilters/templates/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.449740 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/
+-rw-r--r--   0 sax        (501) staff       (20)      176 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/_attrs.html
+-rw-r--r--   0 sax        (501) staff       (20)      428 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/_wrapper.html
+-rw-r--r--   0 sax        (501) staff       (20)     1104 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/autocomplete.html
+-rw-r--r--   0 sax        (501) staff       (20)     2306 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/checkbox.html
+-rw-r--r--   0 sax        (501) staff       (20)      468 2018-08-16 14:14:55.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/combobox.html
+-rw-r--r--   0 sax        (501) staff       (20)     2470 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/dj.html
+-rw-r--r--   0 sax        (501) staff       (20)     3669 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/json.html
+-rw-r--r--   0 sax        (501) staff       (20)     1639 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/querystring.html
+-rw-r--r--   0 sax        (501) staff       (20)      525 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/radio.html
+-rw-r--r--   0 sax        (501) staff       (20)     1741 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/value.html
+-rw-r--r--   0 sax        (501) staff       (20)     1717 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/value_multi.html
+-rw-r--r--   0 sax        (501) staff       (20)     4268 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/utils.py
+-rw-r--r--   0 sax        (501) staff       (20)     4970 2023-05-28 10:29:28.000000 django-adminfilters-2.2.0/src/adminfilters/value.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.451864 django-adminfilters-2.2.0/src/django_adminfilters.egg-info/
+-rw-r--r--   0 sax        (501) staff       (20)     3975 2023-05-28 18:40:55.000000 django-adminfilters-2.2.0/src/django_adminfilters.egg-info/PKG-INFO
+-rw-r--r--   0 sax        (501) staff       (20)     3827 2023-05-28 18:40:55.000000 django-adminfilters-2.2.0/src/django_adminfilters.egg-info/SOURCES.txt
+-rw-r--r--   0 sax        (501) staff       (20)        1 2023-05-28 18:40:55.000000 django-adminfilters-2.2.0/src/django_adminfilters.egg-info/dependency_links.txt
+-rw-r--r--   0 sax        (501) staff       (20)      401 2023-05-28 18:40:55.000000 django-adminfilters-2.2.0/src/django_adminfilters.egg-info/requires.txt
+-rw-r--r--   0 sax        (501) staff       (20)       13 2023-05-28 18:40:55.000000 django-adminfilters-2.2.0/src/django_adminfilters.egg-info/top_level.txt
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.453275 django-adminfilters-2.2.0/src/requirements/
+-rw-r--r--   0 sax        (501) staff       (20)       97 2023-05-28 17:46:45.000000 django-adminfilters-2.2.0/src/requirements/develop.pip
+-rw-r--r--   0 sax        (501) staff       (20)        0 2018-02-21 17:01:55.000000 django-adminfilters-2.2.0/src/requirements/install.pip
+-rw-r--r--   0 sax        (501) staff       (20)      159 2023-05-26 19:11:22.000000 django-adminfilters-2.2.0/src/requirements/testing.pip
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.459691 django-adminfilters-2.2.0/tests/
+-rw-r--r--   0 sax        (501) staff       (20)      648 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/tests/.coveragerc
+-rw-r--r--   0 sax        (501) staff       (20)     1162 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/conftest.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.460032 django-adminfilters-2.2.0/tests/demoapp/
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.463647 django-adminfilters-2.2.0/tests/demoapp/demo/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/tests/demoapp/demo/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)     3615 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/admin.py
+-rw-r--r--   0 sax        (501) staff       (20)     1308 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/backends.py
+-rw-r--r--   0 sax        (501) staff       (20)     3343 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/factories.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.463984 django-adminfilters-2.2.0/tests/demoapp/demo/management/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/tests/demoapp/demo/management/__init__.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.464505 django-adminfilters-2.2.0/tests/demoapp/demo/management/commands/
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/tests/demoapp/demo/management/commands/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)     3212 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/management/commands/init_demo.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.465209 django-adminfilters-2.2.0/tests/demoapp/demo/migrations/
+-rw-r--r--   0 sax        (501) staff       (20)     6169 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/migrations/0001_initial.py
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/tests/demoapp/demo/migrations/__init__.py
+-rw-r--r--   0 sax        (501) staff       (20)     3386 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/models.py
+-rw-r--r--   0 sax        (501) staff       (20)     2807 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/settings.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.465469 django-adminfilters-2.2.0/tests/demoapp/demo/static/
+-rw-r--r--   0 sax        (501) staff       (20)     1150 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/tests/demoapp/demo/static/favicon.ico
+-rw-r--r--   0 sax        (501) staff       (20)     1714 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/urls.py
+-rw-r--r--   0 sax        (501) staff       (20)     7109 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/utils.py
+-rw-r--r--   0 sax        (501) staff       (20)        0 2022-02-22 22:03:36.000000 django-adminfilters-2.2.0/tests/demoapp/demo/views.py
+-rw-r--r--   0 sax        (501) staff       (20)     1131 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/demo/wsgi.py
+-rwxr-xr-x   0 sax        (501) staff       (20)      331 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/demoapp/manage.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.466127 django-adminfilters-2.2.0/tests/depot/
+-rw-r--r--   0 sax        (501) staff       (20)      121 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/depot/test_models.py
+-rw-r--r--   0 sax        (501) staff       (20)     1716 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/depot/test_widget.py
+drwxr-xr-x   0 sax        (501) staff       (20)        0 2023-05-28 18:40:55.468659 django-adminfilters-2.2.0/tests/functional/
+-rw-r--r--   0 sax        (501) staff       (20)     3313 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/functional/conftest.py
+-rw-r--r--   0 sax        (501) staff       (20)      937 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/functional/test_f_automplete.py
+-rw-r--r--   0 sax        (501) staff       (20)     1849 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/functional/test_f_depot.py
+-rw-r--r--   0 sax        (501) staff       (20)     1703 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/functional/test_f_lookup.py
+-rw-r--r--   0 sax        (501) staff       (20)     1272 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/functional/test_f_number.py
+-rw-r--r--   0 sax        (501) staff       (20)     2640 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/functional/test_f_querystring.py
+-rw-r--r--   0 sax        (501) staff       (20)     1997 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/functional/test_f_value.py
+-rw-r--r--   0 sax        (501) staff       (20)      914 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_automplete.py
+-rw-r--r--   0 sax        (501) staff       (20)     1655 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_dates.py
+-rw-r--r--   0 sax        (501) staff       (20)     1230 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_dj.py
+-rw-r--r--   0 sax        (501) staff       (20)     1001 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_django_check.py
+-rw-r--r--   0 sax        (501) staff       (20)      843 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_extra.py
+-rw-r--r--   0 sax        (501) staff       (20)     3678 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_json.py
+-rw-r--r--   0 sax        (501) staff       (20)     2738 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_multiselect.py
+-rw-r--r--   0 sax        (501) staff       (20)     1252 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_number.py
+-rw-r--r--   0 sax        (501) staff       (20)     1582 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_querystring.py
+-rw-r--r--   0 sax        (501) staff       (20)     2283 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_related.py
+-rw-r--r--   0 sax        (501) staff       (20)      662 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_utils.py
+-rw-r--r--   0 sax        (501) staff       (20)     2051 2023-05-28 10:34:10.000000 django-adminfilters-2.2.0/tests/test_value.py
+-rw-r--r--   0 sax        (501) staff       (20)     1556 2023-05-28 17:49:22.000000 django-adminfilters-2.2.0/tox.ini
```

### Comparing `django-adminfilters-2.1.0/CHANGES.md` & `django-adminfilters-2.2.0/CHANGES.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,7 +1,12 @@
+Release 2.2
+=============
+* Improves support for JsonFields (use `#` to cast integer `.` to cast float)
+
+
 Release 2.1
 =============
 * add DateRangeFilter
 * removes `default_app_config`
 * Merge #27 - Foreign Key can refer not only to pk field (@ef-end-y)
```

### Comparing `django-adminfilters-2.1.0/LICENSE` & `django-adminfilters-2.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/MANIFEST.in` & `django-adminfilters-2.2.0/MANIFEST.in`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/PKG-INFO` & `django-adminfilters-2.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-adminfilters
-Version: 2.1.0
+Version: 2.2.0
 Summary: Extra filters for django admin site
 Home-page: https://github.com/saxix/django-adminfilters
 Download-URL: https://github.com/saxix/django-adminfilters
 Author: sax
 Author-email: s.apostolico@gmail.com
 License: MIT
 Platform: any
@@ -48,14 +48,16 @@
   * AutocompleteFilter
 * Simple
   * ValueFilter
 * Combobox
   * AllValuesComboFilter
   * RelatedFieldComboFilter
   * ChoicesFieldComboFilter
+* Dates
+  * DateRangeFilter
 * Radio
   * AllValuesRadioFilter
   * RelatedFieldRadioFilter
   * ChoicesFieldRadioFilter
   * BooleanRadioFilter
 * Checkbox
   * RelatedFieldCheckBoxFilter
```

### Comparing `django-adminfilters-2.1.0/README.md` & `django-adminfilters-2.2.0/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -21,14 +21,16 @@
   * AutocompleteFilter
 * Simple
   * ValueFilter
 * Combobox
   * AllValuesComboFilter
   * RelatedFieldComboFilter
   * ChoicesFieldComboFilter
+* Dates
+  * DateRangeFilter
 * Radio
   * AllValuesRadioFilter
   * RelatedFieldRadioFilter
   * ChoicesFieldRadioFilter
   * BooleanRadioFilter
 * Checkbox
   * RelatedFieldCheckBoxFilter
```

### Comparing `django-adminfilters-2.1.0/docs/_ext/djangodocs.py` & `django-adminfilters-2.2.0/docs/_ext/djangodocs.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,40 +1,40 @@
 """
 Sphinx plugins for Django documentation.
 """
 import json
 import os
 import re
 
-from sphinx import __version__ as sphinx_ver, addnodes
+from sphinx import __version__ as sphinx_ver
+from sphinx import addnodes
 from sphinx.builders.html import StandaloneHTMLBuilder
 from sphinx.util.compat import Directive
 from sphinx.util.console import bold
 from sphinx.writers.html import SmartyPantsHTMLTranslator
 
 # RE for option descriptions without a '--' prefix
-simple_option_desc_re = re.compile(
-    r'([-_a-zA-Z0-9]+)(\s*.*?)(?=,\s+(?:/|-|--)|$)')
+simple_option_desc_re = re.compile(r'([-_a-zA-Z0-9]+)(\s*.*?)(?=,\s+(?:/|-|--)|$)')
 
 
 def setup(app):
     app.add_crossref_type(
         directivename='setting',
         rolename='setting',
         indextemplate='pair: %s; setting',
     )
     app.add_crossref_type(
         directivename='templatetag',
         rolename='ttag',
-        indextemplate='pair: %s; template tag'
+        indextemplate='pair: %s; template tag',
     )
     app.add_crossref_type(
         directivename='templatefilter',
         rolename='tfilter',
-        indextemplate='pair: %s; template filter'
+        indextemplate='pair: %s; template filter',
     )
     app.add_crossref_type(
         directivename='fieldlookup',
         rolename='lookup',
         indextemplate='pair: %s; field lookup type',
     )
     app.add_description_unit(
@@ -69,15 +69,17 @@
         ret.append(node)
         if self.arguments[0] == env.config.django_next_version:
             node['version'] = 'Development version'
         else:
             node['version'] = self.arguments[0]
         node['type'] = self.name
         if len(self.arguments) == 2:
-            inodes, messages = self.state.inline_text(self.arguments[1], self.lineno + 1)
+            inodes, messages = self.state.inline_text(
+                self.arguments[1], self.lineno + 1
+            )
             node.extend(inodes)
             if self.content:
                 self.state.nested_parse(self.content, self.content_offset, node)
             ret = ret + messages
         env.note_versionchange(node['type'], node['version'], node, self.lineno)
         return ret
 
@@ -125,20 +127,18 @@
     version_text = {
         'deprecated': 'Deprecated in Django %s',
         'versionchanged': 'Changed in Django %s',
         'versionadded': 'New in Django %s',
     }
 
     def visit_versionmodified(self, node):
-        self.body.append(
-            self.starttag(node, 'div', CLASS=node['type'])
-        )
+        self.body.append(self.starttag(node, 'div', CLASS=node['type']))
         title = '%s%s' % (
             self.version_text[node['type']] % node['version'],
-            len(node) and ':' or '.'
+            len(node) and ':' or '.',
         )
         self.body.append('<span class="title">%s</span> ' % title)
 
     def depart_versionmodified(self, node):
         self.body.append('</div>\n')
 
     # Give each section a unique ID -- nice for custom CSS hooks
@@ -157,14 +157,15 @@
     signode += addnodes.desc_name(title, title)
     return sig
 
 
 def parse_django_adminopt_node(env, sig, signode):
     """A copy of sphinx.directives.CmdoptionDesc.parse_signature()"""
     from sphinx.domains.std import option_desc_re
+
     count = 0
     firstname = ''
     for m in option_desc_re.finditer(sig):
         optname, args = m.groups()
         if count:
             signode += addnodes.desc_addname(', ', ', ')
         signode += addnodes.desc_name(optname, optname)
@@ -195,17 +196,23 @@
     name = 'djangohtml'
 
     def finish(self):
         super().finish()
         self.info(bold('writing templatebuiltins.js...'))
         xrefs = self.env.domaindata['std']['objects']
         templatebuiltins = {
-            'ttags': [n for ((t, n), (lnk, a)) in xrefs.items()
-                      if t == 'templatetag' and lnk == 'ref/templates/builtins'],
-            'tfilters': [n for ((t, n), (lnk, a)) in xrefs.items()
-                         if t == 'templatefilter' and lnk == 'ref/templates/builtins'],
+            'ttags': [
+                n
+                for ((t, n), (lnk, a)) in xrefs.items()
+                if t == 'templatetag' and lnk == 'ref/templates/builtins'
+            ],
+            'tfilters': [
+                n
+                for ((t, n), (lnk, a)) in xrefs.items()
+                if t == 'templatefilter' and lnk == 'ref/templates/builtins'
+            ],
         }
         outfilename = os.path.join(self.outdir, 'templatebuiltins.js')
         with open(outfilename, 'wb') as fp:
             fp.write('var django_template_builtins = ')
             json.dump(templatebuiltins, fp)
             fp.write(';\n')
```

### Comparing `django-adminfilters-2.1.0/docs/_ext/github.py` & `django-adminfilters-2.2.0/docs/_ext/github.py`

 * *Files 6% similar despite different names*

```diff
@@ -34,23 +34,26 @@
     try:
         base = app.config.github_project_url
         if not base:
             raise AttributeError
         if not base.endswith('/'):
             base += '/'
     except AttributeError as err:
-        raise ValueError('github_project_url configuration value is not set (%s)' % str(err))
+        raise ValueError(
+            'github_project_url configuration value is not set (%s)' % str(err)
+        )
 
     ref = base + type + '/' + slug + '/'
     set_classes(options)
     prefix = '#'
     if type == 'pull':
         prefix = 'PR ' + prefix
-    node = nodes.reference(rawtext, prefix + utils.unescape(slug), refuri=ref,
-                           **options)
+    node = nodes.reference(
+        rawtext, prefix + utils.unescape(slug), refuri=ref, **options
+    )
     return node
 
 
 def ghissue_role(name, rawtext, text, lineno, inliner, options={}, content=[]):
     """Link to a GitHub issue.
 
     Returns 2 part tuple containing list of nodes to insert into the
@@ -69,26 +72,29 @@
     try:
         issue_num = int(text)
         if issue_num <= 0:
             raise ValueError
     except ValueError:
         msg = inliner.reporter.error(
             'GitHub issue number must be a number greater than or equal to 1; '
-            '"%s" is invalid.' % text, line=lineno)
+            '"%s" is invalid.' % text,
+            line=lineno,
+        )
         prb = inliner.problematic(rawtext, rawtext, msg)
         return [prb], [msg]
     app = inliner.document.settings.env.app
     if 'pull' in name.lower():
         category = 'pull'
     elif 'issue' in name.lower():
         category = 'issues'
     else:
         msg = inliner.reporter.error(
-            'GitHub roles include "ghpull" and "ghissue", '
-            '"%s" is invalid.' % name, line=lineno)
+            'GitHub roles include "ghpull" and "ghissue", ' '"%s" is invalid.' % name,
+            line=lineno,
+        )
         prb = inliner.problematic(rawtext, rawtext, msg)
         return [prb], [msg]
     node = make_link_node(rawtext, app, category, str(issue_num), options)
     return [node], []
 
 
 def ghuser_role(name, rawtext, text, lineno, inliner, options={}, content=[]):
@@ -131,15 +137,17 @@
     try:
         base = app.config.github_project_url
         if not base:
             raise AttributeError
         if not base.endswith('/'):
             base += '/'
     except AttributeError as err:
-        raise ValueError('github_project_url configuration value is not set (%s)' % str(err))
+        raise ValueError(
+            'github_project_url configuration value is not set (%s)' % str(err)
+        )
 
     ref = base + text
     node = nodes.reference(rawtext, text[:6], refuri=ref, **options)
     return [node], []
 
 
 def setup(app):
```

### Comparing `django-adminfilters-2.1.0/docs/_ext/version.py` & `django-adminfilters-2.2.0/docs/_ext/version.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,31 +1,30 @@
 import re
 
 from sphinx import addnodes, roles
 from sphinx.util.compat import Directive
 
-simple_option_desc_re = re.compile(
-    r'([-_a-zA-Z0-9]+)(\s*.*?)(?=,\s+(?:/|-|--)|$)')
+simple_option_desc_re = re.compile(r'([-_a-zA-Z0-9]+)(\s*.*?)(?=,\s+(?:/|-|--)|$)')
 
 
 def setup(app):
     app.add_crossref_type(
         directivename='setting',
         rolename='setting',
         indextemplate='pair: %s; setting',
     )
     app.add_crossref_type(
         directivename='templatetag',
         rolename='ttag',
-        indextemplate='pair: %s; template tag'
+        indextemplate='pair: %s; template tag',
     )
     app.add_crossref_type(
         directivename='templatefilter',
         rolename='tfilter',
-        indextemplate='pair: %s; template filter'
+        indextemplate='pair: %s; template filter',
     )
     app.add_crossref_type(
         directivename='fieldlookup',
         rolename='lookup',
         indextemplate='pair: %s; field lookup type',
     )
     app.add_config_value('next_version', '0.0', True)
```

### Comparing `django-adminfilters-2.1.0/docs/conf.py` & `django-adminfilters-2.2.0/docs/conf.py`

 * *Files 4% similar despite different names*

```diff
@@ -13,16 +13,15 @@
 import sys
 
 from django.conf import settings
 
 import adminfilters as app
 
 here = os.path.abspath(os.path.join(os.path.dirname(__file__)))
-up = lambda base, level: os.path.abspath(
-    os.path.join(base, *([os.pardir] * level)))
+up = lambda base, level: os.path.abspath(os.path.join(base, *([os.pardir] * level)))
 sys.path.insert(0, up(here, 2))
 
 settings.configure(SITE_ID=1)
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
@@ -31,28 +30,28 @@
 # -- General configuration -----------------------------------------------
 
 # If your documentation needs a minimal Sphinx version, state it here.
 needs_sphinx = '1.0'
 
 # Add any Sphinx extension module names here, as strings. They can be extensions
 # coming with Sphinx (named 'sphinx.ext.*') or your custom ones.
-sys.path.append(os.path.abspath(
-    os.path.join(os.path.dirname(__file__), '_ext')))
-extensions = ['sphinx.ext.autodoc',
-              'sphinx.ext.todo',
-              'sphinx.ext.graphviz',
-              'sphinx.ext.intersphinx',
-              'sphinx.ext.doctest',
-              'sphinx.ext.extlinks',
-              'sphinx.ext.autosummary',
-              'sphinx.ext.coverage',
-              'sphinx.ext.viewcode',
-              'sphinxcontrib.video',
-              'github',
-              ]
+sys.path.append(os.path.abspath(os.path.join(os.path.dirname(__file__), '_ext')))
+extensions = [
+    'sphinx.ext.autodoc',
+    'sphinx.ext.todo',
+    'sphinx.ext.graphviz',
+    'sphinx.ext.intersphinx',
+    'sphinx.ext.doctest',
+    'sphinx.ext.extlinks',
+    'sphinx.ext.autosummary',
+    'sphinx.ext.coverage',
+    'sphinx.ext.viewcode',
+    'sphinxcontrib.video',
+    'github',
+]
 
 next_version = 'dev'
 github_project_url = 'https://github.com/saxix/django-adminfilters/'
 github_project_url_basesource = 'https://github.com/saxix/django-adminfilters/'
 
 todo_include_todos = True
 intersphinx_mapping = {
@@ -71,16 +70,16 @@
 # The encoding of source files.
 # source_encoding = 'utf-8-sig'
 
 # The master toctree document.
 master_doc = 'index'
 
 # General information about the project.
-project = u'Django AdminFilters'
-copyright = u'2012-2022, Stefano Apostolico'
+project = 'Django AdminFilters'
+copyright = '2012-2022, Stefano Apostolico'
 
 # The version info for the project you're documenting, acts as replacement for
 # |version| and |release|, also used in various other places throughout the
 # built documents.
 #
 # The short X.Y version.
 version = app.VERSION
@@ -220,16 +219,21 @@
 
 # The font size ('10pt', '11pt' or '12pt').
 # latex_font_size = '10pt'
 
 # Grouping the document tree into LaTeX files. List of tuples
 # (source start file, target name, title, author, documentclass [howto/manual]).
 latex_documents = [
-    ('index', 'DjangoAdminActions.tex', u'Django Admin Actions Documentation',
-     u'Stefano Apostolico', 'manual'),
+    (
+        'index',
+        'DjangoAdminActions.tex',
+        'Django Admin Actions Documentation',
+        'Stefano Apostolico',
+        'manual',
+    ),
 ]
 
 # The name of an image file (relative to this directory) to place at the top of
 # the title page.
 # latex_logo = None
 
 # For "manual" documents, if this is true, then toplevel headings are parts,
@@ -253,10 +257,15 @@
 
 
 # -- Options for manual page output --------------------------------------
 
 # One entry per manual page. List of tuples
 # (source start file, name, description, authors, manual section).
 man_pages = [
-    ('index', 'djangoadminactions', u'Django Admin Actions Documentation',
-     [u'Stefano Apostolico'], 1)
+    (
+        'index',
+        'djangoadminactions',
+        'Django Admin Actions Documentation',
+        ['Stefano Apostolico'],
+        1,
+    )
 ]
```

### Comparing `django-adminfilters-2.1.0/setup.py` & `django-adminfilters-2.2.0/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -23,38 +23,37 @@
     return codecs.open(os.path.join(here, 'src', 'requirements', *parts), 'r').read()
 
 
 install_requires = read('install.pip')
 tests_requires = read('testing.pip')
 dev_requires = tests_requires + read('develop.pip')
 
-setup(name=name,
-      version=version,
-      url='https://github.com/saxix/django-adminfilters',
-      download_url='https://github.com/saxix/django-adminfilters',
-      author='sax',
-      author_email='s.apostolico@gmail.com',
-      description='Extra filters for django admin site',
-      license='MIT',
-      package_dir={'': 'src'},
-      packages=find_packages('src'),
-      include_package_data=True,
-      extras_require={
-          'test': tests_requires,
-          'dev': dev_requires
-      },
-      platforms=['any'],
-      classifiers=[
-          'Environment :: Web Environment',
-          'Framework :: Django',
-          'Framework :: Django :: 2.2',
-          'Framework :: Django :: 3.2',
-          'Framework :: Django :: 4.0',
-          'Operating System :: OS Independent',
-          'Programming Language :: Python',
-          'Programming Language :: Python :: 3.8',
-          'Programming Language :: Python :: 3.9',
-          'Programming Language :: Python :: 3.10',
-          'Intended Audience :: Developers'],
-      long_description=codecs.open('README.md', 'r').read(),
-      long_description_content_type='text/markdown',
-      )
+setup(
+    name=name,
+    version=version,
+    url='https://github.com/saxix/django-adminfilters',
+    download_url='https://github.com/saxix/django-adminfilters',
+    author='sax',
+    author_email='s.apostolico@gmail.com',
+    description='Extra filters for django admin site',
+    license='MIT',
+    package_dir={'': 'src'},
+    packages=find_packages('src'),
+    include_package_data=True,
+    extras_require={'test': tests_requires, 'dev': dev_requires},
+    platforms=['any'],
+    classifiers=[
+        'Environment :: Web Environment',
+        'Framework :: Django',
+        'Framework :: Django :: 2.2',
+        'Framework :: Django :: 3.2',
+        'Framework :: Django :: 4.0',
+        'Operating System :: OS Independent',
+        'Programming Language :: Python',
+        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Intended Audience :: Developers',
+    ],
+    long_description=codecs.open('README.md', 'r').read(),
+    long_description_content_type='text/markdown',
+)
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/autocomplete.py` & `django-adminfilters-2.2.0/src/adminfilters/autocomplete.py`

 * *Files 22% similar despite different names*

```diff
@@ -5,77 +5,92 @@
 from django.urls import reverse
 from django.utils.translation import get_language
 
 from adminfilters.mixin import MediaDefinitionFilter, SmartFieldListFilter
 
 
 def get_real_field(model, path):
-    parts = path.split('__')
+    parts = path.split("__")
     current = model
     for p in parts:
         f = current._meta.get_field(p)
         if f.related_model:
             current = f.related_model
     return f
 
 
 class AutoCompleteFilter(SmartFieldListFilter, MediaDefinitionFilter):
-    template = 'adminfilters/autocomplete.html'
-    url_name = '%s:%s_%s_autocomplete'
+    template = "adminfilters/autocomplete.html"
+    url_name = "%s:%s_%s_autocomplete"
 
     def __init__(self, field, request, params, model, model_admin, field_path):
-        self.lookup_kwarg = '%s__exact' % field_path
-        self.lookup_kwarg_isnull = '%s__isnull' % field_path
+        self.lookup_kwarg = "%s__exact" % field_path
+        self.lookup_kwarg_isnull = "%s__isnull" % field_path
         self.lookup_val = params.get(self.lookup_kwarg)
         super().__init__(field, request, params, model, model_admin, field_path)
         self.admin_site = model_admin.admin_site
-        self.query_string = ''
+        self.query_string = ""
         self.target_field = get_real_field(model, field_path)
         self.target_model = self.target_field.related_model
 
         if django.VERSION[0] >= 3:
             self.target_opts = self.target_field.model._meta
         elif django.VERSION[0] == 2:
             self.target_opts = self.target_model._meta
 
-        if not hasattr(field, 'get_limit_choices_to'):
-            raise Exception(f"Filter '{field_path}' of {model_admin} is not supported by AutoCompleteFilter."
-                            f' Check your {model_admin}.list_filter value')
+        if not hasattr(field, "get_limit_choices_to"):
+            raise Exception(
+                f"Filter '{field_path}' of {model_admin} is not supported by AutoCompleteFilter."
+                f" Check your {model_admin}.list_filter value"
+            )
 
         self.url = self.get_url()
 
     def expected_parameters(self):
         return [self.lookup_kwarg, self.lookup_kwarg_isnull]
 
     def get_url(self):
         if django.VERSION[:2] >= (3, 2):
-            return reverse('%s:autocomplete' % self.admin_site.name)
-        return reverse(self.url_name % (self.admin_site.name,
-                                        self.target_opts.app_label,
-                                        self.target_opts.model_name))
+            return reverse("%s:autocomplete" % self.admin_site.name)
+        return reverse(
+            self.url_name
+            % (
+                self.admin_site.name,
+                self.target_opts.app_label,
+                self.target_opts.model_name,
+            )
+        )
 
     def choices(self, changelist):
-        self.query_string = changelist.get_query_string(remove=[self.lookup_kwarg, self.lookup_kwarg_isnull])
+        self.query_string = changelist.get_query_string(
+            remove=[self.lookup_kwarg, self.lookup_kwarg_isnull]
+        )
         if self.lookup_val:
             get_kwargs = {self.field.target_field.name: self.lookup_val}
-            return [str(self.target_model.objects.get(**get_kwargs)) or '']
+            return [str(self.target_model.objects.get(**get_kwargs)) or ""]
         return []
 
     @property
     def media(self):
-        extra = '' if settings.DEBUG else '.min'
+        extra = "" if settings.DEBUG else ".min"
         i18n_name = SELECT2_TRANSLATIONS.get(get_language())
-        i18n_file = ('admin/js/vendor/select2/i18n/%s.js' % i18n_name,) if i18n_name else ()
+        i18n_file = (
+            ("admin/js/vendor/select2/i18n/%s.js" % i18n_name,) if i18n_name else ()
+        )
         return forms.Media(
-            js=('admin/js/vendor/jquery/jquery%s.js' % extra,
-                'admin/js/vendor/select2/select2.full%s.js' % extra,
-                ) + i18n_file + ('admin/js/jquery.init.js',
-                                 'admin/js/autocomplete.js',
-                                 'adminfilters/autocomplete%s.js' % extra,
-                                 ),
+            js=(
+                "admin/js/vendor/jquery/jquery%s.js" % extra,
+                "admin/js/vendor/select2/select2.full%s.js" % extra,
+            )
+            + i18n_file
+            + (
+                "admin/js/jquery.init.js",
+                "admin/js/autocomplete.js",
+                "adminfilters/autocomplete%s.js" % extra,
+            ),
             css={
-                'screen': (
-                    'admin/css/vendor/select2/select2%s.css' % extra,
-                    'adminfilters/adminfilters.css',
+                "screen": (
+                    "admin/css/vendor/select2/select2%s.css" % extra,
+                    "adminfilters/adminfilters.css",
                 ),
             },
         )
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/checkbox.py` & `django-adminfilters-2.2.0/src/adminfilters/checkbox.py`

 * *Files 16% similar despite different names*

```diff
@@ -4,73 +4,89 @@
 from django.utils.encoding import smart_str
 from django.utils.translation import gettext as _
 
 from .mixin import MediaDefinitionFilter, WrappperMixin
 from .utils import parse_bool
 
 
-class RelatedFieldCheckBoxFilter(WrappperMixin, MediaDefinitionFilter, RelatedFieldListFilter):
-    template = 'adminfilters/checkbox.html'
+class RelatedFieldCheckBoxFilter(
+    WrappperMixin, MediaDefinitionFilter, RelatedFieldListFilter
+):
+    template = "adminfilters/checkbox.html"
 
     def __init__(self, field, request, params, model, model_admin, field_path):
         self.model_admin = model_admin
         super().__init__(field, request, params, model, model_admin, field_path)
-        self.lookup_kwarg = '%s__%s' % (field_path, field.target_field.name)
+        self.lookup_kwarg = "%s__%s" % (field_path, field.target_field.name)
         self.lookup_val = request.GET.getlist(self.lookup_kwarg, [])
 
     def queryset(self, request, queryset):
         filters = Q()
         if self.lookup_val:
-            filters.add(Q(**{f'{self.lookup_kwarg}__in': self.lookup_val}), Q.OR)
+            filters.add(Q(**{f"{self.lookup_kwarg}__in": self.lookup_val}), Q.OR)
 
         if self.lookup_val_isnull:
-            filters.add(Q(**{self.lookup_kwarg_isnull: parse_bool(self.lookup_val_isnull)}), Q.OR)
+            filters.add(
+                Q(**{self.lookup_kwarg_isnull: parse_bool(self.lookup_val_isnull)}),
+                Q.OR,
+            )
         return queryset.filter(filters)
 
     def choices(self, cl):
         try:
             from django.contrib.admin.views.main import EMPTY_CHANGELIST_VALUE
         except ImportError:
             EMPTY_CHANGELIST_VALUE = self.model_admin.get_empty_value_display()
 
         uncheck_all = []
-        uncheck_all.append('{}={}'.format(self.lookup_kwarg_isnull, 1))
+        uncheck_all.append("{}={}".format(self.lookup_kwarg_isnull, 1))
         for i in self.lookup_choices:
-            uncheck_all.append('{}={}'.format(self.lookup_kwarg, i[0]))
+            uncheck_all.append("{}={}".format(self.lookup_kwarg, i[0]))
 
         yield {
-            'selected': not len(self.lookup_val) and not self.lookup_val_isnull,
-            'query_string': cl.get_query_string({}, [self.lookup_kwarg, self.lookup_kwarg_isnull]),
-            'display': _('All'),
-            'check_to_remove': '&'.join(uncheck_all)
-
+            "selected": not len(self.lookup_val) and not self.lookup_val_isnull,
+            "query_string": cl.get_query_string(
+                {}, [self.lookup_kwarg, self.lookup_kwarg_isnull]
+            ),
+            "display": _("All"),
+            "check_to_remove": "&".join(uncheck_all),
         }
         yield {
-            'selected': self.lookup_val_isnull,
-            'query_string': cl.get_query_string({self.lookup_kwarg_isnull: 1},
-                                                [self.lookup_kwarg, self.lookup_kwarg_isnull]),
-            'display': _('None'),
-            'uncheck_to_remove': '{}=1'.format(self.lookup_kwarg_isnull)
+            "selected": self.lookup_val_isnull,
+            "query_string": cl.get_query_string(
+                {self.lookup_kwarg_isnull: 1},
+                [self.lookup_kwarg, self.lookup_kwarg_isnull],
+            ),
+            "display": _("None"),
+            "uncheck_to_remove": "{}=1".format(self.lookup_kwarg_isnull),
         }
         for pk_val, val in self.lookup_choices:
             yield {
-                'selected': smart_str(pk_val) in self.lookup_val,
-                'query_string': cl.get_query_string(
+                "selected": smart_str(pk_val) in self.lookup_val,
+                "query_string": cl.get_query_string(
                     {
                         self.lookup_kwarg: pk_val,
                     },
-                    [self.lookup_kwarg_isnull]),
-                'display': val,
-                'uncheck_to_remove': '{}={}'.format(self.lookup_kwarg, pk_val) if pk_val else ''
+                    [self.lookup_kwarg_isnull],
+                ),
+                "display": val,
+                "uncheck_to_remove": "{}={}".format(self.lookup_kwarg, pk_val)
+                if pk_val
+                else "",
             }
-        if ((isinstance(self.field, ForeignObjectRel) and self.field.field.null or
-             hasattr(self.field, 'rel') and self.field.null)):
+        if (
+            isinstance(self.field, ForeignObjectRel)
+            and self.field.field.null
+            or hasattr(self.field, "rel")
+            and self.field.null
+        ):
             yield {
-                'selected': bool(self.lookup_val_isnull),
-                'query_string': cl.get_query_string(
+                "selected": bool(self.lookup_val_isnull),
+                "query_string": cl.get_query_string(
                     {
-                        self.lookup_kwarg_isnull: 'True',
+                        self.lookup_kwarg_isnull: "True",
                     },
-                    [self.lookup_kwarg]),
-                'uncheck_to_remove': '{}=1'.format(self.lookup_kwarg_isnull),
-                'display': EMPTY_CHANGELIST_VALUE,
+                    [self.lookup_kwarg],
+                ),
+                "uncheck_to_remove": "{}=1".format(self.lookup_kwarg_isnull),
+                "display": EMPTY_CHANGELIST_VALUE,
             }
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/checks.py` & `django-adminfilters-2.2.0/src/adminfilters/checks.py`

 * *Files 7% similar despite different names*

```diff
@@ -7,23 +7,30 @@
 
 
 @register()
 def check_adminfilters_media(*args, **kwargs):
     errors = []
     try:
         from django.contrib.admin import site
+
         for model, model_admin in site._registry.items():
             if isclass(model_admin) and not issubclass(model_admin, AdminFiltersMixin):
                 for filter_fields in model_admin.list_filter:
                     filter_class = None
                     if isinstance(filter_fields, tuple):
                         filter_class = filter_fields[1]
-                    elif isclass(filter_fields) and issubclass(filter_fields, (ListFilter,)):
+                    elif isclass(filter_fields) and issubclass(
+                        filter_fields, (ListFilter,)
+                    ):
                         filter_class = filter_fields
 
                     if filter_class and issubclass(filter_class, MediaDefinitionFilter):
-                        errors.append(Error(f"To use '{filter_class.__name__}', "
-                                            f"'{model_admin.__name__}' must inherit from 'AdminFiltersMixin'"))
+                        errors.append(
+                            Error(
+                                f"To use '{filter_class.__name__}', "
+                                f"'{model_admin.__name__}' must inherit from 'AdminFiltersMixin'"
+                            )
+                        )
                         break
     except Exception:  # pragma: no-cover
         raise
     return errors
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/dates.py` & `django-adminfilters-2.2.0/src/adminfilters/dates.py`

 * *Files 9% similar despite different names*

```diff
@@ -3,50 +3,49 @@
 from django.contrib.admin.options import IncorrectLookupParameters
 from django.db.models import DateField, DateTimeField
 
 from adminfilters.numbers import NumberFilter
 
 
 class DateRangeFilter(NumberFilter):
-    rex1 = re.compile(r'^(>=|<=|>|<|=)?(\d{4}-\d{2}-\d{2})$')
-    re_range = re.compile(r'^(\d{4}-\d{2}-\d{2})..(\d{4}-\d{2}-\d{2})$')
-    re_list = re.compile(r'(\d{4}-\d{2}-\d{2}),?')
-    re_unlike = re.compile(r'^(<>)(?P<date>\d{4}-\d{2}-\d{2})$')
+    rex1 = re.compile(r"^(>=|<=|>|<|=)?(\d{4}-\d{2}-\d{2})$")
+    re_range = re.compile(r"^(\d{4}-\d{2}-\d{2})..(\d{4}-\d{2}-\d{2})$")
+    re_list = re.compile(r"(\d{4}-\d{2}-\d{2}),?")
+    re_unlike = re.compile(r"^(<>)(?P<date>\d{4}-\d{2}-\d{2})$")
 
     def __init__(self, field, request, params, model, model_admin, field_path):
         super().__init__(field, request, params, model, model_admin, field_path)
         if isinstance(field, DateTimeField):
-            self.extra_lookup = '__date'
+            self.extra_lookup = "__date"
         elif isinstance(field, DateField):
-            self.extra_lookup = ''
+            self.extra_lookup = ""
 
     def queryset(self, request, queryset):
         if self.value() and self.value()[0]:
             raw_value = self.value()[0]
             m1 = self.rex1.match(raw_value)
             m_range = self.re_range.match(raw_value)
             m_list = self.re_list.match(raw_value)
             m_unlike = self.re_unlike.match(raw_value)
-            lk = f'{self.field.name}{self.extra_lookup}'
+            lk = f"{self.field.name}{self.extra_lookup}"
             if m_unlike and m_unlike.groups():
-                match = f'{lk}__exact'
+                match = f"{lk}__exact"
                 op, value = self.re_unlike.match(raw_value).groups()
                 queryset = queryset.exclude(**{match: value})
             else:
                 if m1 and m1.groups():
                     op, value = self.rex1.match(raw_value).groups()
                     match = f"{lk}__{self.map[op or '=']}"
                     self.filters = {match: value}
                 elif m_range and m_range.groups():
                     start, end = self.re_range.match(raw_value).groups()
-                    self.filters = {f'{lk}__gte': start,
-                                    f'{lk}__lte': end}
+                    self.filters = {f"{lk}__gte": start, f"{lk}__lte": end}
                 elif m_list and m_list.groups():
-                    value = raw_value.split(',')
-                    match = f'{lk}__in'
+                    value = raw_value.split(",")
+                    match = f"{lk}__in"
                     self.filters = {match: value}
                 else:  # pragma: no cover
                     raise IncorrectLookupParameters()
 
                 try:
                     queryset = queryset.filter(**self.filters)
                 except Exception:
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/depot/migrations/0002_migration.py` & `django-adminfilters-2.2.0/src/adminfilters/depot/migrations/0002_migration.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,22 +1,23 @@
 # Generated by Django 3.2.12 on 2022-04-05 21:42
 
 from django.db import migrations, models
 
 
 class Migration(migrations.Migration):
-
     dependencies = [
-        ('depot', '0001_initial'),
+        ("depot", "0001_initial"),
     ]
 
     operations = [
         migrations.AlterModelOptions(
-            name='storedfilter',
-            options={'ordering': ('name',)},
+            name="storedfilter",
+            options={"ordering": ("name",)},
         ),
         migrations.AlterField(
-            model_name='storedfilter',
-            name='id',
-            field=models.BigAutoField(auto_created=True, primary_key=True, serialize=False, verbose_name='ID'),
+            model_name="storedfilter",
+            name="id",
+            field=models.BigAutoField(
+                auto_created=True, primary_key=True, serialize=False, verbose_name="ID"
+            ),
         ),
     ]
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/depot/models.py` & `django-adminfilters-2.2.0/src/adminfilters/depot/models.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 from django.contrib.contenttypes.models import ContentType
 from django.db import models
 
 
 class StoredFilter(models.Model):
     name = models.CharField(blank=False, null=False, max_length=100)
     content_type = models.ForeignKey(ContentType, on_delete=models.CASCADE)
-    query_string = models.TextField(blank=True, null=True, default='')
+    query_string = models.TextField(blank=True, null=True, default="")
     owner = models.ForeignKey(settings.AUTH_USER_MODEL, on_delete=models.CASCADE)
 
     class Meta:
-        ordering = ('name',)
+        ordering = ("name",)
 
     def __str__(self):
         return self.name
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/depot/templates/adminfilters/widget.html` & `django-adminfilters-2.2.0/src/adminfilters/depot/templates/adminfilters/widget.html`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/depot/widget.py` & `django-adminfilters-2.2.0/src/adminfilters/depot/widget.py`

 * *Files 18% similar despite different names*

```diff
@@ -8,76 +8,86 @@
 from adminfilters.depot.models import StoredFilter
 from adminfilters.utils import get_query_string
 
 from ..mixin import WrappperMixin
 
 
 class DepotManager(WrappperMixin, ListFilter):
-    title = 'Saved Filters'
-    template = 'adminfilters/widget.html'
-    parameter_name = 'adminfilters_depot'
-    parameter_name_op = 'adminfilters_depot_op'
+    title = "Saved Filters"
+    template = "adminfilters/widget.html"
+    parameter_name = "adminfilters_depot"
+    parameter_name_op = "adminfilters_depot_op"
 
     def __init__(self, request, params, model, model_admin):
         self.model_admin = model_admin
         super().__init__(request, params, model, model_admin)
         self.request = request
-        self.query_string = get_query_string(self.request, {}, self.expected_parameters())
-        self.can_add_filter = request.user.has_perm('depot.add_storedfilter')
+        self.query_string = get_query_string(
+            self.request, {}, self.expected_parameters()
+        )
+        self.can_add_filter = request.user.has_perm("depot.add_storedfilter")
         self.content_type = ContentType.objects.get_for_model(model_admin.model)
         for p in self.expected_parameters():
             if p in params:
                 self.used_parameters[p] = params.pop(p)
 
     def has_output(self):
         return True
 
     def expected_parameters(self):
         return [self.parameter_name, self.parameter_name_op]
 
     def queryset(self, request, queryset):
         filter_name = self.used_parameters.get(self.parameter_name)
-        operation = self.used_parameters.get(self.parameter_name_op, 'add')
+        operation = self.used_parameters.get(self.parameter_name_op, "add")
         if filter_name:
-            if operation == 'add':
+            if operation == "add":
                 qs = get_query_string(request, {}, self.expected_parameters())
 
-                StoredFilter.objects.update_or_create(content_type=self.content_type,
-                                                      name=filter_name,
-                                                      defaults={
-                                                          'query_string': qs,
-                                                          'owner': request.user,
-                                                      })
-                self.model_admin.message_user(self.request, f"Filter '{filter_name}' successfully saved")
-            elif operation == 'delete':
+                StoredFilter.objects.update_or_create(
+                    content_type=self.content_type,
+                    name=filter_name,
+                    defaults={
+                        "query_string": qs,
+                        "owner": request.user,
+                    },
+                )
+                self.model_admin.message_user(
+                    self.request, f"Filter '{filter_name}' successfully saved"
+                )
+            elif operation == "delete":
                 StoredFilter.objects.filter(id=filter_name).delete()
         return queryset
 
     def choices(self, changelist):
         self.selected = False
-        for f in StoredFilter.objects.filter(content_type=self.content_type).order_by('name'):
+        for f in StoredFilter.objects.filter(content_type=self.content_type).order_by(
+            "name"
+        ):
             if str(self.query_string) == str(f.query_string):
                 self.selected = True
                 self.selected_id = f.pk
 
             yield {
-                'selected': str(self.query_string) == str(f.query_string),
-                'query_string': f.query_string,
-                'name': f.name,
+                "selected": str(self.query_string) == str(f.query_string),
+                "query_string": f.query_string,
+                "name": f.name,
             }
 
     @property
     def media(self):
-        extra = '' if settings.DEBUG else '.min'
+        extra = "" if settings.DEBUG else ".min"
         i18n_name = SELECT2_TRANSLATIONS.get(get_language())
-        i18n_file = ('admin/js/vendor/select2/i18n/%s.js' % i18n_name,) if i18n_name else ()
+        i18n_file = (
+            ("admin/js/vendor/select2/i18n/%s.js" % i18n_name,) if i18n_name else ()
+        )
         return forms.Media(
-            js=('admin/js/vendor/jquery/jquery%s.js' % extra,
-                ) + i18n_file + ('admin/js/jquery.init.js',
-                                 'adminfilters/depot%s.js' % extra,
-                                 ),
+            js=("admin/js/vendor/jquery/jquery%s.js" % extra,)
+            + i18n_file
+            + (
+                "admin/js/jquery.init.js",
+                "adminfilters/depot%s.js" % extra,
+            ),
             css={
-                'screen': (
-                    'adminfilters/adminfilters.css',
-                ),
+                "screen": ("adminfilters/adminfilters.css",),
             },
         )
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/dj.py` & `django-adminfilters-2.2.0/src/adminfilters/dj.py`

 * *Files 12% similar despite different names*

```diff
@@ -1,81 +1,89 @@
 from django import forms
 from django.conf import settings
 from django.contrib.admin.widgets import SELECT2_TRANSLATIONS
 from django.core.exceptions import FieldError, ValidationError
 from django.db.models import Q
-from django.utils.translation import get_language, gettext as _
+from django.utils.translation import get_language
+from django.utils.translation import gettext as _
 
 from .mixin import MediaDefinitionFilter, SmartListFilter
 from .utils import cast_value, get_field_type, get_message_from_exception
 
 
 class DjangoLookupFilter(MediaDefinitionFilter, SmartListFilter):
-    parameter_name = 'dj'
-    title = 'Django Lookup'
-    template = 'adminfilters/dj.html'
+    parameter_name = "dj"
+    title = "Django Lookup"
+    template = "adminfilters/dj.html"
     can_negate = True
     negated = False
     button = True
-    field_placeholder = _('field lookup. Es. name__startswith')
-    placeholder = _('field value')
+    field_placeholder = _("field lookup. Es. name__startswith")
+    placeholder = _("field value")
 
     def __init__(self, request, params, model, model_admin):
-        self.lookup_kwarg_key = '%s__key' % self.parameter_name
-        self.lookup_kwarg_value = '%s__value' % self.parameter_name
-        self.lookup_kwarg_negated = '%s__negate' % self.parameter_name
-        self.lookup_field_val = params.pop(self.lookup_kwarg_key, '')
-        self.lookup_value_val = params.pop(self.lookup_kwarg_value, '')
-        self.lookup_negated_val = params.pop(self.lookup_kwarg_negated, 'false')
+        self.lookup_kwarg_key = "%s__key" % self.parameter_name
+        self.lookup_kwarg_value = "%s__value" % self.parameter_name
+        self.lookup_kwarg_negated = "%s__negate" % self.parameter_name
+        self.lookup_field_val = params.pop(self.lookup_kwarg_key, "")
+        self.lookup_value_val = params.pop(self.lookup_kwarg_value, "")
+        self.lookup_negated_val = params.pop(self.lookup_kwarg_negated, "false")
         self.error_message = None
         self.exception = None
         self.filters = None
         self.exclude = None
         self.model = model
         self.query_string = None
         super().__init__(request, params, model, model_admin)
 
     @classmethod
     def factory(cls, **kwargs):
-        return type('DjangoLookupFilter', (cls,), kwargs)
+        return type("DjangoLookupFilter", (cls,), kwargs)
 
     def expected_parameters(self):
-        return [self.lookup_kwarg_key,
-                self.lookup_kwarg_value,
-                self.lookup_kwarg_negated]
+        return [
+            self.lookup_kwarg_key,
+            self.lookup_kwarg_value,
+            self.lookup_kwarg_negated,
+        ]
 
     def has_output(self):
         return True
 
     def value(self):
         try:
             if self.lookup_field_val:
-                field, lookup, field_type = get_field_type(self.model, self.lookup_field_val)
+                field, lookup, field_type = get_field_type(
+                    self.model, self.lookup_field_val
+                )
                 value = cast_value(self.lookup_value_val, field, lookup)
                 return [
                     self.lookup_field_val,
                     value,
-                    (self.can_negate and self.lookup_negated_val == 'true') or self.negated,
+                    (self.can_negate and self.lookup_negated_val == "true")
+                    or self.negated,
                 ]
         except ValidationError as e:  # pragma: no cover
             self.exception = e
             self.error_message = str(e.message)
 
         return [None, None, None]
 
     def choices(self, changelist):
-        self.query_string = changelist.get_query_string(remove=self.expected_parameters())
+        self.query_string = changelist.get_query_string(
+            remove=self.expected_parameters()
+        )
         return []
 
     def queryset(self, request, queryset):
         try:
             key, value, negated = self.value()
             if key:
                 try:
-                    self.filters = Q(**{f'{self.lookup_field_val}': value})
+                    self.filters = Q(**{f"{self.lookup_field_val}": value})
 
                     if negated:
                         self.filters = ~self.filters
 
                     queryset = queryset.filter(self.filters)
                 except FieldError as e:
                     self.exception = e
@@ -84,21 +92,23 @@
             self.exception = e
             self.error_message = str(e.message)
 
         return queryset
 
     @property
     def media(self):
-        extra = '' if settings.DEBUG else '.min'
+        extra = "" if settings.DEBUG else ".min"
         i18n_name = SELECT2_TRANSLATIONS.get(get_language())
-        i18n_file = ('admin/js/vendor/select2/i18n/%s.js' % i18n_name,) if i18n_name else ()
+        i18n_file = (
+            ("admin/js/vendor/select2/i18n/%s.js" % i18n_name,) if i18n_name else ()
+        )
         return forms.Media(
-            js=('admin/js/vendor/jquery/jquery%s.js' % extra,
-                ) + i18n_file + ('admin/js/jquery.init.js',
-                                 'adminfilters/dj%s.js' % extra,
-                                 ),
+            js=("admin/js/vendor/jquery/jquery%s.js" % extra,)
+            + i18n_file
+            + (
+                "admin/js/jquery.init.js",
+                "adminfilters/dj%s.js" % extra,
+            ),
             css={
-                'screen': (
-                    'adminfilters/adminfilters.css',
-                ),
+                "screen": ("adminfilters/adminfilters.css",),
             },
         )
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/filters.py` & `django-adminfilters-2.2.0/src/adminfilters/filters.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,13 +1,11 @@
 from .autocomplete import AutoCompleteFilter
 from .checkbox import RelatedFieldCheckBoxFilter
-from .combo import (AllValuesComboFilter, ChoicesFieldComboFilter,
-                    RelatedFieldComboFilter,)
+from .combo import AllValuesComboFilter, ChoicesFieldComboFilter, RelatedFieldComboFilter
 from .dj import DjangoLookupFilter
 from .extra import PermissionPrefixFilter
 from .json import JsonFieldFilter
 from .multiselect import IntersectionFieldListFilter, UnionFieldListFilter
 from .numbers import MaxMinFilter, NumberFilter
 from .querystring import QueryStringFilter
-from .radio import (AllValuesRadioFilter, BooleanRadioFilter,
-                    ChoicesFieldRadioFilter, RelatedFieldRadioFilter,)
+from .radio import AllValuesRadioFilter, BooleanRadioFilter, ChoicesFieldRadioFilter, RelatedFieldRadioFilter
 from .value import MultiValueFilter, ValueFilter
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/json.py` & `django-adminfilters-2.2.0/src/adminfilters/json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,98 +1,111 @@
 from django import forms
 from django.conf import settings
 from django.contrib.admin.widgets import SELECT2_TRANSLATIONS
 from django.db.models import Q
-from django.utils.translation import get_language, gettext as _
+from django.utils.translation import get_language
+from django.utils.translation import gettext as _
 
 from .mixin import MediaDefinitionFilter, SmartFieldListFilter
 
 
 class JsonFieldFilter(MediaDefinitionFilter, SmartFieldListFilter):
     parameter_name = None
     title = None
-    template = 'adminfilters/json.html'
+    template = "adminfilters/json.html"
     can_negate = True
     negated = False
     options = True
-    key_placeholder = _('JSON key')
-    placeholder = _('JSON value')
+    key_placeholder = _("JSON key")
+    placeholder = _("JSON value")
 
     def __init__(self, field, request, params, model, model_admin, field_path):
-        self.lookup_kwarg_key = '%s__key' % field_path
-        self.lookup_kwarg_value = '%s__value' % field_path
-        self.lookup_kwarg_negated = '%s__negate' % field_path
-        self.lookup_kwarg_options = '%s__options' % field_path
-        self.lookup_kwarg_type = '%s__type' % field_path
-        self.lookup_key_val = params.get(self.lookup_kwarg_key, '')
-        self.lookup_value_val = params.get(self.lookup_kwarg_value, '')
-        self.lookup_negated_val = params.get(self.lookup_kwarg_negated, 'false')
-        self.lookup_options_val = params.get(self.lookup_kwarg_options, 'e')
-        self.lookup_type_val = params.get(self.lookup_kwarg_type, 'any')
+        self.lookup_kwarg_key = "%s__key" % field_path
+        self.lookup_kwarg_value = "%s__value" % field_path
+        self.lookup_kwarg_negated = "%s__negate" % field_path
+        self.lookup_kwarg_options = "%s__options" % field_path
+        self.lookup_kwarg_type = "%s__type" % field_path
+        self.lookup_key_val = params.get(self.lookup_kwarg_key, "")
+        self.lookup_value_val = params.get(self.lookup_kwarg_value, "")
+        self.lookup_negated_val = params.get(self.lookup_kwarg_negated, "false")
+        self.lookup_options_val = params.get(self.lookup_kwarg_options, "e")
+        self.lookup_type_val = params.get(self.lookup_kwarg_type, "any")
 
         self.field = field
         self.query_string = None
         self.field_path = field_path
-        self.title = getattr(field, 'verbose_name', field_path)
+        self.title = getattr(field, "verbose_name", field_path)
         super().__init__(field, request, params, model, model_admin, field_path)
 
     @classmethod
     def factory(cls, **kwargs):
-        return type('JsonFieldFilter', (cls,), kwargs)
+        return type("JsonFieldFilter", (cls,), kwargs)
 
     def expected_parameters(self):
-        return [self.lookup_kwarg_key,
-                self.lookup_kwarg_value,
-                self.lookup_kwarg_negated, self.lookup_kwarg_options, self.lookup_kwarg_type]
+        return [
+            self.lookup_kwarg_key,
+            self.lookup_kwarg_value,
+            self.lookup_kwarg_negated,
+            self.lookup_kwarg_options,
+            self.lookup_kwarg_type,
+        ]
 
     def value(self):
         return [
             self.lookup_key_val,
             self.lookup_value_val,
             self.lookup_options_val,
-            (self.can_negate and self.lookup_negated_val == 'true') or self.negated,
+            (self.can_negate and self.lookup_negated_val == "true") or self.negated,
             self.lookup_type_val,
         ]
 
     def choices(self, changelist):
-        self.query_string = changelist.get_query_string(remove=self.expected_parameters())
+        self.query_string = changelist.get_query_string(
+            remove=self.expected_parameters()
+        )
         return []
 
     def queryset(self, request, queryset):
         key, value, options, negated, type_ = self.value()
         if key:
-            if type_ == 'any' and value.isnumeric():
-                filters = Q(**{f'{self.field_path}__{key}': value}) | Q(**{f'{self.field_path}__{key}': int(value)})
-            elif type_ == 'num' and value.isnumeric():
-                filters = Q(**{f'{self.field_path}__{key}': float(value)})
+            if type_ == "any" and value.isnumeric():
+                filters = Q(**{f"{self.field_path}__{key}": value}) | Q(
+                    **{f"{self.field_path}__{key}": int(value)}
+                )
+            elif type_ == "num" and value.isnumeric():
+                filters = Q(**{f"{self.field_path}__{key}": float(value)})
             else:  # type_ == 'str':
-                filters = Q(**{f'{self.field_path}__{key}': str(value)})
+                filters = Q(**{f"{self.field_path}__{key}": str(value)})
 
             if negated:
-                if self.options and options == 'e':
+                if self.options and options == "e":
                     filters = ~filters
                 else:
-                    filters = Q(**{f'{self.field_path}__{key}__isnull': True}) | ~filters
+                    filters = (
+                        Q(**{f"{self.field_path}__{key}__isnull": True}) | ~filters
+                    )
             else:
-                if options == 'i':
-                    filters = filters | Q(**{f'{self.field_path}__{key}__isnull': True})
+                if options == "i":
+                    filters = filters | Q(**{f"{self.field_path}__{key}__isnull": True})
 
             queryset = queryset.filter(filters)
 
         return queryset
 
     @property
     def media(self):
-        extra = '' if settings.DEBUG else '.min'
+        extra = "" if settings.DEBUG else ".min"
         i18n_name = SELECT2_TRANSLATIONS.get(get_language())
-        i18n_file = ('admin/js/vendor/select2/i18n/%s.js' % i18n_name,) if i18n_name else ()
+        i18n_file = (
+            ("admin/js/vendor/select2/i18n/%s.js" % i18n_name,) if i18n_name else ()
+        )
         return forms.Media(
-            js=('admin/js/vendor/jquery/jquery%s.js' % extra,
-                ) + i18n_file + ('admin/js/jquery.init.js',
-                                 'adminfilters/jsonfilter%s.js' % extra,
-                                 ),
+            js=("admin/js/vendor/jquery/jquery%s.js" % extra,)
+            + i18n_file
+            + (
+                "admin/js/jquery.init.js",
+                "adminfilters/jsonfilter%s.js" % extra,
+            ),
             css={
-                'screen': (
-                    'adminfilters/adminfilters.css',
-                ),
+                "screen": ("adminfilters/adminfilters.css",),
             },
         )
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/mixin.py` & `django-adminfilters-2.2.0/src/adminfilters/mixin.py`

 * *Files 9% similar despite different names*

```diff
@@ -4,38 +4,45 @@
 
 
 class WrappperMixin:
     negated = False
     can_negate = False
     title = None
     negated_title = None
-    placeholder = ''
+    placeholder = ""
 
     def __init__(self, *args, **kwargs) -> None:
         self.error = None
         self.error_message = None
         super().__init__(*args, **kwargs)
-        if hasattr(self, 'media') and self.model_admin and not isinstance(self.model_admin, AdminFiltersMixin):
-            raise Exception(f'{self.model_admin.__class__.__name__} must inherit from AdminFiltersMixin')
+        if (
+            hasattr(self, "media")
+            and self.model_admin
+            and not isinstance(self.model_admin, AdminFiltersMixin)
+        ):
+            raise Exception(
+                f"{self.model_admin.__class__.__name__} must inherit from AdminFiltersMixin"
+            )
 
     def html_attrs(self):
-        classes = f'adminfilters box {self.__class__.__name__.lower()}'
+        classes = f"adminfilters box {self.__class__.__name__.lower()}"
         if self.error_message:
-            classes += ' error'
+            classes += " error"
 
-        return {'class': classes,
-                'id': '_'.join(self.expected_parameters()),
-                }
+        return {
+            "class": classes,
+            "id": "_".join(self.expected_parameters()),
+        }
 
     def get_title(self):
         if not self.can_negate and self.negated:
             if self.negated_title:
                 return self.negated_title
             else:
-                return f'not {self.title}'
+                return f"not {self.title}"
         return self.title
 
 
 class SmartListFilter(WrappperMixin, ListFilter):
     def __init__(self, request, params, model, model_admin):
         self.model_admin = model_admin
         super().__init__(request, params, model, model_admin)
@@ -48,25 +55,24 @@
 
 
 class MediaDefinitionFilter:
     pass
 
 
 class AdminFiltersMixin(ModelAdmin):
-
     def get_changelist_instance(self, request):
         cl = super().get_changelist_instance(request)
         for flt in cl.filter_specs:
-            if hasattr(flt, 'media'):
+            if hasattr(flt, "media"):
                 self.admin_filters_media += flt.media
         return cl
 
     def __init__(self, model, admin_site):
         self.admin_filters_media = forms.Media()
         super().__init__(model, admin_site)
 
     @property
     def media(self):
         original = super().media
-        if hasattr(self, 'admin_filters_media'):
+        if hasattr(self, "admin_filters_media"):
             original += self.admin_filters_media
         return original
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/multiselect.py` & `django-adminfilters-2.2.0/src/adminfilters/multiselect.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,91 +2,88 @@
 from django.db.models.fields import AutoField, BigAutoField, IntegerField
 from django.utils.translation import gettext_lazy as _
 
 from adminfilters.mixin import SmartFieldListFilter
 
 
 class MultipleSelectFieldListFilter(SmartFieldListFilter):
-
     def __init__(self, field, request, params, model, model_admin, field_path):
-        self.lookup_kwarg = '%s_filter' % field_path
-        self.filter_statement = '%s' % field_path
+        self.lookup_kwarg = "%s_filter" % field_path
+        self.filter_statement = "%s" % field_path
         self.lookup_val = params.pop(self.lookup_kwarg, None)
         self.lookup_choices = field.get_choices(include_blank=False)
         super().__init__(field, request, params, model, model_admin, field_path)
-        self.used_parameters[self.lookup_kwarg] = prepare_lookup_value(self.lookup_kwarg,
-                                                                       self.lookup_val)
+        self.used_parameters[self.lookup_kwarg] = prepare_lookup_value(
+            self.lookup_kwarg, self.lookup_val
+        )
 
     def expected_parameters(self):
         return [self.lookup_kwarg]
 
     def get_field(self):
         return self.field.remote_field.model._meta.pk
 
     def values(self):
         """
         Returns a list of values to filter on.
         """
         values = []
         value = self.used_parameters.get(self.lookup_kwarg, None)
         if value:
-            values = value.split(',')
+            values = value.split(",")
 
         field = self.get_field()
         # convert to integers if IntegerField
         if type(field) in [IntegerField, AutoField, BigAutoField]:
             values = [int(x) for x in values]
         return values
 
     def queryset(self, request, queryset):
         raise NotImplementedError
 
     def choices(self, cl):
         # from django.contrib.admin.views.main import EMPTY_CHANGELIST_VALUE
         yield {
-            'selected': self.lookup_val is None,
-            'query_string': cl.get_query_string(
-                {},
-                [self.lookup_kwarg]),
-            'display': _('All')
+            "selected": self.lookup_val is None,
+            "query_string": cl.get_query_string({}, [self.lookup_kwarg]),
+            "display": _("All"),
         }
         for pk_val, val in self.lookup_choices:
             selected = pk_val in self.values()
             pk_list = set(self.values())
             if selected:
                 pk_list.remove(pk_val)
             else:
                 pk_list.add(pk_val)
-            queryset_value = ','.join([str(x) for x in pk_list])
+            queryset_value = ",".join([str(x) for x in pk_list])
             if pk_list:
                 query_string = cl.get_query_string(
                     {
                         self.lookup_kwarg: queryset_value,
-                    })
+                    }
+                )
             else:
                 query_string = cl.get_query_string({}, [self.lookup_kwarg])
             yield {
-                'selected': selected,
-                'query_string': query_string,
-                'display': val,
+                "selected": selected,
+                "query_string": query_string,
+                "display": val,
             }
 
 
 class IntersectionFieldListFilter(MultipleSelectFieldListFilter):
     """
     A FieldListFilter which allows multiple selection of
     filters for many-to-many type fields. A list of objects will be
     returned whose m2m contains all the selected filters.
     """
 
     def queryset(self, request, queryset):
         for value in self.values():
-            filter_dct = {
-                self.filter_statement: value
-            }
+            filter_dct = {self.filter_statement: value}
             queryset = queryset.filter(**filter_dct)
         return queryset
 
 
 class UnionFieldListFilter(MultipleSelectFieldListFilter):
     """
     A FieldListFilter which allows multiple selection of
@@ -95,23 +92,22 @@
     contains one of the selected filters.
     """
 
     def get_field(self):
         try:
             field = super().get_field()
         except AttributeError:  # pragma: no cover
-            if hasattr(self.field, 'choices') and self.field.choices:
+            if hasattr(self.field, "choices") and self.field.choices:
                 field = self.field  # It's a *Field with choises
             else:
                 raise AttributeError(
-                    'Multiselect field must be a FK or any type with choices')
+                    "Multiselect field must be a FK or any type with choices"
+                )
         return field
 
     def queryset(self, request, queryset):
         filter_values = self.values()
         if filter_values:
-            filter_statement = '%s__in' % self.filter_statement
-            filter_dct = {
-                filter_statement: filter_values
-            }
+            filter_statement = "%s__in" % self.filter_statement
+            filter_dct = {filter_statement: filter_values}
             queryset = queryset.filter(**filter_dct).distinct()
         return queryset
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/numbers.py` & `django-adminfilters-2.2.0/src/adminfilters/numbers.py`

 * *Files 13% similar despite different names*

```diff
@@ -2,75 +2,80 @@
 
 from django.contrib.admin.options import IncorrectLookupParameters
 
 from .value import ValueFilter
 
 
 class NumberFilter(ValueFilter):
-    rex1 = re.compile(r'^(>=|<=|>|<|=)?([-+]?[0-9]+)$')
-    re_range = re.compile(r'^(\d+)\.{2,}(\d+)$')
-    re_list = re.compile(r'(\d+),?')
-    re_unlike = re.compile(r'^(<>)([-+]?[0-9]+)$')
-    map = {'>=': 'gte',
-           '<=': 'lte',
-           '>': 'gt',
-           '<': 'lt',
-           '=': 'exact',
-           '<>': 'not',
-           }
+    rex1 = re.compile(r"^(>=|<=|>|<|=)?([-+]?[0-9]+)$")
+    re_range = re.compile(r"^(\d+)\.{2,}(\d+)$")
+    re_list = re.compile(r"(\d+),?")
+    re_unlike = re.compile(r"^(<>)([-+]?[0-9]+)$")
+    map = {
+        ">=": "gte",
+        "<=": "lte",
+        ">": "gt",
+        "<": "lt",
+        "=": "exact",
+        "<>": "not",
+    }
     can_negate = False
 
     # def __init__(self, field, request, params, model, model_admin, field_path):
     #     super().__init__(field, request, params, model, model_admin, field_path)
     #     self.lookup_kwarg = '%s__%s' % (field_path, self.lookup_name)
 
     @classmethod
     def factory(cls, *, title=None, **kwargs):
-        if 'lookup_name' in kwargs:
-            raise ValueError(f"'lookup_name' is not a valid value for "
-                             f"'{cls.__class__.__name__}.factory'")
+        if "lookup_name" in kwargs:
+            raise ValueError(
+                f"'lookup_name' is not a valid value for "
+                f"'{cls.__class__.__name__}.factory'"
+            )
         return super().factory(title=title, **kwargs)
 
     def placeholder(self):
-        return '1 or >< <=> <> 1 or 1..10 or 1,4,5'
+        return "1 or >< <=> <> 1 or 1..10 or 1,4,5"
 
     # def parse_query_string(self, params):
     #     self.lookup_val = params.get(self.field.name, '')
     def expected_parameters(self):
         self.lookup_kwarg = self.field_path
         return [self.lookup_kwarg]
 
     def value(self):
         return [
-            self.parameters.get(self.lookup_kwarg, ''),
+            self.parameters.get(self.lookup_kwarg, ""),
         ]
 
     def queryset(self, request, queryset):
         if self.value() and self.value()[0]:
             raw_value = self.value()[0]
             m1 = self.rex1.match(raw_value)
             m_range = self.re_range.match(raw_value)
             m_list = self.re_list.match(raw_value)
             m_unlike = self.re_unlike.match(raw_value)
             if m_unlike and m_unlike.groups():
-                match = '%s__exact' % self.field.name
+                match = "%s__exact" % self.field.name
                 op, value = self.re_unlike.match(raw_value).groups()
                 queryset = queryset.exclude(**{match: value})
             else:
                 if m1 and m1.groups():
                     op, value = self.rex1.match(raw_value).groups()
-                    match = '%s__%s' % (self.field.name, self.map[op or '='])
+                    match = "%s__%s" % (self.field.name, self.map[op or "="])
                     self.filters = {match: value}
                 elif m_range and m_range.groups():
                     start, end = self.re_range.match(raw_value).groups()
-                    self.filters = {f'{self.field.name}__gte': start,
-                                    f'{self.field.name}__lte': end}
+                    self.filters = {
+                        f"{self.field.name}__gte": start,
+                        f"{self.field.name}__lte": end,
+                    }
                 elif m_list and m_list.groups():
-                    value = raw_value.split(',')
-                    match = '%s__in' % self.field.name
+                    value = raw_value.split(",")
+                    match = "%s__in" % self.field.name
                     self.filters = {match: value}
                 # elif m_unlike and m_unlike.groups():
                 #     match = '%s__exact' % self.field.name
                 #     op, value = self.re_unlike.match(raw).groups()
                 #     queryset = queryset.exclude(**{match: value})
                 else:  # pragma: no cover
                     raise IncorrectLookupParameters()
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/querystring.py` & `django-adminfilters-2.2.0/src/adminfilters/querystring.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,118 +1,136 @@
 import logging
 from urllib import parse
 
 from django import forms
 from django.conf import settings
 from django.contrib.admin.widgets import SELECT2_TRANSLATIONS
 from django.core.exceptions import FieldError, ValidationError
-from django.utils.translation import get_language, gettext as _
+from django.utils.translation import get_language
+from django.utils.translation import gettext as _
 
 from .mixin import MediaDefinitionFilter, SmartListFilter
 from .utils import cast_value, get_field_type, get_message_from_exception
 
 logger = logging.getLogger(__name__)
 
 
 class QueryStringFilter(MediaDefinitionFilter, SmartListFilter):
-    parameter_name = 'qs'
-    title = 'QueryString'
-    template = 'adminfilters/querystring.html'
+    parameter_name = "qs"
+    title = "QueryString"
+    template = "adminfilters/querystring.html"
     can_negate = True
     negated = False
     options = True
-    separator = ','
-    placeholder = _('django db lookup values')
+    separator = ","
+    placeholder = _("django db lookup values")
 
     def __init__(self, request, params, model, model_admin):
-        self.parameter_name_negated = '%s__negate' % self.parameter_name
-        self.lookup_field_val = params.pop(self.parameter_name, '')
-        self.lookup_negated_val = params.pop(self.parameter_name_negated, 'false')
+        self.parameter_name_negated = "%s__negate" % self.parameter_name
+        self.lookup_field_val = params.pop(self.parameter_name, "")
+        self.lookup_negated_val = params.pop(self.parameter_name_negated, "false")
         self.query_string = None
         self.error_message = None
         self.exception = None
         self.filters = None
         self.exclude = None
         self.model_admin = model_admin
         self.model = model
         self.validation_errors = {}
         self.filters = {}
         self.exclude = {}
         super().__init__(request, params, model, model_admin)
 
     @classmethod
     def factory(cls, **kwargs):
-        return type('QueryStringFilter', (cls,), kwargs)
+        return type("QueryStringFilter", (cls,), kwargs)
 
     def expected_parameters(self):
-        return [self.parameter_name,
-                self.parameter_name_negated]
+        return [self.parameter_name, self.parameter_name_negated]
 
     def has_output(self):
         return True
 
     def value(self):
         return [
             self.lookup_field_val,
-            (self.can_negate and self.lookup_negated_val == 'true') or self.negated,
+            (self.can_negate and self.lookup_negated_val == "true") or self.negated,
         ]
 
     def choices(self, changelist):
-        self.query_string = changelist.get_query_string(remove=self.expected_parameters())
+        self.query_string = changelist.get_query_string(
+            remove=self.expected_parameters()
+        )
         return []
 
     def get_filters(self, value):
-        query_params = dict(parse.parse_qsl('&'.join(value.splitlines())))
+        query_params = dict(parse.parse_qsl("&".join(value.splitlines())))
         exclude = {}
         filters = {}
         for field_name, raw_value in query_params.items():
             target = filters
-            if field_name[0] == '!':
+            cast = None
+
+            if field_name[0] == "!":
                 field_name = field_name[1:]
                 target = exclude
+
+            if field_name[0] == "#":
+                field_name = field_name[1:]
+                cast = int
+            elif field_name[0] == ".":
+                field_name = field_name[1:]
+                cast = float
+
             field, lookup, field_type = get_field_type(self.model, field_name)
-            value = cast_value(raw_value, field, lookup)
+            value = cast_value(raw_value, field, lookup, force=cast)
             target[field_name] = value
 
         return filters, exclude
 
     def queryset(self, request, queryset):
         value, negated = self.value()
         if value:
             try:
                 self.filters, self.exclude = self.get_filters(value)
                 if not (self.filters or self.exclude):
-                    self.error_message = _('Invalid django filter')
+                    self.error_message = _("Invalid django filter")
                 else:
                     if negated:
-                        queryset = queryset.filter(**self.exclude).exclude(**self.filters)
+                        queryset = queryset.filter(**self.exclude).exclude(
+                            **self.filters
+                        )
                     else:
-                        queryset = queryset.filter(**self.filters).exclude(**self.exclude)
+                        queryset = queryset.filter(**self.filters).exclude(
+                            **self.exclude
+                        )
             except FieldError as e:
                 self.error_message = get_message_from_exception(e)
             except ValidationError as e:  # pragma: no cover
-                self.error_message = ', '.join(e.messages)
+                self.error_message = ", ".join(e.messages)
             except Exception as e:  # pragma: no cover
                 logger.exception(e)
                 if settings.DEBUG:
-                    self.error_message = f'{e.__class__.__name__}: {e}'
+                    self.error_message = f"{e.__class__.__name__}: {e}"
                 else:
                     logger.exception(e)
-                    self.error_message = 'Invalid filter'
+                    self.error_message = "Invalid filter"
         return queryset
 
     @property
     def media(self):
-        extra = '' if settings.DEBUG else '.min'
+        extra = "" if settings.DEBUG else ".min"
         i18n_name = SELECT2_TRANSLATIONS.get(get_language())
-        i18n_file = ('admin/js/vendor/select2/i18n/%s.js' % i18n_name,) if i18n_name else ()
+        i18n_file = (
+            ("admin/js/vendor/select2/i18n/%s.js" % i18n_name,) if i18n_name else ()
+        )
         return forms.Media(
-            js=('admin/js/vendor/jquery/jquery%s.js' % extra,
-                ) + i18n_file + ('admin/js/jquery.init.js',
-                                 'adminfilters/querystring%s.js' % extra,
-                                 ),
+            js=("admin/js/vendor/jquery/jquery%s.js" % extra,)
+            + i18n_file
+            + (
+                "admin/js/jquery.init.js",
+                "adminfilters/querystring%s.js" % extra,
+            ),
             css={
-                'screen': (
-                    'adminfilters/adminfilters.css',
-                ),
+                "screen": ("adminfilters/adminfilters.css",),
             },
         )
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/radio.py` & `django-adminfilters-2.2.0/src/adminfilters/radio.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,22 +1,24 @@
-from django.contrib.admin.filters import (AllValuesFieldListFilter,
-                                          BooleanFieldListFilter,
-                                          ChoicesFieldListFilter,
-                                          RelatedFieldListFilter,)
+from django.contrib.admin.filters import (
+    AllValuesFieldListFilter,
+    BooleanFieldListFilter,
+    ChoicesFieldListFilter,
+    RelatedFieldListFilter,
+)
 
 from .mixin import WrappperMixin
 
 
 class AllValuesRadioFilter(WrappperMixin, AllValuesFieldListFilter):
-    template = 'adminfilters/radio.html'
+    template = "adminfilters/radio.html"
 
 
 class RelatedFieldRadioFilter(WrappperMixin, RelatedFieldListFilter):
-    template = 'adminfilters/radio.html'
+    template = "adminfilters/radio.html"
 
 
 class ChoicesFieldRadioFilter(WrappperMixin, ChoicesFieldListFilter):
-    template = 'adminfilters/radio.html'
+    template = "adminfilters/radio.html"
 
 
 class BooleanRadioFilter(WrappperMixin, BooleanFieldListFilter):
-    template = 'adminfilters/radio.html'
+    template = "adminfilters/radio.html"
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/adminfilters.css` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/adminfilters.css`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/depot.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/depot.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/depot.min.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/depot.min.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/dj.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/dj.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/dj.min.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/dj.min.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/jsonfilter.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/jsonfilter.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/jsonfilter.min.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/jsonfilter.min.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/querystring.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/querystring.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/querystring.min.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/querystring.min.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/value.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/value.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/static/adminfilters/value.min.js` & `django-adminfilters-2.2.0/src/adminfilters/static/adminfilters/value.min.js`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/autocomplete.html` & `django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/autocomplete.html`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/checkbox.html` & `django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/checkbox.html`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/dj.html` & `django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/dj.html`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/json.html` & `django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/json.html`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/querystring.html` & `django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/querystring.html`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/radio.html` & `django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/radio.html`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/value.html` & `django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/value.html`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/templates/adminfilters/value_multi.html` & `django-adminfilters-2.2.0/src/adminfilters/templates/adminfilters/value_multi.html`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/src/adminfilters/utils.py` & `django-adminfilters-2.2.0/src/adminfilters/utils.py`

 * *Files 10% similar despite different names*

```diff
@@ -8,26 +8,26 @@
 
 logger = logging.getLogger(__name__)
 
 rex = re.compile("'.*'")
 
 
 def parse_bool(value):
-    if str(value).lower() in ['true', '1', 'yes', 't', 'y']:
+    if str(value).lower() in ["true", "1", "yes", "t", "y"]:
         return True
-    elif str(value).lower() in ['false', '0', 'no', 'f', 'n']:
+    elif str(value).lower() in ["false", "0", "no", "f", "n"]:
         return False
     return value
 
 
 def get_message_from_exception(e: FieldError):
     message = str(e)
-    fieldname = rex.findall(message) or ['']
-    if 'Unsupported lookup' in message:
-        return f'Unsupported lookup: {fieldname[0]}'
+    fieldname = rex.findall(message) or [""]
+    if "Unsupported lookup" in message:
+        return f"Unsupported lookup: {fieldname[0]}"
     else:
         return message
 
 
 def get_query_string(request, new_params=None, remove=None):
     if new_params is None:
         new_params = {}
@@ -40,31 +40,39 @@
                 del p[k]
     for k, v in new_params.items():
         if v is None:
             if k in p:
                 del p[k]
         else:
             p[k] = v
-    return '?%s' % urlencode(sorted(p.items()))
+    return "?%s" % urlencode(sorted(p.items()))
 
 
 def get_field_by_name(model, name):
     field = model._meta.get_field(name)
     direct = not field.auto_created or field.concrete
     return field, field.model, direct, field.many_to_many
 
 
 def get_all_field_names(model):
     from itertools import chain
+
     if not model:
         raise ValueError("'model' must be a Model instance")
-    return list(set(chain.from_iterable((field.name, field.attname)
-                                        if hasattr(field, 'attname') else (field.name,)
-                                        for field in model._meta.get_fields()
-                                        if not (field.many_to_one and field.related_model is None))))
+    return list(
+        set(
+            chain.from_iterable(
+                (field.name, field.attname)
+                if hasattr(field, "attname")
+                else (field.name,)
+                for field in model._meta.get_fields()
+                if not (field.many_to_one and field.related_model is None)
+            )
+        )
+    )
 
 
 def get_field_by_path(model, field_path):
     """
     get a Model class or instance and a path to a attribute, returns the field object
 
     :param model: :class:`django.db.models.Model`
@@ -77,56 +85,69 @@
     >>> p = Permission(name='perm')
     >>> get_field_by_path(Permission, 'content_type').name
     'content_type'
     >>> p = Permission(name='perm')
     >>> get_field_by_path(p, 'content_type.app_label').name
     'app_label'
     """
-    parts = field_path.split('.')
+    parts = field_path.split(".")
     target = parts[0]
     if not model:
         raise ValueError("'model' must be a Model instance")
 
     if target in get_all_field_names(model):
         field_object, model, direct, m2m = get_field_by_name(model, target)
         if isinstance(field_object, models.ForeignKey):
             if parts[1:]:
                 while True:
                     if field_object.related_model is None:
                         break
-                    fk = get_field_by_path(field_object.related_model, '.'.join(parts[1:]))
+                    fk = get_field_by_path(
+                        field_object.related_model, ".".join(parts[1:])
+                    )
                     if fk is None:
                         break
                     field_object = fk
                 return field_object
             else:
                 return field_object
         else:
             return field_object
     return None
 
 
 def get_field_type(model, field_path):
-    lookup = 'exact'
+    lookup = "exact"
     try:
-        parts = field_path.split('__')
-        field = get_field_by_path(model, '.'.join(parts))
+        parts = field_path.split("__")
+        field = get_field_by_path(model, ".".join(parts))
         if not field:
             raise ValidationError(f"Unknown field '{field_path}'")
         if field.name != parts[-1]:
             lookup = parts[-1]
         field_type = field.get_internal_type()
     except Exception:
         raise
     return field, lookup, field_type
 
 
-def cast_value(v, fld, lookup):
-    if isinstance(fld, (BooleanField,)) or lookup in ['isnull']:
+def cast_value(v, fld, lookup, force=None):
+    if force:
+        func = force
+    elif isinstance(fld, (BooleanField,)) or lookup in ["isnull"]:
         func = parse_bool
-    elif isinstance(fld, (DateField, DateTimeField,)) and lookup:
+    elif (
+        isinstance(
+            fld,
+            (
+                DateField,
+                DateTimeField,
+            ),
+        )
+        and lookup
+    ):
         return v
     else:
         func = fld.to_python
-    if lookup in ['in']:
-        return [func(e) for e in v.split(',')]
+    if lookup in ["in"]:
+        return [func(e) for e in v.split(",")]
     return func(v)
```

### Comparing `django-adminfilters-2.1.0/src/adminfilters/value.py` & `django-adminfilters-2.2.0/src/adminfilters/value.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,24 +1,24 @@
-
 import json
 
 from django import forms
 from django.conf import settings
 from django.contrib import messages
 from django.contrib.admin.widgets import SELECT2_TRANSLATIONS
-from django.utils.translation import get_language, gettext as _
+from django.utils.translation import get_language
+from django.utils.translation import gettext as _
 
 from adminfilters.mixin import MediaDefinitionFilter, SmartFieldListFilter
 
 
 class ValueFilter(MediaDefinitionFilter, SmartFieldListFilter):
-    template = 'adminfilters/value.html'
+    template = "adminfilters/value.html"
     toggleable = False
     filter_title = None
-    lookup_name = 'exact'
+    lookup_name = "exact"
     button = True
     can_negate = True
     negated = False
 
     def __init__(self, field, request, params, model, model_admin, field_path):
         # self.lookup_negated_val = None
         # self.model = model
@@ -41,45 +41,45 @@
         # self.query_string = get_query_string(request, remove=self.expected_parameters())
 
         # self.params = params
         # self.query_values = []
         # self.operator = '+'
 
     def expected_parameters(self):
-        self.lookup_kwarg = '%s__%s' % (self.field_path, self.lookup_name)
-        self.lookup_kwarg_negated = '%s__negate' % self.lookup_kwarg
+        self.lookup_kwarg = "%s__%s" % (self.field_path, self.lookup_name)
+        self.lookup_kwarg_negated = "%s__negate" % self.lookup_kwarg
         return [self.lookup_kwarg, self.lookup_kwarg_negated]
 
     def value(self):
         return [
-            self.parameters.get(self.lookup_kwarg, ''),
-            self.parameters.get(self.lookup_kwarg_negated, '') == 'true'
+            self.parameters.get(self.lookup_kwarg, ""),
+            self.parameters.get(self.lookup_kwarg_negated, "") == "true"
             # self.parameters[self.lookup_kwarg],
             # self.parameters[self.lookup_kwarg_negated] == 'true'
             # self.lookup_val,
             # self.lookup_negated_val == 'true'
         ]
 
     def js_options(self):
-        return json.dumps(dict(button=self.button,
-                               canNegate=self.can_negate,
-                               negated=self.negated))
+        return json.dumps(
+            dict(button=self.button, canNegate=self.can_negate, negated=self.negated)
+        )
 
     def _get_title(self):
         if self.filter_title:
             return self.filter_title
-        elif '__' in self.field_path:
-            return self.field_path.replace('__', '->')
-        return getattr(self.field, 'verbose_name', self.field_path)
+        elif "__" in self.field_path:
+            return self.field_path.replace("__", "->")
+        return getattr(self.field, "verbose_name", self.field_path)
 
     @classmethod
-    def factory(cls, *, title=None, lookup_name='exact', **kwargs):
-        kwargs['filter_title'] = title
-        kwargs['lookup_name'] = lookup_name
-        return type('ValueFilter', (cls,), kwargs)
+    def factory(cls, *, title=None, lookup_name="exact", **kwargs):
+        kwargs["filter_title"] = title
+        kwargs["lookup_name"] = lookup_name
+        return type("ValueFilter", (cls,), kwargs)
 
     # def parse_query_string(self, params):
     #     self.lookup_negated_val = params.get(self.lookup_kwarg_negated)
     #     self.lookup_val = params.get(self.lookup_kwarg, '')
 
     def queryset(self, request, queryset):
         target, exclude = self.value()
@@ -87,56 +87,57 @@
             try:
                 self.filters = {self.lookup_kwarg: target}
                 if exclude:
                     queryset = queryset.exclude(**self.filters)
                 else:
                     queryset = queryset.filter(**self.filters)
             except Exception as e:
-                msg = _('%s filter ignored due to an error %s') % (self.title, e)
+                msg = _("%s filter ignored due to an error %s") % (self.title, e)
                 self.model_admin.message_user(request, msg, messages.ERROR)
                 pass
         return queryset
 
     def choices(self, changelist):
-        self.query_string = changelist.get_query_string(remove=self.expected_parameters())
+        self.query_string = changelist.get_query_string(
+            remove=self.expected_parameters()
+        )
         return []
 
     @property
     def media(self):
-        extra = '' if settings.DEBUG else '.min'
+        extra = "" if settings.DEBUG else ".min"
         i18n_name = SELECT2_TRANSLATIONS.get(get_language())
-        i18n_file = ('admin/js/vendor/select2/i18n/%s.js' % i18n_name,) if i18n_name else ()
+        i18n_file = (
+            ("admin/js/vendor/select2/i18n/%s.js" % i18n_name,) if i18n_name else ()
+        )
         return forms.Media(
-            js=('admin/js/vendor/jquery/jquery%s.js' % extra,
-                ) + i18n_file + ('admin/js/jquery.init.js',
-                                 'adminfilters/value%s.js' % extra,
-                                 ),
+            js=("admin/js/vendor/jquery/jquery%s.js" % extra,)
+            + i18n_file
+            + (
+                "admin/js/jquery.init.js",
+                "adminfilters/value%s.js" % extra,
+            ),
             css={
-                'screen': (
-                    'adminfilters/adminfilters.css',
-                ),
+                "screen": ("adminfilters/adminfilters.css",),
             },
         )
 
 
 class MultiValueFilter(ValueFilter):
-    template = 'adminfilters/value_multi.html'
-    separator = ','
+    template = "adminfilters/value_multi.html"
+    separator = ","
     filter_title = None
-    lookup_name = 'in'
+    lookup_name = "in"
 
     def placeholder(self):
-        return _('comma separated list of values')
+        return _("comma separated list of values")
 
     def value(self):
         values = self.parameters.get(self.lookup_kwarg, None)
         if values is not None:
             values = values.split(self.separator)
-        return [
-            values,
-            self.parameters.get(self.lookup_kwarg_negated, '') == 'true'
-        ]
+        return [values, self.parameters.get(self.lookup_kwarg_negated, "") == "true"]
 
 
 TextFieldFilter = ValueFilter
 ForeignKeyFieldFilter = TextFieldFilter
 MultiValueTextFieldFilter = MultiValueFilter
```

### Comparing `django-adminfilters-2.1.0/src/django_adminfilters.egg-info/PKG-INFO` & `django-adminfilters-2.2.0/src/django_adminfilters.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-adminfilters
-Version: 2.1.0
+Version: 2.2.0
 Summary: Extra filters for django admin site
 Home-page: https://github.com/saxix/django-adminfilters
 Download-URL: https://github.com/saxix/django-adminfilters
 Author: sax
 Author-email: s.apostolico@gmail.com
 License: MIT
 Platform: any
@@ -48,14 +48,16 @@
   * AutocompleteFilter
 * Simple
   * ValueFilter
 * Combobox
   * AllValuesComboFilter
   * RelatedFieldComboFilter
   * ChoicesFieldComboFilter
+* Dates
+  * DateRangeFilter
 * Radio
   * AllValuesRadioFilter
   * RelatedFieldRadioFilter
   * ChoicesFieldRadioFilter
   * BooleanRadioFilter
 * Checkbox
   * RelatedFieldCheckBoxFilter
```

### Comparing `django-adminfilters-2.1.0/src/django_adminfilters.egg-info/SOURCES.txt` & `django-adminfilters-2.2.0/src/django_adminfilters.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -31,14 +31,15 @@
 src/adminfilters/depot/__init__.py
 src/adminfilters/depot/admin.py
 src/adminfilters/depot/apps.py
 src/adminfilters/depot/models.py
 src/adminfilters/depot/widget.py
 src/adminfilters/depot/migrations/0001_initial.py
 src/adminfilters/depot/migrations/0002_migration.py
+src/adminfilters/depot/migrations/0003_alter_storedfilter_id.py
 src/adminfilters/depot/migrations/__init__.py
 src/adminfilters/depot/templates/adminfilters/widget.html
 src/adminfilters/static/adminfilters/adminfilters.css
 src/adminfilters/static/adminfilters/autocomplete.js
 src/adminfilters/static/adminfilters/autocomplete.min.js
 src/adminfilters/static/adminfilters/depot.js
 src/adminfilters/static/adminfilters/depot.min.js
```

### Comparing `django-adminfilters-2.1.0/tests/.coveragerc` & `django-adminfilters-2.2.0/tests/.coveragerc`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/admin.py` & `django-adminfilters-2.2.0/tests/demoapp/demo/admin.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,107 +1,109 @@
 from django.contrib.admin import ModelAdmin
 from django.contrib.admin.views.main import ChangeList
 from django.contrib.auth.admin import UserAdmin
 
 from adminfilters.autocomplete import AutoCompleteFilter
 from adminfilters.combo import ChoicesFieldComboFilter
 from adminfilters.depot.widget import DepotManager
-from adminfilters.filters import (BooleanRadioFilter, DjangoLookupFilter,
-                                  IntersectionFieldListFilter, NumberFilter,
-                                  QueryStringFilter, RelatedFieldCheckBoxFilter,
-                                  RelatedFieldRadioFilter, UnionFieldListFilter,
-                                  ValueFilter,)
+from adminfilters.filters import (
+    BooleanRadioFilter,
+    DjangoLookupFilter,
+    IntersectionFieldListFilter,
+    NumberFilter,
+    QueryStringFilter,
+    RelatedFieldCheckBoxFilter,
+    RelatedFieldRadioFilter,
+    UnionFieldListFilter,
+    ValueFilter,
+)
 from adminfilters.json import JsonFieldFilter
 from adminfilters.mixin import AdminFiltersMixin
 from adminfilters.value import MultiValueFilter
 
 from .models import Artist, Band, Country
 
 
 class DebugChangeList(ChangeList):
     def get_queryset(self, request):
         try:
             return super().get_queryset(request)
         except Exception as e:
-            raise Exception(f'{e.__class__.__name__}: {e}')
+            raise Exception(f"{e.__class__.__name__}: {e}")
 
     def get_filters(self, request):
         try:
             return super().get_filters(request)
         except Exception as e:
-            raise Exception(f'{e.__class__.__name__}: {e}')
+            raise Exception(f"{e.__class__.__name__}: {e}")
 
 
 class DebugMixin:
     def get_changelist(self, request, **kwargs):
         return DebugChangeList
 
 
 class DemoModelAdmin_RelatedFieldCheckBoxFilter(DebugMixin, ModelAdmin):
     list_display = [f.name for f in Artist._meta.fields]
-    list_filter = (('bands', RelatedFieldCheckBoxFilter),
-                   )
-    search_fields = ('name',)
+    list_filter = (("bands", RelatedFieldCheckBoxFilter),)
+    search_fields = ("name",)
 
 
 class DemoModelAdmin_RelatedFieldRadioFilter(DebugMixin, ModelAdmin):
     list_display = [f.name for f in Artist._meta.fields]
-    list_filter = (('bands', RelatedFieldRadioFilter),)
-    search_fields = ('name',)
+    list_filter = (("bands", RelatedFieldRadioFilter),)
+    search_fields = ("name",)
 
 
 class DemoModelAdmin_UnionFieldListFilter(DebugMixin, ModelAdmin):
     list_display = [f.name for f in Artist._meta.fields]
-    list_filter = (('bands', UnionFieldListFilter),)
-    search_fields = ('name',)
+    list_filter = (("bands", UnionFieldListFilter),)
+    search_fields = ("name",)
 
 
 class DemoModelAdmin_IntersectionFieldListFilter(DebugMixin, ModelAdmin):
     list_display = [f.name for f in Artist._meta.fields]
-    list_filter = (('bands', IntersectionFieldListFilter),)
-    search_fields = ('name',)
+    list_filter = (("bands", IntersectionFieldListFilter),)
+    search_fields = ("name",)
 
 
 class DemoModelFieldAdmin(DebugMixin, AdminFiltersMixin, ModelAdmin):
-    list_display = ('char', 'integer', 'logic', 'email', 'choices', 'date')
+    list_display = ("char", "integer", "logic", "email", "choices", "date")
     list_filter = (
         QueryStringFilter,
-        ('choices', ChoicesFieldComboFilter),
-        ('integer', NumberFilter),
+        ("choices", ChoicesFieldComboFilter),
+        ("integer", NumberFilter),
     )
 
 
 class CountryModelAdmin(DebugMixin, ModelAdmin):
     list_display = [f.name for f in Country._meta.fields]
-    search_fields = ('name',)
+    search_fields = ("name",)
 
 
 class BandModelAdmin(DebugMixin, ModelAdmin):
     list_display = [f.name for f in Band._meta.fields]
-    search_fields = ('name',)
-    list_filter = ('genre',
-                   )
+    search_fields = ("name",)
+    list_filter = ("genre",)
 
 
 class ArtistModelAdmin(DebugMixin, AdminFiltersMixin, ModelAdmin):
     list_display = [f.name for f in Artist._meta.fields]
     list_filter = (
         DepotManager,
-        ('country', AutoCompleteFilter),
-        ('year_of_birth', NumberFilter),
-        ('bands__name', MultiValueFilter),
+        ("country", AutoCompleteFilter),
+        ("year_of_birth", NumberFilter),
+        ("bands__name", MultiValueFilter),
         QueryStringFilter,
         DjangoLookupFilter,
-        ('country__name', ValueFilter),
-        ('name', MultiValueFilter),
-        ('last_name', ValueFilter.factory(lookup_name='istartswith', title='LastName')),
-        ('flags', JsonFieldFilter.factory(can_negate=True, options=True)),
-        ('active', BooleanRadioFilter),
+        ("country__name", ValueFilter),
+        ("name", MultiValueFilter),
+        ("last_name", ValueFilter.factory(lookup_name="istartswith", title="LastName")),
+        ("flags", JsonFieldFilter.factory(can_negate=True, options=True)),
+        ("active", BooleanRadioFilter),
     )
-    search_fields = ('name',)
+    search_fields = ("name",)
 
 
 class IUserAdmin(DebugMixin, AdminFiltersMixin, UserAdmin):
-    list_display = ('username', 'email', 'first_name', 'last_name',
-                    'is_staff')
-    list_filter = (('username', ValueFilter.factory(lookup_name='istartswith')),
-                   )
+    list_display = ("username", "email", "first_name", "last_name", "is_staff")
+    list_filter = (("username", ValueFilter.factory(lookup_name="istartswith")),)
```

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/backends.py` & `django-adminfilters-2.2.0/tests/demoapp/demo/backends.py`

 * *Files 24% similar despite different names*

```diff
@@ -3,25 +3,34 @@
 
 
 class AnonymousAccessUserBackend(ModelBackend):
     supports_object_permissions = False
     supports_anonymous_user = True
 
     def get_all_permissions(self, user_obj, obj=None):
-        return Permission.objects.all().values_list('content_type__app_label', 'codename').order_by()
+        return (
+            Permission.objects.all()
+            .values_list("content_type__app_label", "codename")
+            .order_by()
+        )
 
     def get_group_permissions(self, user_obj, obj=None):
-        return Permission.objects.all().values_list('content_type__app_label', 'codename').order_by()
+        return (
+            Permission.objects.all()
+            .values_list("content_type__app_label", "codename")
+            .order_by()
+        )
 
     def has_perm(self, user_obj, perm, obj=None):
         return True
 
     def has_module_perms(self, user_obj, app_label):
         return True
 
+
 #
 # class AnyUserAuthBackend(ModelBackend):
 #     def authenticate(self, request, username=None, password=None, **kwargs):
 #         user, __ = User.objects.update_or_create(username=username,
 #                                                  defaults=dict(is_staff=True,
 #                                                  is_active=True,
 #                                                  is_superuser=True,
```

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/factories.py` & `django-adminfilters-2.2.0/tests/demoapp/demo/factories.py`

 * *Files 14% similar despite different names*

```diff
@@ -12,97 +12,102 @@
 class AutoRegisterFactoryMetaClass(FactoryMetaClass):
     def __new__(mcs, class_name, bases, attrs):
         new_class = super().__new__(mcs, class_name, bases, attrs)
         factories_registry[new_class._meta.model] = new_class
         return new_class
 
 
-class ModelFactory(factory.django.DjangoModelFactory, metaclass=AutoRegisterFactoryMetaClass):
+class ModelFactory(
+    factory.django.DjangoModelFactory, metaclass=AutoRegisterFactoryMetaClass
+):
     pass
 
 
 def get_flags():
     # Convert to plain ascii text
-    f = lambda: random.choice([
-        ('int', random.randint(1, 100)),
-        ('chr', chr(random.randrange(65, 90))),
-        ('int', '__'),
-        ('chr', ''),
-        ('chr', None),
-        ('int', None),
-        ('chr', '__'),
-    ])
+    f = lambda: random.choice(
+        [
+            ("int", random.randint(1, 100)),
+            ("chr", chr(random.randrange(65, 90))),
+            ("int", "__"),
+            ("chr", ""),
+            ("chr", None),
+            ("int", None),
+            ("chr", "__"),
+        ]
+    )
     value = f()
-    if value[1] == '__':
+    if value[1] == "__":
         base = {}
     else:
         base = dict([value])
     value = f()
-    if value[1] != '__':
+    if value[1] != "__":
         base.update(dict([value]))
     return base
 
 
 class DemoModelFieldFactory(ModelFactory):
-    char = factory.Faker('name')
-    integer = factory.Faker('pyint')
-    date = factory.Faker('date_this_decade')
-    datetime = factory.Faker('date_this_decade')
-    time = factory.Faker('time')
-    logic = factory.Faker('pybool')
-    decimal = factory.Faker('coordinate')
-    float = factory.Faker('pyfloat')
-    bigint = factory.Faker('pyint')
-    generic_ip = factory.Faker('ipv4')
+    char = factory.Faker("name")
+    integer = factory.Faker("pyint")
+    date = factory.Faker("date_this_decade")
+    datetime = factory.Faker("date_this_decade")
+    time = factory.Faker("time")
+    logic = factory.Faker("pybool")
+    decimal = factory.Faker("coordinate")
+    float = factory.Faker("pyfloat")
+    bigint = factory.Faker("pyint")
+    generic_ip = factory.Faker("ipv4")
     choices = factory.fuzzy.FuzzyChoice([1, 2, 3])
     unique = factory.Sequence(lambda a: a)
-    email = factory.Faker('email')
+    email = factory.Faker("email")
+    json = {"char": "string", "integer": 100, "float": 2.0}
 
     class Meta:
         model = models.DemoModelField
 
     @factory.lazy_attribute
     def flags(self):
         return get_flags()
 
 
 class UserFactory(ModelFactory):
     class Meta:
         model = User
-        django_get_or_create = ('username',)
+        django_get_or_create = ("username",)
 
 
 class CountryFactory(ModelFactory):
-    name = factory.Faker('country')
+    name = factory.Faker("country")
 
     class Meta:
         model = models.Country
-        django_get_or_create = ('name',)
+        django_get_or_create = ("name",)
 
 
 class BandFactory(ModelFactory):
-    name = factory.Faker('name')
+    name = factory.Faker("name")
     genre = factory.fuzzy.FuzzyChoice([1, 2, 3, 4])
 
     class Meta:
         model = models.Band
-        django_get_or_create = ('name',)
+        django_get_or_create = ("name",)
 
 
 class ArtistFactory(ModelFactory):
-    name = factory.Faker('first_name')
-    last_name = factory.Faker('last_name')
-    full_name = factory.LazyAttribute(lambda o: f'{o.last_name}, {o.name}')
+    name = factory.Faker("first_name")
+    last_name = factory.Faker("last_name")
+    full_name = factory.LazyAttribute(lambda o: f"{o.last_name}, {o.name}")
 
     country = factory.SubFactory(CountryFactory)
-    year_of_birth = factory.Faker('year')
+    year_of_birth = factory.Faker("year")
 
     class Meta:
         model = models.Artist
-        django_get_or_create = ('name', 'last_name')
+        django_get_or_create = ("name", "last_name")
 
     @factory.post_generation
     def bands(self, create, extracted, **kwargs):
         if not create:
             # Simple build, do nothing.
             return
 
@@ -119,8 +124,8 @@
 
 def get_factory_for_model(_model):
     class Meta:
         model = _model
 
     if _model in factories_registry:
         return factories_registry[_model]
-    return type('AAA', (ModelFactory,), {'Meta': Meta})
+    return type("AAA", (ModelFactory,), {"Meta": Meta})
```

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/management/commands/init_demo.py` & `django-adminfilters-2.2.0/tests/demoapp/demo/management/commands/init_demo.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,103 +3,123 @@
 from django.core.management import BaseCommand, call_command
 from django.db import IntegrityError
 
 from adminfilters.depot.models import StoredFilter
 
 
 def sample_data():
-    from demo.factories import (ArtistFactory, BandFactory,
-                                CountryFactory, UserFactory,)
+    from demo.factories import ArtistFactory, BandFactory, CountryFactory, UserFactory
     from demo.models import Artist
     from django.contrib.contenttypes.models import ContentType
 
-    user = UserFactory(username='user')
+    user = UserFactory(username="user")
 
-    uk = CountryFactory(name='United Kingdom')
-    australia = CountryFactory(name='Australia')
+    uk = CountryFactory(name="United Kingdom")
+    australia = CountryFactory(name="Australia")
 
-    acdc = BandFactory(name='AC/DC', active=True)
-    geordie = BandFactory(name='Geordie', active=False)
+    acdc = BandFactory(name="AC/DC", active=True)
+    geordie = BandFactory(name="Geordie", active=False)
 
-    ArtistFactory(name='Angus',
-                  last_name='Young',
-                  full_name='Young, Angus',
-                  active=True,
-                  year_of_birth=1955,
-                  bands=[acdc],
-                  country=uk, flags={'v': 1})
-
-    ArtistFactory(name='Malcom',
-                  last_name='Young',
-                  full_name='Young, Malcom',
-                  year_of_birth=1953,
-                  active=True,
-                  bands=[acdc],
-                  country=uk, flags={'v': 1})
-
-    ArtistFactory(name='Phil',
-                  last_name='Rudd',
-                  full_name='Rudd, Phil',
-                  year_of_birth=1954,
-                  bands=[acdc],
-                  active=True,
-                  country=australia, flags={'full_name': 'Phil Rudd'})
-
-    ArtistFactory(name='Brian',
-                  last_name='Johnson',
-                  full_name='Johnson, Brian',
-                  year_of_birth=1947,
-                  active=True,
-                  bands=[acdc, geordie],
-                  country=uk, flags={'full_name': 'Brian Johnson'})
-
-    ArtistFactory(name='Bon',
-                  last_name='Scott',
-                  full_name='Scott, Bon',
-                  year_of_birth=1946,
-                  active=False,
-                  bands=[acdc],
-                  country=uk, flags={'full_name': 'Bon Scott'})
+    ArtistFactory(
+        name="Angus",
+        last_name="Young",
+        full_name="Young, Angus",
+        active=True,
+        year_of_birth=1955,
+        bands=[acdc],
+        country=uk,
+        flags={"v": 1},
+    )
+
+    ArtistFactory(
+        name="Malcom",
+        last_name="Young",
+        full_name="Young, Malcom",
+        year_of_birth=1953,
+        active=True,
+        bands=[acdc],
+        country=uk,
+        flags={"v": 1},
+    )
+
+    ArtistFactory(
+        name="Phil",
+        last_name="Rudd",
+        full_name="Rudd, Phil",
+        year_of_birth=1954,
+        bands=[acdc],
+        active=True,
+        country=australia,
+        flags={"full_name": "Phil Rudd"},
+    )
+
+    ArtistFactory(
+        name="Brian",
+        last_name="Johnson",
+        full_name="Johnson, Brian",
+        year_of_birth=1947,
+        active=True,
+        bands=[acdc, geordie],
+        country=uk,
+        flags={"full_name": "Brian Johnson"},
+    )
+
+    ArtistFactory(
+        name="Bon",
+        last_name="Scott",
+        full_name="Scott, Bon",
+        year_of_birth=1946,
+        active=False,
+        bands=[acdc],
+        country=uk,
+        flags={"full_name": "Bon Scott"},
+    )
     ct = ContentType.objects.get_for_model(Artist)
     StoredFilter.objects.update_or_create(
-        name='AC/DC',
+        name="AC/DC",
         owner=user,
         defaults=dict(
             owner=user,
-            query_string='?%s' % urlencode({'qs': 'bands__name=AC/DC'}),
-            content_type=ct)
+            query_string="?%s" % urlencode({"qs": "bands__name=AC/DC"}),
+            content_type=ct,
+        ),
     )
     StoredFilter.objects.update_or_create(
-        name='QueryString',
+        name="QueryString",
         owner=user,
         defaults=dict(
-            query_string='?%s' % urlencode({'qs': """country__name__istartswith=australia
+            query_string="?%s"
+            % urlencode(
+                {
+                    "qs": """country__name__istartswith=australia
 name=Phil
 year_of_birth__gt=1950
 Aactive=true""",
-                                            'qs__negate': 'false'}),
-            content_type=ct
-        )
+                    "qs__negate": "false",
+                }
+            ),
+            content_type=ct,
+        ),
     )
     StoredFilter.objects.update_or_create(
-        name='Active Artists',
+        name="Active Artists",
         owner=user,
         defaults=dict(
-            query_string='?%s' % urlencode({'qs': 'active=true'}),
-            content_type=ct
-        )
+            query_string="?%s" % urlencode({"qs": "active=true"}), content_type=ct
+        ),
     )
 
     return [acdc, geordie]
 
 
 class Command(BaseCommand):
     def handle(self, *args, **options):
         from demo.factories import ArtistFactory, DemoModelFieldFactory
-        call_command('migrate')
-        call_command('collectstatic', interactive=False)
+
+        call_command("migrate")
+        call_command("collectstatic", interactive=False)
         try:
             ArtistFactory.create_batch(10)
             DemoModelFieldFactory.create_batch(10)
         except IntegrityError:
             pass
         sample_data()
```

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/models.py` & `django-adminfilters-2.2.0/tests/demoapp/demo/models.py`

 * *Files 11% similar despite different names*

```diff
@@ -24,66 +24,68 @@
     email = models.EmailField()
     #    filepath = models.FilePathField(path=__file__)
     float = models.FloatField()
     bigint = models.BigIntegerField()
     generic_ip = models.GenericIPAddressField()
     url = models.URLField()
     text = models.TextField()
-
+    json = models.JSONField()
     unique = models.CharField(max_length=255, unique=True)
     nullable = models.CharField(max_length=255, null=True)
     blank = models.CharField(max_length=255, blank=True, null=True)
-    not_editable = models.CharField(max_length=255, editable=False,
-                                    blank=True, null=True)
-    choices = models.IntegerField(choices=((1, 'Choice 1'),
-                                           (2, 'Choice 2'),
-                                           (3, 'Choice 3')))
+    not_editable = models.CharField(
+        max_length=255, editable=False, blank=True, null=True
+    )
+    choices = models.IntegerField(
+        choices=((1, "Choice 1"), (2, "Choice 2"), (3, "Choice 3"))
+    )
 
     class Meta:
-        app_label = 'demo'
+        app_label = "demo"
 
 
 class Country(models.Model):
     name = models.CharField(max_length=255)
 
     def __str__(self):
         return self.name
 
     class Meta:
-        verbose_name_plural = 'Countries'
-        ordering = ('name',)
+        verbose_name_plural = "Countries"
+        ordering = ("name",)
 
 
 class Band(models.Model):
     name = models.CharField(max_length=255)
-    genre = models.IntegerField(choices=((1, 'Rock'),
-                                         (2, 'Blues'),
-                                         (3, 'Soul'),
-                                         (4, 'Other'),
-                                         ))
+    genre = models.IntegerField(
+        choices=(
+            (1, "Rock"),
+            (2, "Blues"),
+            (3, "Soul"),
+            (4, "Other"),
+        )
+    )
     active = models.BooleanField(default=True)
 
     def __str__(self):
         return self.name
 
 
 class Artist(JSONMixin, models.Model):
     name = models.CharField(max_length=255)
     last_name = models.CharField(max_length=255)
     full_name = models.CharField(max_length=255)
     country = models.ForeignKey(Country, on_delete=models.CASCADE)
     year_of_birth = models.IntegerField()
     active = models.BooleanField(default=True)
-    bands = models.ManyToManyField(Band,
-                                   related_name='bands',
-                                   verbose_name='Bands')
+    bands = models.ManyToManyField(Band, related_name="bands", verbose_name="Bands")
 
     class Meta:
-        app_label = 'demo'
-        ordering = ('name',)
+        app_label = "demo"
+        ordering = ("name",)
 
     def __str__(self):
         return self.name
 
 
 #
 # class DemoModel2(models.Model):
@@ -96,26 +98,26 @@
 #     class Meta:
 #         app_label = 'demo'
 
 
 class Artist_RelatedFieldCheckBoxFilter(Artist):
     class Meta:
         proxy = True
-        verbose_name = 'RelatedFieldCheckBoxFilter'
+        verbose_name = "RelatedFieldCheckBoxFilter"
 
 
 class Artist_RelatedFieldRadioFilter(Artist):
     class Meta:
         proxy = True
-        verbose_name = 'RelatedFieldRadioFilter'
+        verbose_name = "RelatedFieldRadioFilter"
 
 
 class Artist_UnionFieldListFilter(Artist):
     class Meta:
         proxy = True
-        verbose_name = 'UnionFieldListFilter'
+        verbose_name = "UnionFieldListFilter"
 
 
 class Artist_IntersectionFieldListFilter(Artist):
     class Meta:
         proxy = True
-        verbose_name = 'IntersectionFieldListFilter'
+        verbose_name = "IntersectionFieldListFilter"
```

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/settings.py` & `django-adminfilters-2.2.0/tests/demoapp/demo/settings.py`

 * *Files 24% similar despite different names*

```diff
@@ -2,105 +2,104 @@
 import sys
 from pathlib import Path
 from uuid import uuid4
 
 from environ import environ
 
 here = os.path.dirname(__file__)
-sys.path.append(os.path.abspath(os.path.join(here, '..', '..')))
+sys.path.append(os.path.abspath(os.path.join(here, "..", "..")))
 
 BASE_DIR = Path(__file__).resolve(strict=True).parents[3]
 
 env = environ.Env(
     DEBUG=(bool, False),
-    STATIC_ROOT=(str, str(BASE_DIR / '~build' / 'staticfiles')),
-    DATABASE_URL=(str, ''),
+    STATIC_ROOT=(str, str(BASE_DIR / "~build" / "staticfiles")),
+    DATABASE_URL=(str, ""),
     ROOT_TOKEN=(str, uuid4().hex),
 )
 
-DEBUG = env('DEBUG')
+DEBUG = env("DEBUG")
 TEMPLATE_DEBUG = DEBUG
-ALLOWED_HOSTS = ['*']
+ALLOWED_HOSTS = ["*"]
 
-TIME_ZONE = 'Asia/Bangkok'
-LANGUAGE_CODE = 'en-us'
+TIME_ZONE = "Asia/Bangkok"
+LANGUAGE_CODE = "en-us"
 SITE_ID = 1
 USE_I18N = True
 USE_L10N = True
 USE_TZ = True
-MEDIA_ROOT = os.path.join(here, 'media')
-MEDIA_URL = '/media/'
-STATIC_ROOT = env('STATIC_ROOT')
-STATIC_URL = '/static/'
-DEFAULT_AUTO_FIELD = 'django.db.models.AutoField'
+MEDIA_ROOT = os.path.join(here, "media")
+MEDIA_URL = "/media/"
+STATIC_ROOT = env("STATIC_ROOT")
+STATIC_URL = "/static/"
+DEFAULT_AUTO_FIELD = "django.db.models.AutoField"
 
-STATICFILES_DIRS = (
+STATICFILES_DIRS = ()
 
-)
-
-SECRET_KEY = 'c73*n!y=)tziu^2)y*@5i2^)$8z$tx#b9*_r3i6o1ohxo%*2^a'
+SECRET_KEY = "c73*n!y=)tziu^2)y*@5i2^)$8z$tx#b9*_r3i6o1ohxo%*2^a"
 MIDDLEWARE = (
-    'django.middleware.common.CommonMiddleware',
-    'django.contrib.sessions.middleware.SessionMiddleware',
-    'django.middleware.csrf.CsrfViewMiddleware',
-    'django.contrib.auth.middleware.AuthenticationMiddleware',
-    'django.contrib.messages.middleware.MessageMiddleware',)
+    "django.middleware.common.CommonMiddleware",
+    "django.contrib.sessions.middleware.SessionMiddleware",
+    "django.middleware.csrf.CsrfViewMiddleware",
+    "django.contrib.auth.middleware.AuthenticationMiddleware",
+    "django.contrib.messages.middleware.MessageMiddleware",
+)
 
-DATABASES = {
-    'default': env.db()
-}
-MESSAGE_STORAGE = 'django.contrib.messages.storage.cookie.CookieStorage'
+DATABASES = {"default": env.db()}
+MESSAGE_STORAGE = "django.contrib.messages.storage.cookie.CookieStorage"
 
-ROOT_URLCONF = 'demo.urls'
-WSGI_APPLICATION = 'demo.wsgi.application'
+ROOT_URLCONF = "demo.urls"
+WSGI_APPLICATION = "demo.wsgi.application"
 
-AUTHENTICATION_BACKENDS = ('demo.backends.AnonymousAccessUserBackend',)
+AUTHENTICATION_BACKENDS = ("demo.backends.AnonymousAccessUserBackend",)
 
 INSTALLED_APPS = (
-    'django.contrib.auth',
-    'django.contrib.contenttypes',
-    'django.contrib.sessions',
-    'django.contrib.sites',
-    'django.contrib.messages',
-    'django.contrib.staticfiles',
-    'django.contrib.admin',
-    'adminfilters',
-    'adminfilters.depot',
-    'demo')
+    "django.contrib.auth",
+    "django.contrib.contenttypes",
+    "django.contrib.sessions",
+    "django.contrib.sites",
+    "django.contrib.messages",
+    "django.contrib.staticfiles",
+    "django.contrib.admin",
+    "adminfilters",
+    "adminfilters.depot",
+    "demo",
+)
 
 TEMPLATES = [
-    {'BACKEND': 'django.template.backends.django.DjangoTemplates',
-     'DIRS': [],
-     'APP_DIRS': True,
-     'OPTIONS': {
-         'debug': DEBUG,
-         'context_processors': [
-             'django.contrib.auth.context_processors.auth',
-             'django.template.context_processors.request',
-             'django.template.context_processors.debug',
-             'django.template.context_processors.i18n',
-             'django.template.context_processors.media',
-             'django.template.context_processors.static',
-             'django.template.context_processors.tz',
-             'django.contrib.messages.context_processors.messages',
-         ],
-     },
-     }
+    {
+        "BACKEND": "django.template.backends.django.DjangoTemplates",
+        "DIRS": [],
+        "APP_DIRS": True,
+        "OPTIONS": {
+            "debug": DEBUG,
+            "context_processors": [
+                "django.contrib.auth.context_processors.auth",
+                "django.template.context_processors.request",
+                "django.template.context_processors.debug",
+                "django.template.context_processors.i18n",
+                "django.template.context_processors.media",
+                "django.template.context_processors.static",
+                "django.template.context_processors.tz",
+                "django.contrib.messages.context_processors.messages",
+            ],
+        },
+    }
 ]
 
 LOGGING = {
-    'version': 1,
-    'disable_existing_loggers': False,
-    'handlers': {
-        'console': {
-            'class': 'logging.StreamHandler',
+    "version": 1,
+    "disable_existing_loggers": False,
+    "handlers": {
+        "console": {
+            "class": "logging.StreamHandler",
         },
     },
-    'root': {
-        'handlers': ['console'],
-        'level': 'ERROR',
+    "root": {
+        "handlers": ["console"],
+        "level": "ERROR",
     },
-    'pytest_selenium': {
-        'handlers': ['console'],
-        'level': 'ERROR',
+    "pytest_selenium": {
+        "handlers": ["console"],
+        "level": "ERROR",
     },
 }
```

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/static/favicon.ico` & `django-adminfilters-2.2.0/tests/demoapp/demo/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/urls.py` & `django-adminfilters-2.2.0/tests/demoapp/demo/urls.py`

 * *Files 12% similar despite different names*

```diff
@@ -7,35 +7,48 @@
 from adminfilters.depot.admin import StoredFilterAdmin
 from adminfilters.depot.models import StoredFilter
 
 from . import admin, models
 
 
 class PublicAdminSite(django.contrib.admin.sites.AdminSite):
-
     def has_permission(self, request):
-        request.user = User.objects.get_or_create(username='sax')[0]
+        request.user = User.objects.get_or_create(username="sax")[0]
         return True
 
 
 public_site = PublicAdminSite()
 django.contrib.admin.autodiscover()
-public_site.register(models.Artist_RelatedFieldCheckBoxFilter,
-                     admin.DemoModelAdmin_RelatedFieldCheckBoxFilter)
-public_site.register(models.Artist_RelatedFieldRadioFilter,
-                     admin.DemoModelAdmin_RelatedFieldRadioFilter)
-public_site.register(models.Artist_UnionFieldListFilter,
-                     admin.DemoModelAdmin_UnionFieldListFilter)
-public_site.register(models.Artist_IntersectionFieldListFilter,
-                     admin.DemoModelAdmin_IntersectionFieldListFilter)
+public_site.register(
+    models.Artist_RelatedFieldCheckBoxFilter,
+    admin.DemoModelAdmin_RelatedFieldCheckBoxFilter,
+)
+public_site.register(
+    models.Artist_RelatedFieldRadioFilter, admin.DemoModelAdmin_RelatedFieldRadioFilter
+)
+public_site.register(
+    models.Artist_UnionFieldListFilter, admin.DemoModelAdmin_UnionFieldListFilter
+)
+public_site.register(
+    models.Artist_IntersectionFieldListFilter,
+    admin.DemoModelAdmin_IntersectionFieldListFilter,
+)
 public_site.register(models.Country, admin.CountryModelAdmin)
 public_site.register(models.Band, admin.BandModelAdmin)
 public_site.register(models.Artist, admin.ArtistModelAdmin)
 public_site.register(models.DemoModelField, admin.DemoModelFieldAdmin)
 public_site.register(User, admin.IUserAdmin)
 public_site.register(StoredFilter, StoredFilterAdmin)
 
 urlpatterns = (
-    re_path(r'^(?P<path>favicon.ico)$', django.views.static.serve, {'document_root': settings.STATIC_ROOT}),
-    re_path(r'^static/(?P<path>.*)$', django.views.static.serve, {'document_root': settings.STATIC_ROOT}),
-    re_path(r'', public_site.urls),
+    re_path(
+        r"^(?P<path>favicon.ico)$",
+        django.views.static.serve,
+        {"document_root": settings.STATIC_ROOT},
+    ),
+    re_path(
+        r"^static/(?P<path>.*)$",
+        django.views.static.serve,
+        {"document_root": settings.STATIC_ROOT},
+    ),
+    re_path(r"", public_site.urls),
 )
```

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/utils.py` & `django-adminfilters-2.2.0/tests/demoapp/demo/utils.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,152 +4,164 @@
 from django.utils.functional import cached_property
 from django.utils.html import strip_tags
 from selenium.common.exceptions import NoSuchElementException
 from selenium.webdriver.common.by import By
 from selenium.webdriver.remote.webelement import WebElement
 
 DATA = {
-    'date': '2013-01-29',
-    'datetime': '2013-01-01T02:18:33Z',
-    'integer': 888888,
-    'nullable': 'bbbb',
-    'time': '19:00:35',
-    'bigint': 333333333,
+    "date": "2013-01-29",
+    "datetime": "2013-01-01T02:18:33Z",
+    "integer": 888888,
+    "nullable": "bbbb",
+    "time": "19:00:35",
+    "bigint": 333333333,
     # "blank": "",
-    'choices': 2,
-    'decimal': '22.2',
+    "choices": 2,
+    "decimal": "22.2",
     # "email": "s.apostolico@gmail.com",
-    'float': 10.1,
-    'generic_ip': '192.168.10.2',
+    "float": 10.1,
+    "generic_ip": "192.168.10.2",
     # "logic": False,
     # "not_editable": None,
     # "text": "lorem ipsum",
     # "url": "https://github.com/saxix/django-adminfilters",
     # # "flags": {},
 }
 
 
 def check_link_by_class(selenium, cls, view_name):
     link = selenium.find_element_by_class_name(cls)
-    url = reverse(f'{view_name}')
-    return f' href="{url}"' in link.get_attribute('innerHTML')
+    url = reverse(f"{view_name}")
+    return f' href="{url}"' in link.get_attribute("innerHTML")
 
 
 def get_all_attributes(driver, element):
-    return list(driver.execute_script(
-        'var items = {}; for (index = 0; index < arguments[0].attributes.length; ++index) {'
-        ' items[arguments[0].attributes[index].name] = arguments[0].attributes[index].value'
-        ' }; return items;',
-        element))
+    return list(
+        driver.execute_script(
+            "var items = {}; for (index = 0; index < arguments[0].attributes.length; ++index) {"
+            " items[arguments[0].attributes[index].name] = arguments[0].attributes[index].value"
+            " }; return items;",
+            element,
+        )
+    )
 
 
 def is_clickable(driver, element):
     """Tries to click the element"""
     try:
         element.click()
         return True
     except Exception:
         return False
 
 
 def mykey(group, request):
-    return request.META['REMOTE_ADDR'][::-1]
+    return request.META["REMOTE_ADDR"][::-1]
 
 
 def callable_rate(group, request):
     if request.user.is_authenticated:
         return None
     return (0, 1)
 
 
 def scroll_to(driver, *args, _timeout=10):
     from selenium.webdriver.support import expected_conditions as EC
     from selenium.webdriver.support.ui import WebDriverWait
+
     wait = WebDriverWait(driver, _timeout)
     wait.until(EC.visibility_of_element_located((*args,)))
     return driver.find_element(*args)
 
 
 def wait_for(driver, *args, _timeout=10):
     from selenium.webdriver.support import expected_conditions as EC
     from selenium.webdriver.support.ui import WebDriverWait
+
     wait = WebDriverWait(driver, _timeout)
     wait.until(EC.visibility_of_element_located((*args,)))
     return driver.find_element(*args)
 
 
 def prompt(driver, text, _timeout=10):
     from selenium.webdriver.common.alert import Alert
     from selenium.webdriver.support.expected_conditions import alert_is_present
     from selenium.webdriver.support.ui import WebDriverWait
+
     wait = WebDriverWait(driver, _timeout)
     wait.until(alert_is_present())
 
     alert = Alert(driver)
     alert.send_keys(text)
     return alert
 
 
 def confirm(driver, _timeout=10):
     from selenium.webdriver.common.alert import Alert
     from selenium.webdriver.support.expected_conditions import alert_is_present
     from selenium.webdriver.support.ui import WebDriverWait
+
     wait = WebDriverWait(driver, _timeout)
     wait.until(alert_is_present())
 
     alert = Alert(driver)
     return alert
 
 
 def wait_and_click(driver, *args, _timeout=10):
     from selenium.webdriver.support import expected_conditions as EC
     from selenium.webdriver.support.ui import WebDriverWait
+
     wait = WebDriverWait(driver, _timeout)
     wait.until(EC.element_to_be_clickable((*args,)))
     return driver.find_element(*args).click()
 
 
 def wait_for_url(driver, url):
     from selenium.webdriver.support import expected_conditions as EC
     from selenium.webdriver.support.ui import WebDriverWait
+
     wait = WebDriverWait(driver, 10)
     wait.until(EC.url_contains(url))
 
 
 class WebElementWrapper:
     def __init__(self, element: WebElement):
         self.element = element
 
     def __getattr__(self, item):
         return getattr(self.element, item)
 
     def __repr__(self):
         return '<{0.__module__}.{0.__name__} (session="{1}", element="{2}")>'.format(
-            type(self.element), self._parent.session_id, self.element._id)
+            type(self.element), self._parent.session_id, self.element._id
+        )
 
     @property
     def driver(self):
         return self.element.parent
 
 
 class CellWrapper(WebElementWrapper):
     @cached_property
     def text(self):
-        return (self.element.get_attribute('innerText') or strip_tags(self.element.get_attribute('innerHTML')))
+        return self.element.get_attribute("innerText") or strip_tags(
+            self.element.get_attribute("innerHTML")
+        )
 
 
 class RowWrapper(WebElementWrapper):
     @cached_property
     def values(self):
         return [e.text for e in self.cells]
 
     @cached_property
     def cells(self):
         ret = []
-        for e in self.element.find_elements(By.CSS_SELECTOR, 'td,th')[1:]:
+        for e in self.element.find_elements(By.CSS_SELECTOR, "td,th")[1:]:
             ret.append(CellWrapper(e))
         return ret
 
 
 class EmptyChangeListWrapper(WebElementWrapper):
     rows = []
     header = []
@@ -165,25 +177,30 @@
         return None
 
 
 class ChangeListWrapper(EmptyChangeListWrapper):
     @classmethod
     def find_in_page(cls, driver):
         try:
-            return ChangeListWrapper(driver.find_element(By.CSS_SELECTOR, '#changelist-form #result_list'))
+            return ChangeListWrapper(
+                driver.find_element(By.CSS_SELECTOR, "#changelist-form #result_list")
+            )
         except NoSuchElementException:
             return EmptyChangeListWrapper(None)
 
     @cached_property
     def header(self) -> [RowWrapper]:
-        return RowWrapper(self.element.find_element(By.CSS_SELECTOR, 'thead tr'))
+        return RowWrapper(self.element.find_element(By.CSS_SELECTOR, "thead tr"))
 
     @cached_property
     def rows(self) -> [RowWrapper]:
-        return [RowWrapper(e) for e in self.element.find_elements(By.CSS_SELECTOR, 'tbody tr')]
+        return [
+            RowWrapper(e)
+            for e in self.element.find_elements(By.CSS_SELECTOR, "tbody tr")
+        ]
 
     def get_row(self, num):
         return list(self.rows)[num]
 
     def get_col(self, num):
         return [row.cells[num] for row in self.rows]
 
@@ -205,27 +222,28 @@
         cells = []
         for row in self.rows:
             cells.append([c.text for c in row.cells])
         return cells
 
     def pretty(self):
         from prettytable import PrettyTable
+
         x = PrettyTable(max_table_width=180)
         x.field_names = self.header.values
         x.add_rows(self.matrix)
-        sys.stdout.write(f'\n{x}\n')
+        sys.stdout.write(f"\n{x}\n")
 
 
 class Checkbox(WebElementWrapper):
     def checked(self, value):
         if value and not self.element.is_selected():
-            self.driver.execute_script('arguments[0].click();', self.element)
+            self.driver.execute_script("arguments[0].click();", self.element)
         if not value and self.element.is_selected():
-            self.driver.execute_script('arguments[0].click();', self.element)
+            self.driver.execute_script("arguments[0].click();", self.element)
 
     def check(self):
         if not self.element.is_selected():
-            self.driver.execute_script('arguments[0].click();', self.element)
+            self.driver.execute_script("arguments[0].click();", self.element)
 
     def uncheck(self):
         if self.element.is_selected():
-            self.driver.execute_script('arguments[0].click();', self.element)
+            self.driver.execute_script("arguments[0].click();", self.element)
```

### Comparing `django-adminfilters-2.1.0/tests/demoapp/demo/wsgi.py` & `django-adminfilters-2.2.0/tests/demoapp/demo/wsgi.py`

 * *Files 11% similar despite different names*

```diff
@@ -16,14 +16,14 @@
 import os
 
 # This application object is used by any WSGI server configured to use this
 # file. This includes Django's development server, if the WSGI_APPLICATION
 # setting points here.
 from django.core.wsgi import get_wsgi_application
 
-os.environ.setdefault('DJANGO_SETTINGS_MODULE', 'demo.settings')
+os.environ.setdefault("DJANGO_SETTINGS_MODULE", "demo.settings")
 
 application = get_wsgi_application()
 
 # Apply WSGI middleware here.
 # from helloworld.wsgi import HelloWorldApplication
 # application = HelloWorldApplication(application)
```

### Comparing `django-adminfilters-2.1.0/tests/functional/conftest.py` & `django-adminfilters-2.2.0/tests/functional/conftest.py`

 * *Files 4% similar despite different names*

```diff
@@ -7,27 +7,28 @@
 from selenium.webdriver.chrome.options import Options
 from selenium.webdriver.common.by import By
 
 
 @pytest.fixture
 def chrome_options(request):
     chrome_options = Options()
-    if not request.config.getvalue('show_browser'):
-        chrome_options.add_argument('--headless')
+    if not request.config.getvalue("show_browser"):
+        chrome_options.add_argument("--headless")
     return chrome_options
 
 
 SELENIUM_DEFAULT_PAGE_LOAD_TIMEOUT = 3
 SELENIUM_DEFAULT_IMPLICITLY_WAIT = 2
 SELENIUM_DEFAULT_SCRIPT_TIMEOUT = 2
 
 
 @contextlib.contextmanager
 def timeouts(driver, wait=None, page=None, script=None):
     from selenium.webdriver.common.timeouts import Timeouts
+
     _current: Timeouts = driver.timeouts
     if wait:
         driver.implicitly_wait(wait)
     if page:
         driver.set_page_load_timeout(page)
     if script:
         driver.set_script_timeout(script)
@@ -45,56 +46,59 @@
 def get_errors(driver):
     """
     Checks browser for errors, returns a list of errors
     :param driver:
     :return:
     """
     try:
-        browser_logs = driver.get_log('browser')
+        browser_logs = driver.get_log("browser")
     except (ValueError, WebDriverException) as e:
         # Some browsers does not support getting logs
-        logging.debug('Could not get browser logs for driver %s due to exception: %s',
-                      driver, e)
+        logging.debug(
+            "Could not get browser logs for driver %s due to exception: %s", driver, e
+        )
         return []
 
-    errors = [entry for entry in browser_logs if entry['level'] == 'SEVERE']
+    errors = [entry for entry in browser_logs if entry["level"] == "SEVERE"]
 
     return errors
 
 
 @pytest.fixture
 def selenium(driver):
     from demo.utils import confirm, prompt, wait_and_click, wait_for
+
     driver.with_timeouts = timeouts.__get__(driver)
     driver.set_input_value = set_input_value.__get__(driver)
     driver.wait_for = wait_for.__get__(driver)
     driver.wait_and_click = wait_and_click.__get__(driver)
     driver.prompt = prompt.__get__(driver)
     driver.confirm = confirm.__get__(driver)
     driver.get_errors = get_errors.__get__(driver)
     yield driver
 
 
 @pytest.fixture(autouse=True)
 def data():
     from demo.factories import ArtistFactory
     from demo.management.commands.init_demo import sample_data
+
     ArtistFactory.create_batch(20)
     sample_data()
 
 
 class AdminSite:
     def __init__(self, live_server, driver):
         self.live_server = live_server
         self.driver = driver
 
-    def open(self, path=''):
+    def open(self, path=""):
         self.driver.get(urljoin(self.live_server.url, path))
         dim = self.driver.get_window_size()
-        self.driver.set_window_size(1100, dim['height'])
+        self.driver.set_window_size(1100, dim["height"])
 
     def wait_for(self, *args):
         return self.driver.wait_for(*args)
 
     def prompt(self, *args):
         return self.driver.prompt(*args)
 
@@ -107,12 +111,12 @@
     def get_errors(self):
         return self.driver.get_errors()
 
 
 @pytest.fixture
 def admin_site(live_server, selenium, data):
     site = AdminSite(live_server, selenium)
-    site.open('/')
-    site.wait_for(By.LINK_TEXT, 'Artists').click()
+    site.open("/")
+    site.wait_for(By.LINK_TEXT, "Artists").click()
     errors = site.get_errors()
-    assert len(errors) == 0, '\n'.join(['{message}'.format(**err) for err in errors])
+    assert len(errors) == 0, "\n".join(["{message}".format(**err) for err in errors])
     return site
```

### Comparing `django-adminfilters-2.1.0/tests/functional/test_f_automplete.py` & `django-adminfilters-2.2.0/tests/functional/test_f_automplete.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,24 +2,26 @@
 from demo.utils import ChangeListWrapper
 from selenium.webdriver.common.by import By
 
 pytestmark = pytest.mark.selenium
 
 
 def get_elements(selenium):
-    container = selenium.find_element(By.ID, 'country__exact_country__isnull')
-    el = selenium.find_elements(By.CSS_SELECTOR, 'input.select2-search__field')
-    return [container,
-            container.find_element(By.CSS_SELECTOR, 'span[role=combobox]'),
-            el[0] if el else None,
-            ChangeListWrapper.find_in_page(selenium)]
+    container = selenium.find_element(By.ID, "country__exact_country__isnull")
+    el = selenium.find_elements(By.CSS_SELECTOR, "input.select2-search__field")
+    return [
+        container,
+        container.find_element(By.CSS_SELECTOR, "span[role=combobox]"),
+        el[0] if el else None,
+        ChangeListWrapper.find_in_page(selenium),
+    ]
 
 
 @pytest.mark.selenium
 def test_autocomplete(admin_site):
     __, select2, *__ = get_elements(admin_site.driver)
     select2.click()
     __, __, input_text, __ = get_elements(admin_site.driver)
-    input_text.send_keys('United K')
+    input_text.send_keys("United K")
     admin_site.wait_and_click(By.XPATH, '//li[contains(text(), "United Kingdom")]')
     *__, cl = get_elements(admin_site.driver)
-    assert set(cl.get_values(None, 5)) == {'United Kingdom'}
+    assert set(cl.get_values(None, 5)) == {"United Kingdom"}
```

### Comparing `django-adminfilters-2.1.0/tests/functional/test_f_depot.py` & `django-adminfilters-2.2.0/tests/functional/test_f_depot.py`

 * *Files 19% similar despite different names*

```diff
@@ -5,50 +5,52 @@
 
 from adminfilters.depot.models import StoredFilter
 
 pytestmark = pytest.mark.selenium
 
 
 def get_elements(selenium):
-    container = selenium.find_element(By.ID, 'adminfilters_depot_adminfilters_depot_op')
-    btn = container.find_elements(By.CSS_SELECTOR, 'a.button')
-    return [container,
-            Select(container.find_element(By.CSS_SELECTOR, 'select')),
-            btn[0] if btn else None,
-            ChangeListWrapper.find_in_page(selenium)]
+    container = selenium.find_element(By.ID, "adminfilters_depot_adminfilters_depot_op")
+    btn = container.find_elements(By.CSS_SELECTOR, "a.button")
+    return [
+        container,
+        Select(container.find_element(By.CSS_SELECTOR, "select")),
+        btn[0] if btn else None,
+        ChangeListWrapper.find_in_page(selenium),
+    ]
 
 
 @pytest.mark.selenium
 def test_save_filter(admin_site):
-    qs = '?name__in=Angus&name__in__negate=false'
-    admin_site.open(f'/demo/artist/{qs}')
+    qs = "?name__in=Angus&name__in__negate=false"
+    admin_site.open(f"/demo/artist/{qs}")
     __, select, button, cl = get_elements(admin_site.driver)
 
     button.click()
-    admin_site.prompt('Filter #1').accept()
+    admin_site.prompt("Filter #1").accept()
 
     __, select, button, cl = get_elements(admin_site.driver)
-    sf = StoredFilter.objects.get(name='Filter #1')
+    sf = StoredFilter.objects.get(name="Filter #1")
     assert sf.query_string == qs
 
 
 @pytest.mark.selenium
 def test_select_filter(admin_site):
-    sf = StoredFilter.objects.get(name='QueryString')
+    sf = StoredFilter.objects.get(name="QueryString")
 
     __, select, button, cl = get_elements(admin_site.driver)
     select.select_by_visible_text(sf.name)
-    admin_site.wait_for(By.TAG_NAME, 'body')
+    admin_site.wait_for(By.TAG_NAME, "body")
     assert sf.query_string in admin_site.driver.current_url
 
 
 @pytest.mark.selenium
 def test_delete_filter(admin_site):
-    sf = StoredFilter.objects.get(name='QueryString')
+    sf = StoredFilter.objects.get(name="QueryString")
     __, select, button, cl = get_elements(admin_site.driver)
     select.select_by_visible_text(sf.name)
-    admin_site.wait_for(By.TAG_NAME, 'body')
+    admin_site.wait_for(By.TAG_NAME, "body")
     __, select, button, cl = get_elements(admin_site.driver)
     button.click()
     admin_site.confirm().accept()
-    admin_site.wait_for(By.TAG_NAME, 'body')
-    assert not StoredFilter.objects.filter(name='QueryString').exists()
+    admin_site.wait_for(By.TAG_NAME, "body")
+    assert not StoredFilter.objects.filter(name="QueryString").exists()
```

### Comparing `django-adminfilters-2.1.0/tests/functional/test_f_querystring.py` & `django-adminfilters-2.2.0/tests/functional/test_f_querystring.py`

 * *Files 16% similar despite different names*

```diff
@@ -2,67 +2,86 @@
 from demo.utils import ChangeListWrapper, Checkbox
 from selenium.webdriver.common.by import By
 
 pytestmark = pytest.mark.selenium
 
 
 def get_elements(selenium):
-    container = selenium.find_element(By.ID, 'qs_qs__negate')
-    return [container,
-            container.find_element(By.CSS_SELECTOR, 'textarea'),
-            container.find_element(By.CSS_SELECTOR, 'a.button'),
-            Checkbox(container.find_element(By.CSS_SELECTOR, 'input[type=checkbox]')),
-            ChangeListWrapper.find_in_page(selenium)]
-
-
-@pytest.mark.parametrize('query,negated,check',
-                         [('name=Angus', False, lambda cl: len(cl.rows) == 1),
-                          ('bands__name=AC/DC', False, lambda cl: len(cl.rows) == 5),
-                          ('bands__name=AC/DC', True, lambda cl: 'Rudd, Phil' not in cl.get_values(None, 4)),
-                          ('country__name=United Kingdom\nbands__name=AC/DC\n!name=Angus', False,
-                           lambda cl: 'Young, Angus' not in cl.get_values(None, 4)),
-                          ('bands__name=AC/DC\nname__in=Angus,Malcom', False,
-                           lambda cl: {'Young'} == set(cl.get_values(None, 3))),
-                          ])
+    container = selenium.find_element(By.ID, "qs_qs__negate")
+    return [
+        container,
+        container.find_element(By.CSS_SELECTOR, "textarea"),
+        container.find_element(By.CSS_SELECTOR, "a.button"),
+        Checkbox(container.find_element(By.CSS_SELECTOR, "input[type=checkbox]")),
+        ChangeListWrapper.find_in_page(selenium),
+    ]
+
+
+@pytest.mark.parametrize(
+    "query,negated,check",
+    [
+        ("name=Angus", False, lambda cl: len(cl.rows) == 1),
+        ("bands__name=AC/DC", False, lambda cl: len(cl.rows) == 5),
+        (
+            "bands__name=AC/DC",
+            True,
+            lambda cl: "Rudd, Phil" not in cl.get_values(None, 4),
+        ),
+        (
+            "country__name=United Kingdom\nbands__name=AC/DC\n!name=Angus",
+            False,
+            lambda cl: "Young, Angus" not in cl.get_values(None, 4),
+        ),
+        (
+            "bands__name=AC/DC\nname__in=Angus,Malcom",
+            False,
+            lambda cl: {"Young"} == set(cl.get_values(None, 3)),
+        ),
+    ],
+)
 @pytest.mark.selenium
 def test_querystring(admin_site, query, negated, check):
     __, textarea, button, negate, cl = get_elements(admin_site.driver)
     textarea.send_keys(query)
     negate.checked(negated)
     button.click()
     __, textarea, button, negate, cl = get_elements(admin_site.driver)
     assert check(cl), cl.pretty()
 
 
 @pytest.mark.selenium
-@pytest.mark.parametrize('flag,results', [('active=true', 1),
-                                          ('active=false', 0),
-                                          ('!active=false', 1),
-                                          ('!active=true', 0),
-                                          ])
+@pytest.mark.parametrize(
+    "flag,results",
+    [
+        ("active=true", 1),
+        ("active=false", 0),
+        ("!active=false", 1),
+        ("!active=true", 0),
+    ],
+)
 def test_querystring_bool(admin_site, flag, results):
     __, textarea, button, negate, cl = get_elements(admin_site.driver)
 
     negate.uncheck()
     textarea.clear()
-    textarea.send_keys(f'{flag}\ncountry__name=Australia\nname=Phil')
+    textarea.send_keys(f"{flag}\ncountry__name=Australia\nname=Phil")
     button.click()
     __, textarea, button, negate, cl = get_elements(admin_site.driver)
     assert len(cl.rows) == results
 
 
 @pytest.mark.selenium
 def test_errored_querystring(admin_site):
     __, textarea, button, negate, cl = get_elements(admin_site.driver)
 
-    textarea.send_keys('invalid_field=AAAA')
+    textarea.send_keys("invalid_field=AAAA")
     button.click()
     assert "Unknown field 'invalid_field'" in admin_site.driver.page_source
 
 
 @pytest.mark.selenium
 def test_invalid_querystring(admin_site):
     __, textarea, button, negate, cl = get_elements(admin_site.driver)
 
-    textarea.send_keys('=')
+    textarea.send_keys("=")
     button.click()
-    assert 'Invalid django filter' in admin_site.driver.page_source
+    assert "Invalid django filter" in admin_site.driver.page_source
```

### Comparing `django-adminfilters-2.1.0/tests/functional/test_f_value.py` & `django-adminfilters-2.2.0/tests/functional/test_f_value.py`

 * *Files 10% similar despite different names*

```diff
@@ -2,53 +2,57 @@
 from demo.utils import ChangeListWrapper, Checkbox
 from selenium.webdriver.common.by import By
 
 pytestmark = pytest.mark.selenium
 
 
 def get_elements(selenium):
-    container = selenium.find_element(By.ID, 'last_name__istartswith_last_name__istartswith__negate')
-    return [container.find_element(By.CSS_SELECTOR, 'input[type=text]'),
-            Checkbox(container.find_element(By.CSS_SELECTOR, 'input[type=checkbox]')),
-            container.find_element(By.CSS_SELECTOR, 'a.button'),
-            ChangeListWrapper.find_in_page(selenium)]
+    container = selenium.find_element(
+        By.ID, "last_name__istartswith_last_name__istartswith__negate"
+    )
+    return [
+        container.find_element(By.CSS_SELECTOR, "input[type=text]"),
+        Checkbox(container.find_element(By.CSS_SELECTOR, "input[type=checkbox]")),
+        container.find_element(By.CSS_SELECTOR, "a.button"),
+        ChangeListWrapper.find_in_page(selenium),
+    ]
 
 
 @pytest.mark.selenium
 def test_value_simple_filter(data, admin_site):
     input_text, negate, button, cl = get_elements(admin_site.driver)
-    input_text.send_keys('Young')
+    input_text.send_keys("Young")
     button.click()
     input_text, negate, button, cl = get_elements(admin_site.driver)
-    assert set(cl.get_values(None, 3)) == {'Young'}
+    assert set(cl.get_values(None, 3)) == {"Young"}
     negate.click()
     button.click()
     input_text, negate, button, cl = get_elements(admin_site.driver)
-    assert 'Young' not in set(cl.get_values(None, 3))
+    assert "Young" not in set(cl.get_values(None, 3))
 
 
 @pytest.mark.selenium
 def test_multivalue_simple_filter(data, admin_site):
     input_text, negate, button, cl = get_elements(admin_site.driver)
-    input_text.send_keys('Young')
+    input_text.send_keys("Young")
     button.click()
     input_text, negate, button, cl = get_elements(admin_site.driver)
-    assert set(cl.get_values(None, 3)) == {'Young'}
+    assert set(cl.get_values(None, 3)) == {"Young"}
 
     negate.click()
     button.click()
     input_text, negate, button, cl = get_elements(admin_site.driver)
-    assert 'Young' not in set(cl.get_values(None, 3))
+    assert "Young" not in set(cl.get_values(None, 3))
 
 
 @pytest.mark.selenium
 def test_multivalue_filter_clear(data, admin_site):
     input_text, negate, button, cl = get_elements(admin_site.driver)
-    input_text.send_keys('Young')
+    input_text.send_keys("Young")
     button.click()
     input_text, negate, button, cl = get_elements(admin_site.driver)
-    assert set(cl.get_values(None, 3)) == {'Young'}
+    assert set(cl.get_values(None, 3)) == {"Young"}
     assert len(cl.rows) == 2
 
     button.click()
     input_text, negate, button, cl = get_elements(admin_site.driver)
     assert len(cl.rows) == 25
```

### Comparing `django-adminfilters-2.1.0/tests/test_dj.py` & `django-adminfilters-2.2.0/tests/test_dj.py`

 * *Files 22% similar despite different names*

```diff
@@ -3,35 +3,41 @@
 
 from adminfilters.dj import DjangoLookupFilter
 
 
 @pytest.fixture
 def fixtures(db):
     from demo.factories import ArtistFactory
-    ArtistFactory(name='a1', active=True)
-    ArtistFactory(name='a2', active=True)
-    ArtistFactory(name='b1', active=True)
-    ArtistFactory(name='c1', active=False)
+
+    ArtistFactory(name="a1", active=True)
+    ArtistFactory(name="a2", active=True)
+    ArtistFactory(name="b1", active=True)
+    ArtistFactory(name="c1", active=False)
 
 
 def test_media():
-    assert DjangoLookupFilter.factory(title='Title')(None, {}, Artist, None).media
+    assert DjangoLookupFilter.factory(title="Title")(None, {}, Artist, None).media
 
 
-@pytest.mark.parametrize('key,value,negate,expected', [('name', 'a1', False, ['a1']),
-                                                       ('name__endswith', '2', False, ['a2']),
-                                                       ('name__in', 'a1,a2', False, ['a1', 'a2']),
-                                                       ('active', 'true', False, ['a1', 'a2', 'b1']),
-                                                       ('active', 'false', False, ['c1']),
-                                                       ('active', 'false', True, ['a1', 'a2', 'b1']),
-                                                       ('xx', 'zz', True, ['a1', 'a2', 'b1', 'c1']),
-                                                       ])
+@pytest.mark.parametrize(
+    "key,value,negate,expected",
+    [
+        ("name", "a1", False, ["a1"]),
+        ("name__endswith", "2", False, ["a2"]),
+        ("name__in", "a1,a2", False, ["a1", "a2"]),
+        ("active", "true", False, ["a1", "a2", "b1"]),
+        ("active", "false", False, ["c1"]),
+        ("active", "false", True, ["a1", "a2", "b1"]),
+        ("xx", "zz", True, ["a1", "a2", "b1", "c1"]),
+    ],
+)
 def test_value_filter(fixtures, key, value, negate, expected):
-    f = DjangoLookupFilter(None, {'dj__key': key,
-                                  'dj__value': value,
-                                  'dj__negate': str(negate).lower()
-                                  },
-                           Artist, None)
+    f = DjangoLookupFilter(
+        None,
+        {"dj__key": key, "dj__value": value, "dj__negate": str(negate).lower()},
+        Artist,
+        None,
+    )
 
     result = f.queryset(None, Artist.objects.all())
-    value = list(result.values_list('name', flat=True))
+    value = list(result.values_list("name", flat=True))
     assert value == expected
```

### Comparing `django-adminfilters-2.1.0/tests/test_django_check.py` & `django-adminfilters-2.2.0/tests/test_django_check.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,19 +12,21 @@
 
 
 def test():
     ret = check_adminfilters_media(None)
     assert ret == [], [e.msg for e in ret]
 
 
-@pytest.mark.parametrize('filter_class', [QueryStringFilter, ('name', ValueFilter)])
+@pytest.mark.parametrize("filter_class", [QueryStringFilter, ("name", ValueFilter)])
 def test_check_error(filter_class):
     class InvalidModelAdmin(ModelAdmin):
-        list_filter = ('active',
-                       filter_class,
-                       ('genre', RelatedFieldCheckBoxFilter),
-                       )
+        list_filter = (
+            "active",
+            filter_class,
+            ("genre", RelatedFieldCheckBoxFilter),
+        )
 
-    with patch.dict(site._registry, {Artist: ArtistModelAdmin,
-                                     Band: InvalidModelAdmin}, clear=True):
+    with patch.dict(
+        site._registry, {Artist: ArtistModelAdmin, Band: InvalidModelAdmin}, clear=True
+    ):
         ret = check_adminfilters_media(None)
         assert len(ret) == 1, [e.msg for e in ret]
```

### Comparing `django-adminfilters-2.1.0/tests/test_multiselect.py` & `django-adminfilters-2.2.0/tests/test_multiselect.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,64 +1,94 @@
 from functools import partial
 from unittest.mock import Mock
 
 import pytest
 from demo.models import Artist
 
-from adminfilters.multiselect import (IntersectionFieldListFilter,
-                                      UnionFieldListFilter,)
+from adminfilters.multiselect import IntersectionFieldListFilter, UnionFieldListFilter
 from adminfilters.utils import get_query_string
 
 
 @pytest.fixture
 def fixtures(db):
     from demo.factories import ArtistFactory, BandFactory
-    band1 = BandFactory(id=1, name='band1')
-    band2 = BandFactory(id=2, name='band2')
-    band3 = BandFactory(id=3, name='band3')
-    ArtistFactory(name='a1', bands=[band1])
-    ArtistFactory(name='a2', bands=[band2])
-    ArtistFactory(name='a3', bands=[band3])
-    ArtistFactory(name='a12', bands=[band1, band2])
-    ArtistFactory(name='a23', bands=[band2, band3])
-
-
-@pytest.mark.parametrize('value,expected', [('1', ['a1', 'a12']),
-                                            ('2', ['a12', 'a2', 'a23']),
-                                            ('1,2', ['a1', 'a12', 'a2', 'a23']),
-                                            ('2,3', ['a12', 'a2', 'a23', 'a3']),
-                                            ('', ['a1', 'a12', 'a2', 'a23', 'a3']),
-                                            ])
+
+    band1 = BandFactory(id=1, name="band1")
+    band2 = BandFactory(id=2, name="band2")
+    band3 = BandFactory(id=3, name="band3")
+    ArtistFactory(name="a1", bands=[band1])
+    ArtistFactory(name="a2", bands=[band2])
+    ArtistFactory(name="a3", bands=[band3])
+    ArtistFactory(name="a12", bands=[band1, band2])
+    ArtistFactory(name="a23", bands=[band2, band3])
+
+
+@pytest.mark.parametrize(
+    "value,expected",
+    [
+        ("1", ["a1", "a12"]),
+        ("2", ["a12", "a2", "a23"]),
+        ("1,2", ["a1", "a12", "a2", "a23"]),
+        ("2,3", ["a12", "a2", "a23", "a3"]),
+        ("", ["a1", "a12", "a2", "a23", "a3"]),
+    ],
+)
 def test_union(fixtures, value, expected):
-    f = UnionFieldListFilter(Artist._meta.get_field('bands'), None,
-                             {'bands_filter': value}, None, None, 'bands')
-    result = f.queryset(None, Artist.objects.order_by('name'))
-    value = list(result.order_by('name').values_list('name', flat=True))
+    f = UnionFieldListFilter(
+        Artist._meta.get_field("bands"),
+        None,
+        {"bands_filter": value},
+        None,
+        None,
+        "bands",
+    )
+    result = f.queryset(None, Artist.objects.order_by("name"))
+    value = list(result.order_by("name").values_list("name", flat=True))
     assert value == expected
 
 
-@pytest.mark.parametrize('value,expected', [('1', ['a1', 'a12']),
-                                            ('2', ['a12', 'a2', 'a23']),
-                                            ('1,2', ['a12']),
-                                            ('2,3', ['a23']),
-                                            ('', ['a1', 'a12', 'a2', 'a23', 'a3']),
-                                            ])
+@pytest.mark.parametrize(
+    "value,expected",
+    [
+        ("1", ["a1", "a12"]),
+        ("2", ["a12", "a2", "a23"]),
+        ("1,2", ["a12"]),
+        ("2,3", ["a23"]),
+        ("", ["a1", "a12", "a2", "a23", "a3"]),
+    ],
+)
 def test_intersection(fixtures, value, expected):
-    f = IntersectionFieldListFilter(Artist._meta.get_field('bands'), None,
-                                    {'bands_filter': value}, None, None, 'bands')
-    result = f.queryset(None, Artist.objects.order_by('name'))
-    value = list(result.order_by('name').values_list('name', flat=True))
+    f = IntersectionFieldListFilter(
+        Artist._meta.get_field("bands"),
+        None,
+        {"bands_filter": value},
+        None,
+        None,
+        "bands",
+    )
+    result = f.queryset(None, Artist.objects.order_by("name"))
+    value = list(result.order_by("name").values_list("name", flat=True))
     assert value == expected
 
 
 def test_choices(fixtures):
-    params = {'bands_filter': '1,2'}
-    f = IntersectionFieldListFilter(Artist._meta.get_field('bands'), None,
-                                    params, None, None, 'bands')
+    params = {"bands_filter": "1,2"}
+    f = IntersectionFieldListFilter(
+        Artist._meta.get_field("bands"), None, params, None, None, "bands"
+    )
     # result = f.queryset(None, Artist.objects.order_by('name'))
-    cl = Mock(get_query_string=partial(get_query_string, Mock(GET=params)),
-              params=params)
+    cl = Mock(
+        get_query_string=partial(get_query_string, Mock(GET=params)), params=params
+    )
     choices = list(f.choices(cl))
     assert len(choices) == 4
-    assert choices[0] == {'display': 'All', 'query_string': '?', 'selected': False}
-    assert choices[1] == {'display': 'band1', 'query_string': '?bands_filter=2', 'selected': True}
-    assert choices[2] == {'display': 'band2', 'query_string': '?bands_filter=1', 'selected': True}
+    assert choices[0] == {"display": "All", "query_string": "?", "selected": False}
+    assert choices[1] == {
+        "display": "band1",
+        "query_string": "?bands_filter=2",
+        "selected": True,
+    }
+    assert choices[2] == {
+        "display": "band2",
+        "query_string": "?bands_filter=1",
+        "selected": True,
+    }
```

### Comparing `django-adminfilters-2.1.0/tests/test_number.py` & `django-adminfilters-2.2.0/tests/test_number.py`

 * *Files 19% similar despite different names*

```diff
@@ -3,38 +3,51 @@
 
 from adminfilters.numbers import NumberFilter
 
 
 @pytest.fixture
 def fixtures(db):
     from demo.utils import DATA
+
     for i in range(1, 5):
         values = DATA.copy()
-        values['unique'] = i
+        values["unique"] = i
+        values["json"] = {}
         DemoModelField.objects.create(**values)
 
 
-@pytest.mark.parametrize('op,expected', [('=1', '1'),
-                                         ('1', '1'),
-                                         ('>1', '2,3,4'),
-                                         ('>=1', '1,2,3,4'),
-                                         ('<>2', '1,3,4'),
-                                         ('<2', '1'),
-                                         ('<=2', '1,2'),
-                                         ('1,3', '1,3'),
-                                         ('2..4', '2,3,4'),
-                                         ])
+@pytest.mark.parametrize(
+    "op,expected",
+    [
+        ("=1", "1"),
+        ("1", "1"),
+        (">1", "2,3,4"),
+        (">=1", "1,2,3,4"),
+        ("<>2", "1,3,4"),
+        ("<2", "1"),
+        ("<=2", "1,2"),
+        ("1,3", "1,3"),
+        ("2..4", "2,3,4"),
+    ],
+)
 def test_NumberFilter(fixtures, op, expected):
-    f = NumberFilter(DemoModelField._meta.get_field('unique'), None, {'unique': op}, None, None, 'unique')
+    f = NumberFilter(
+        DemoModelField._meta.get_field("unique"),
+        None,
+        {"unique": op},
+        None,
+        None,
+        "unique",
+    )
     assert f.value() == [op]
     result = f.queryset(None, DemoModelField.objects.all())
-    value = list(result.values_list('unique', flat=True))
-    assert value == expected.split(','), f.error_message
+    value = list(result.values_list("unique", flat=True))
+    assert value == expected.split(","), f.error_message
 
 
 def test_factory(fixtures):
-    assert NumberFilter.factory(title='CustomTitle')
+    assert NumberFilter.factory(title="CustomTitle")
 
 
 def test_factory_invalid(fixtures):
     with pytest.raises(ValueError):
-        assert NumberFilter.factory(title='CustomTitle', lookup_name='in')
+        assert NumberFilter.factory(title="CustomTitle", lookup_name="in")
```

### Comparing `django-adminfilters-2.1.0/tests/test_related.py` & `django-adminfilters-2.2.0/tests/test_related.py`

 * *Files 16% similar despite different names*

```diff
@@ -8,50 +8,74 @@
 from django.contrib.admin import site
 
 from adminfilters.checkbox import RelatedFieldCheckBoxFilter
 
 
 @pytest.fixture
 def fixtures(db):
-    ArtistFactory(name='name1', bands=[])
+    ArtistFactory(name="name1", bands=[])
     return sample_data()
 
 
 def test_RelatedFieldCheckBoxFilte_single(fixtures, rf):
     acdc, geordie = fixtures
-    request = rf.get(f'/?bands__id={geordie.id}')
-    f = RelatedFieldCheckBoxFilter(Artist._meta.get_field('bands'), request,
-                                   {}, None, ArtistModelAdmin(Artist, site), 'bands')
+    request = rf.get(f"/?bands__id={geordie.id}")
+    f = RelatedFieldCheckBoxFilter(
+        Artist._meta.get_field("bands"),
+        request,
+        {},
+        None,
+        ArtistModelAdmin(Artist, site),
+        "bands",
+    )
     result = f.queryset(None, Artist.objects.all())
 
-    value = sorted(list(result.values_list('name', flat=True)))
-    assert value == ['Brian']
+    value = sorted(list(result.values_list("name", flat=True)))
+    assert value == ["Brian"]
 
 
 def test_RelatedFieldCheckBoxFilte_multi(fixtures, rf):
     acdc, geordie = fixtures
-    request = rf.get(f'/?bands__id={acdc.id}&bands_id={geordie.id}')
-    f = RelatedFieldCheckBoxFilter(Artist._meta.get_field('bands'), request,
-                                   {}, None, ArtistModelAdmin(Artist, site), 'bands')
+    request = rf.get(f"/?bands__id={acdc.id}&bands_id={geordie.id}")
+    f = RelatedFieldCheckBoxFilter(
+        Artist._meta.get_field("bands"),
+        request,
+        {},
+        None,
+        ArtistModelAdmin(Artist, site),
+        "bands",
+    )
     result = f.queryset(None, Artist.objects.all())
 
-    value = sorted(list(result.values_list('name', flat=True)))
-    assert value == ['Angus', 'Bon', 'Brian', 'Malcom', 'Phil']
+    value = sorted(list(result.values_list("name", flat=True)))
+    assert value == ["Angus", "Bon", "Brian", "Malcom", "Phil"]
 
 
 def test_RelatedFieldCheckBoxFilte_isnull(fixtures, rf):
-    request = rf.get('/?bands__isnull=true')
-    f = RelatedFieldCheckBoxFilter(Artist._meta.get_field('bands'), request,
-                                   {'bands__isnull': 'true'}, None, ArtistModelAdmin(Artist, site), 'bands')
+    request = rf.get("/?bands__isnull=true")
+    f = RelatedFieldCheckBoxFilter(
+        Artist._meta.get_field("bands"),
+        request,
+        {"bands__isnull": "true"},
+        None,
+        ArtistModelAdmin(Artist, site),
+        "bands",
+    )
     result = f.queryset(None, Artist.objects.all())
 
-    value = sorted(list(result.values_list('name', flat=True)))
-    assert value == ['name1']
+    value = sorted(list(result.values_list("name", flat=True)))
+    assert value == ["name1"]
 
 
 def test_RelatedFieldCheckBoxFilte_choices(fixtures, rf):
-    request = rf.get('/')
-    f = RelatedFieldCheckBoxFilter(Artist._meta.get_field('bands'), request,
-                                   {}, None, ArtistModelAdmin(Artist, site), 'bands')
+    request = rf.get("/")
+    f = RelatedFieldCheckBoxFilter(
+        Artist._meta.get_field("bands"),
+        request,
+        {},
+        None,
+        ArtistModelAdmin(Artist, site),
+        "bands",
+    )
     choices = list(f.choices(Mock()))
     assert len(choices) == 4
-    assert [c['display'] for c in choices] == ['All', 'None', 'AC/DC', 'Geordie']
+    assert [c["display"] for c in choices] == ["All", "None", "AC/DC", "Geordie"]
```

### Comparing `django-adminfilters-2.1.0/tests/test_value.py` & `django-adminfilters-2.2.0/tests/test_value.py`

 * *Files 27% similar despite different names*

```diff
@@ -3,52 +3,81 @@
 
 from adminfilters.filters import MultiValueFilter, ValueFilter
 
 
 @pytest.fixture
 def fixtures(db):
     from demo.factories import ArtistFactory
-    ArtistFactory(name='a1')
-    ArtistFactory(name='a2')
-    ArtistFactory(name='b1')
-    ArtistFactory(name='c1')
+
+    ArtistFactory(name="a1")
+    ArtistFactory(name="a2")
+    ArtistFactory(name="b1")
+    ArtistFactory(name="c1")
 
 
 def test_media():
-    assert ValueFilter.factory(title='Title')(None, None, {}, None, None, 'unique').media
+    assert ValueFilter.factory(title="Title")(
+        None, None, {}, None, None, "unique"
+    ).media
 
 
-@pytest.mark.parametrize('value,negate,expected', [('n', False, []),
-                                                   ('a1', False, ['a1']),
-                                                   ('a1', True, ['a2', 'b1', 'c1']),
-                                                   ])
+@pytest.mark.parametrize(
+    "value,negate,expected",
+    [
+        ("n", False, []),
+        ("a1", False, ["a1"]),
+        ("a1", True, ["a2", "b1", "c1"]),
+    ],
+)
 def test_value_filter(fixtures, value, negate, expected):
-    f = ValueFilter(Artist._meta.get_field('name'), None,
-                    {'name__exact': value, 'name__exact__negate': str(negate).lower()}, None, None, 'name')
+    f = ValueFilter(
+        Artist._meta.get_field("name"),
+        None,
+        {"name__exact": value, "name__exact__negate": str(negate).lower()},
+        None,
+        None,
+        "name",
+    )
 
     result = f.queryset(None, Artist.objects.all())
-    value = list(result.values_list('name', flat=True))
+    value = list(result.values_list("name", flat=True))
     assert value == expected
 
 
 def test_factory(fixtures):
-    F = ValueFilter.factory(title='CustomTitle')
-    f = F(Artist._meta.get_field('name'), None,
-          {'name__exact': 'a1', 'name__exact__negate': 'false'}, None, None, 'name')
+    F = ValueFilter.factory(title="CustomTitle")
+    f = F(
+        Artist._meta.get_field("name"),
+        None,
+        {"name__exact": "a1", "name__exact__negate": "false"},
+        None,
+        None,
+        "name",
+    )
 
-    assert f.value() == ['a1', False]
+    assert f.value() == ["a1", False]
     result = f.queryset(None, Artist.objects.all())
-    value = list(result.values_list('name', flat=True))
-    assert value == ['a1']
+    value = list(result.values_list("name", flat=True))
+    assert value == ["a1"]
 
 
-@pytest.mark.parametrize('value,negate,expected', [('n', False, []),
-                                                   ('a1', False, ['a1']),
-                                                   ('a1', True, ['a2', 'b1', 'c1']),
-                                                   ])
+@pytest.mark.parametrize(
+    "value,negate,expected",
+    [
+        ("n", False, []),
+        ("a1", False, ["a1"]),
+        ("a1", True, ["a2", "b1", "c1"]),
+    ],
+)
 def test_MultiValueTextFieldFilter(fixtures, value, negate, expected):
-    f = MultiValueFilter(Artist._meta.get_field('name'), None,
-                         {'name__in': value, 'name__in__negate': str(negate).lower()}, None, None, 'name')
+    f = MultiValueFilter(
+        Artist._meta.get_field("name"),
+        None,
+        {"name__in": value, "name__in__negate": str(negate).lower()},
+        None,
+        None,
+        "name",
+    )
     assert f.value() == [[value], negate]
     result = f.queryset(None, Artist.objects.all())
-    value = list(result.values_list('name', flat=True))
+    value = list(result.values_list("name", flat=True))
     assert value == expected
```

### Comparing `django-adminfilters-2.1.0/tox.ini` & `django-adminfilters-2.2.0/tox.ini`

 * *Files 19% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 [tox]
-envlist = py{39,310}-d{32,40}
+envlist = d{32,41}-py{39,310,311}
 skip_missing_interpreters = true
 
 [pytest]
 ;python_paths=./tests/demoapp
 django_find_project = false
 log_format = %(asctime)s %(levelname)s %(message)s
 log_level = CRITICAL
@@ -16,31 +16,44 @@
 
 markers =
     selenium: Run selenium functional tests
 filterwarnings =
     ignore::DeprecationWarning
 
 [testenv:lint]
+envdir={toxworkdir}/d32-py39/
+skip_install = true
+deps=
+;    black
+;    flake8
+;    isort
+    -rsrc/requirements/testing.pip
+    -rsrc/requirements/develop.pip
+    pre-commit
+
 commands =
-    flake8 --config .flake8 src/ tests/
-    isort -c src/ tests/
+;    black --check ./src ./tests
+    pre-commit run --all-files
+;    flake8 src tests
+;    isort src tests --check --settings .isort.cfg
 
 [testenv]
 passenv =
     PYTHONPATH
     DATABASE_URL
 
 setenv =
 whitelist_externals = mkdir
 
 deps =
     -rsrc/requirements/testing.pip
     d22: django==2.2.*
     d32: django==3.2.*
     d40: django==4.0.*
+    d41: django==4.1.*
 
 commands =
     {posargs:py.test tests/ --create-db --selenium --cov-report=xml --cov-report=term --junitxml=pytest.xml \
     --cov-config=tests/.coveragerc --cov adminfilters}
 
 [testenv:package]
 deps=
```

