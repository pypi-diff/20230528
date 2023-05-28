# Comparing `tmp/djangocms-frontend-1.1.3.tar.gz` & `tmp/djangocms-frontend-1.1.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "djangocms-frontend-1.1.3.tar", last modified: Fri May 26 17:21:32 2023, max compression
+gzip compressed data, was "djangocms-frontend-1.1.4.tar", last modified: Sun May 28 18:01:35 2023, max compression
```

## Comparing `djangocms-frontend-1.1.3.tar` & `djangocms-frontend-1.1.4.tar`

### file list

```diff
@@ -1,686 +1,686 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend/
--rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/cms_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend/common/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/attributes.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/background.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/background.py
--rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/responsive.py
--rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/sizing.py
--rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/spacing.py
--rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/common/title.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.534249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.534249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
--rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.558249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
--rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
--rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
--rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
--rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.562250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
--rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
--rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.538249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
--rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
--rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/foundation6.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.566249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
--rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/conf.py
--rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.570249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
--rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.586250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
--rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
--rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
--rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
--rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
--rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
--rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
--rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-05-26 17:21:23.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
--rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
--rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
--rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
--rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
--rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
--rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
--rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
--rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
--rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
--rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
--rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.594250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
--rw-r--r--   0 runner    (1001) docker     (123)    48146 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    30533 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
--rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
--rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
--rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
--rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
--rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
--rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
--rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
--rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
--rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
--rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
--rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
--rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
--rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.594250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
--rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
--rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.594250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
--rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
--rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.594250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
--rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
--rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
--rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
--rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
--rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
--rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
--rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
--rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
--rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.598250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.542249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.602250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
--rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/
--rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/apps.py
--rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
--rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
--rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.606250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.610250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
--rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
--rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
--rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
--rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.546249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
--rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.614250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/cms_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/forms.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
--rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
--rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
--rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/fields.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/frameworks/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/frameworks/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/frameworks/bootstrap5.py
--rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/de/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/en/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/locale/en/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/en/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/fr/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/locale/fr/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
--rw-r--r--   0 runner    (1001) docker     (123)    39659 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.618250 djangocms-frontend-1.1.3/djangocms_frontend/management/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/bootstrap4_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
--rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/migrate.py
--rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/stale_references.py
--rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/sync_permissions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/icon_migration.py
--rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/management/styled_link_migration.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/migrations/0001_initial.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/settings.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.550249 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/
--rw-r--r--   0 runner    (1001) docker     (123)    93571 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/base.css
--rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/base.css.map
--rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/button_group.css
--rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
--rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/div_select.css
--rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/select2.css
--rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/
--rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
--rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
--rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
--rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
--rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.622250 djangocms-frontend-1.1.3/djangocms_frontend/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/
--rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/base.html
--rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/dropdown.html
--rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/menu.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/
--rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/base.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/includes/
--rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
--rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
--rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/html_container.html
--rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend.html
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/djangocms_frontend/templatetags/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templatetags/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/djangocms_frontend/templatetags/frontend.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.554249 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)    33033 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-26 17:21:32.000000 djangocms-frontend-1.1.3/djangocms_frontend.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.626250 djangocms-frontend-1.1.3/tests/accordion/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/accordion/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/accordion/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/accordion/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/alert/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/alert/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/alert/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/alert/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/badge/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/badge/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/badge/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/badge/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/card/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/card/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/card/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/card/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/carousel/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/carousel/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/carousel/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/carousel/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/collapse/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/collapse/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/collapse/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/collapse/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/content/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/content/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/content/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/content/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/fixtures.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/grid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/grid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/grid/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/grid/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/helpers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/icon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/icon/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/icon/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/icon/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.630250 djangocms-frontend-1.1.3/tests/image/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/image/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/image/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/image/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/jumbotron/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/jumbotron/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/jumbotron/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/jumbotron/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/link/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/link/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/link/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/link/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/listgroup/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/listgroup/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/listgroup/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/listgroup/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/media/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/media/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/media/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/media/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/navigation/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/navigation/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/navigation/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/navigation/test_plugins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/tabs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/tabs/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/tabs/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/tabs/test_plugins.py
--rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_fields.py
--rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_migrations.py
--rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/test_settings.py
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/urls.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:32.634250 djangocms-frontend-1.1.3/tests/utilities/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/utilities/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/utilities/test_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-26 17:21:24.000000 djangocms-frontend-1.1.3/tests/utilities/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.044579 djangocms-frontend-1.1.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1475 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-28 18:01:35.044579 djangocms-frontend-1.1.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6470 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.904573 djangocms-frontend-1.1.4/djangocms_frontend/
+-rw-r--r--   0 runner    (1001) docker     (123)      986 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/cms_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.904573 djangocms-frontend-1.1.4/djangocms_frontend/common/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      859 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/attributes.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/background.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.908573 djangocms-frontend-1.1.4/djangocms_frontend/common/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/bootstrap5/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/bootstrap5/background.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2095 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/bootstrap5/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/bootstrap5/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/responsive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/sizing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7879 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/spacing.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/common/title.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.908573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.908573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2788 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2617 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.908573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      869 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.908573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      919 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      867 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.868572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.868572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.912573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      358 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1201 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.912573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1053 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1602 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.912573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1635 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)      451 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.912573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      397 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.868572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.868572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.912573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/djangocms_frontend/admin/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.912573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      513 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.912573 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.916574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1002 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1339 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.916574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      289 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.916574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      570 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.868572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.916574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.916574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/templates/djangocms_frontend/admin/badge.html
+-rw-r--r--   0 runner    (1001) docker     (123)      126 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/templates/djangocms_frontend/badge.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.920574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4500 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6606 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.920574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1578 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2029 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.920574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1626 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.872572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.872572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.920574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card.html
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.920574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      665 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.920574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2906 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      897 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5779 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.924574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1358 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.924574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1178 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2299 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.872572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.872572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.924574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/admin/carousel.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.872572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.872572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.924574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html
+-rw-r--r--   0 runner    (1001) docker     (123)      661 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html
+-rw-r--r--   0 runner    (1001) docker     (123)      843 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.924574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2665 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.924574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      481 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.924574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1272 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1353 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.872572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.872572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.928574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      283 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/admin/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.928574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      544 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html
+-rw-r--r--   0 runner    (1001) docker     (123)      487 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.928574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2567 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      235 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3743 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.928574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      873 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.928574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1241 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.928574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.932574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      784 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html
+-rw-r--r--   0 runner    (1001) docker     (123)      239 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/code.html
+-rw-r--r--   0 runner    (1001) docker     (123)      467 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/figure.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.932574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5220 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7853 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.932574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2609 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2017 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/frameworks/foundation6.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.932574 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2480 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.936575 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      900 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html
+-rw-r--r--   0 runner    (1001) docker     (123)      249 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      732 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.936575 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      450 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/djangocms_frontend/bootstrap5/grid_row.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.936575 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1310 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2155 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/conf.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1522 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.936575 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.936575 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      434 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.936575 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/
+-rw-r--r--   0 runner    (1001) docker     (123)       69 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/ckeditor/ckeditor.icons.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.960575 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/
+-rw-r--r--   0 runner    (1001) docker     (123)    59572 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   277297 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    59388 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    63664 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   123564 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   516494 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   123376 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   123452 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    89988 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    76736 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   101648 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    78268 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    16276 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    13224 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    54568 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   150535 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    56976 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    32020 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   643290 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   127824 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   103304 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)   105448 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   304476 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   105284 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   105360 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    28196 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot
+-rw-r--r--   0 runner    (1001) docker     (123)    20996 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf
+-rw-r--r--   0 runner    (1001) docker     (123)    54789 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    28028 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    14984 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   729984 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot
+-rw-r--r--   0 runner    (1001) docker     (123)  2883039 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg
+-rw-r--r--   0 runner    (1001) docker     (123)   729800 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)   386256 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff
+-rw-r--r--   0 runner    (1001) docker     (123)   282928 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    99774 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   184969 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    99564 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    56468 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff
+-rw-r--r--   0 runner    (1001) docker     (123)    44720 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2
+-rw-r--r--   0 runner    (1001) docker     (123)    45816 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot
+-rw-r--r--   0 runner    (1001) docker     (123)   132305 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg
+-rw-r--r--   0 runner    (1001) docker     (123)    45648 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf
+-rw-r--r--   0 runner    (1001) docker     (123)    45724 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.972576 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/
+-rw-r--r--   0 runner    (1001) docker     (123)    48146 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30533 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    10004 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6733 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5917 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    48978 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35481 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6934 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5542 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2855 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2357 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    18498 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15099 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    30092 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json
+-rw-r--r--   0 runner    (1001) docker     (123)    23027 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6237 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3659 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8409 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     6765 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     9789 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json
+-rw-r--r--   0 runner    (1001) docker     (123)     5339 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24992 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15565 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    24997 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15570 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    25003 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json
+-rw-r--r--   0 runner    (1001) docker     (123)    15576 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4845 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2807 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    35227 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)    21372 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)    14032 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     8718 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json
+-rw-r--r--   0 runner    (1001) docker     (123)     4936 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2925 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.972576 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/
+-rw-r--r--   0 runner    (1001) docker     (123)      631 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      872 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg
+-rw-r--r--   0 runner    (1001) docker     (123)      645 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.976576 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    21397 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js
+-rw-r--r--   0 runner    (1001) docker     (123)    12890 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    11580 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.976576 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/
+-rw-r--r--   0 runner    (1001) docker     (123)    10722 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.984577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/
+-rw-r--r--   0 runner    (1001) docker     (123)    30045 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    28165 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15830 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    13288 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)   137737 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)   115209 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20997 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    18213 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    27048 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    21866 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    24776 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css
+-rw-r--r--   0 runner    (1001) docker     (123)    20593 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12126 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css
+-rw-r--r--   0 runner    (1001) docker     (123)    10110 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    77647 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    65062 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9566 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css
+-rw-r--r--   0 runner    (1001) docker     (123)     9348 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    32569 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    26765 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)    15463 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css
+-rw-r--r--   0 runner    (1001) docker     (123)    12839 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.876572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.984577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)     3255 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.984577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      423 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/djangocms_frontend/bootstrap5/icon.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.984577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)      140 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/djangocms_frontend/icon/add_css.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.984577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      673 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templatetags/icon_tags.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.984577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9218 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.984577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1145 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.984577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      830 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5588 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.984577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/templates/djangocms_frontend/admin/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.988577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.988577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1410 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1648 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.988577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.988577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      578 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      486 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.988577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/admin/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.988577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      496 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/templates/djangocms_frontend/bootstrap5/jumbotron/default/jumbotron.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.992577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/
+-rw-r--r--   0 runner    (1001) docker     (123)      144 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      947 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/apps.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3304 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      536 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13530 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.992577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4602 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.992577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      568 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4675 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.992577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.880572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.884572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.992577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/admin/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.884572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.884572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.992577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      646 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.884572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.884572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.992577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/icon.html
+-rw-r--r--   0 runner    (1001) docker     (123)      741 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)      912 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.992577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1883 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      148 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2505 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.992577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      674 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.996577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      959 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.884572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.884572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.996577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/templates/djangocms_frontend/admin/list-group.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.996577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1319 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1067 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.996577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.996577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      904 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      640 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.000577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      278 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/templates/djangocms_frontend/admin/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.000577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      485 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/templates/djangocms_frontend/bootstrap5/media.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.000577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4991 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3548 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.000577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.000577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1934 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.004577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      115 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      118 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/navlink.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/admin/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.004577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1652 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      809 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      119 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.008577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/
+-rw-r--r--   0 runner    (1001) docker     (123)      593 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1647 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html
+-rw-r--r--   0 runner    (1001) docker     (123)      944 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu_dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      942 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)      755 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html
+-rw-r--r--   0 runner    (1001) docker     (123)      121 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/page_tree.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.008577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2140 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)      690 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2864 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.008577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      991 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.008577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)      896 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      647 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.008577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      131 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/admin/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.888572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.008577 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/item.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1332 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.012578 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4053 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/cms_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5352 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/forms.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.012578 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.012578 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1250 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1737 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.892572 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.012578 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.012578 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      214 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/no_form.html
+-rw-r--r--   0 runner    (1001) docker     (123)      252 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/admin/spacing.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.012578 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)      922 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html
+-rw-r--r--   0 runner    (1001) docker     (123)      589 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/toc.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.012578 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      395 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templatetags/fe_utilities.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6935 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/fields.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.012578 djangocms-frontend-1.1.4/djangocms_frontend/frameworks/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/frameworks/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4374 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/frameworks/bootstrap5.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4763 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.892572 djangocms-frontend-1.1.4/djangocms_frontend/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.892572 djangocms-frontend-1.1.4/djangocms_frontend/locale/de/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.016578 djangocms-frontend-1.1.4/djangocms_frontend/locale/de/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    26790 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    44731 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/locale/de/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.892572 djangocms-frontend-1.1.4/djangocms_frontend/locale/en/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.016578 djangocms-frontend-1.1.4/djangocms_frontend/locale/en/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)      378 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    34046 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/locale/en/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.892572 djangocms-frontend-1.1.4/djangocms_frontend/locale/fr/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.016578 djangocms-frontend-1.1.4/djangocms_frontend/locale/fr/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    46281 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/locale/fr/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.892572 djangocms-frontend-1.1.4/djangocms_frontend/locale/sq/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.016578 djangocms-frontend-1.1.4/djangocms_frontend/locale/sq/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)    15741 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo
+-rw-r--r--   0 runner    (1001) docker     (123)    39659 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/locale/sq/LC_MESSAGES/django.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.016578 djangocms-frontend-1.1.4/djangocms_frontend/management/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17900 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/bootstrap4_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.020578 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      905 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.020578 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4130 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      603 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/frequency_analysis.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9951 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/migrate.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1656 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/stale_references.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6068 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/sync_permissions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4880 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/icon_migration.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2960 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/management/styled_link_migration.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.020578 djangocms-frontend-1.1.4/djangocms_frontend/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)     1908 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/migrations/0001_initial.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3478 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4236 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/settings.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.896573 djangocms-frontend-1.1.4/djangocms_frontend/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.896573 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.024578 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/
+-rw-r--r--   0 runner    (1001) docker     (123)    78932 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/base.css
+-rw-r--r--   0 runner    (1001) docker     (123)     8035 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/base.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)     5121 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/button_group.css
+-rw-r--r--   0 runner    (1001) docker     (123)      816 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map
+-rw-r--r--   0 runner    (1001) docker     (123)      142 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/div_select.css
+-rw-r--r--   0 runner    (1001) docker     (123)      630 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/select2.css
+-rw-r--r--   0 runner    (1001) docker     (123)      190 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/select2.css.map
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.024578 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/
+-rw-r--r--   0 runner    (1001) docker     (123)     1156 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/auto_input.js
+-rw-r--r--   0 runner    (1001) docker     (123)    13738 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js
+-rw-r--r--   0 runner    (1001) docker     (123)    95562 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js
+-rw-r--r--   0 runner    (1001) docker     (123)     4260 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js
+-rw-r--r--   0 runner    (1001) docker     (123)     2708 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/django_select2.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.024578 djangocms-frontend-1.1.4/djangocms_frontend/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.028578 djangocms-frontend-1.1.4/djangocms_frontend/templates/bootstrap5/
+-rw-r--r--   0 runner    (1001) docker     (123)     2392 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/bootstrap5/base.html
+-rw-r--r--   0 runner    (1001) docker     (123)      290 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/bootstrap5/dropdown.html
+-rw-r--r--   0 runner    (1001) docker     (123)      911 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/bootstrap5/menu.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.028578 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.028578 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/
+-rw-r--r--   0 runner    (1001) docker     (123)      463 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/base-collapse.html
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html
+-rw-r--r--   0 runner    (1001) docker     (123)       73 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/base.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.028578 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/includes/
+-rw-r--r--   0 runner    (1001) docker     (123)     1842 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.028578 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/
+-rw-r--r--   0 runner    (1001) docker     (123)      597 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      542 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)      586 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/select.html
+-rw-r--r--   0 runner    (1001) docker     (123)      349 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/html_container.html
+-rw-r--r--   0 runner    (1001) docker     (123)     1882 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend.html
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.028578 djangocms-frontend-1.1.4/djangocms_frontend/templatetags/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templatetags/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3383 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/djangocms_frontend/templatetags/frontend.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:34.904573 djangocms-frontend-1.1.4/djangocms_frontend.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8608 2023-05-28 18:01:34.000000 djangocms-frontend-1.1.4/djangocms_frontend.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)    33033 2023-05-28 18:01:34.000000 djangocms-frontend-1.1.4/djangocms_frontend.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:01:34.000000 djangocms-frontend-1.1.4/djangocms_frontend.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 18:01:34.000000 djangocms-frontend-1.1.4/djangocms_frontend.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      317 2023-05-28 18:01:34.000000 djangocms-frontend-1.1.4/djangocms_frontend.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-28 18:01:34.000000 djangocms-frontend-1.1.4/djangocms_frontend.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      560 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)      339 2023-05-28 18:01:35.044579 djangocms-frontend-1.1.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2889 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.032579 djangocms-frontend-1.1.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.032579 djangocms-frontend-1.1.4/tests/accordion/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/accordion/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      799 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/accordion/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2588 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/accordion/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.032579 djangocms-frontend-1.1.4/tests/alert/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/alert/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      443 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/alert/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1164 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/alert/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.036579 djangocms-frontend-1.1.4/tests/badge/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/badge/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      419 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/badge/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2014 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/badge/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.036579 djangocms-frontend-1.1.4/tests/card/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/card/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1147 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/card/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3710 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/card/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.036579 djangocms-frontend-1.1.4/tests/carousel/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/carousel/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2229 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/carousel/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4278 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/carousel/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.036579 djangocms-frontend-1.1.4/tests/collapse/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/collapse/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/collapse/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2731 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/collapse/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.036579 djangocms-frontend-1.1.4/tests/content/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/content/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1082 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/content/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2804 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/content/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4723 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/fixtures.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.040579 djangocms-frontend-1.1.4/tests/grid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/grid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1696 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/grid/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5264 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/grid/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3360 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/helpers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.040579 djangocms-frontend-1.1.4/tests/icon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/icon/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/icon/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)      967 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/icon/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.040579 djangocms-frontend-1.1.4/tests/image/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/image/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      429 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/image/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3124 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/image/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.040579 djangocms-frontend-1.1.4/tests/jumbotron/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/jumbotron/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      508 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/jumbotron/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1275 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/jumbotron/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.040579 djangocms-frontend-1.1.4/tests/link/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/link/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      465 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/link/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6382 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/link/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.040579 djangocms-frontend-1.1.4/tests/listgroup/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/listgroup/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1175 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/listgroup/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3020 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/listgroup/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.044579 djangocms-frontend-1.1.4/tests/media/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/media/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      541 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/media/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1186 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/media/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.044579 djangocms-frontend-1.1.4/tests/navigation/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/navigation/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1056 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/navigation/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3931 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/navigation/test_plugins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.044579 djangocms-frontend-1.1.4/tests/tabs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/tabs/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      767 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/tabs/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1612 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/tabs/test_plugins.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1742 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/test_constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/test_fields.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5455 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/test_helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)      898 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/test_migrations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3463 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/test_settings.py
+-rw-r--r--   0 runner    (1001) docker     (123)      162 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/urls.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:35.044579 djangocms-frontend-1.1.4/tests/utilities/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/utilities/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1192 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/utilities/test_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3217 2023-05-28 18:01:23.000000 djangocms-frontend-1.1.4/tests/utilities/test_plugins.py
```

### Comparing `djangocms-frontend-1.1.3/LICENSE` & `djangocms-frontend-1.1.4/LICENSE`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/PKG-INFO` & `djangocms-frontend-1.1.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.3
+Version: 1.1.4
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-frontend-1.1.3/README.rst` & `djangocms-frontend-1.1.4/README.rst`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/__init__.py` & `djangocms-frontend-1.1.4/djangocms_frontend/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -15,8 +15,8 @@
  9. git push
 10. Assure that all tests pass on https://github.com/django-cms/djangocms-frontend/actions
 11. Create a new release on https://github.com/django-cms/djangocms-frontend/releases/new
 12. Publish the release when ready
 13. Github actions will publish the new package to pypi
 """
 
-__version__ = "1.1.3"
+__version__ = "1.1.4"
```

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/common/attributes.py` & `djangocms-frontend-1.1.4/djangocms_frontend/common/attributes.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/background.py` & `djangocms-frontend-1.1.4/djangocms_frontend/common/bootstrap5/background.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/responsive.py` & `djangocms-frontend-1.1.4/djangocms_frontend/common/bootstrap5/responsive.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/common/bootstrap5/sizing.py` & `djangocms-frontend-1.1.4/djangocms_frontend/common/bootstrap5/sizing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/common/spacing.py` & `djangocms-frontend-1.1.4/djangocms_frontend/common/spacing.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/common/title.py` & `djangocms-frontend-1.1.4/djangocms_frontend/common/title.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/accordion/templates/djangocms_frontend/bootstrap5/accordion_item.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/djangocms_frontend/bootstrap5/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/alert/templates/djangocms_frontend/foundation6/alert.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/badge/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/badge/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/constants.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/frameworks/foundation6.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/templates/djangocms_frontend/admin/card_layout.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/card/templates/djangocms_frontend/bootstrap5/card.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/constants.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/carousel.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/carousel/templates/djangocms_frontend/bootstrap5/carousel/default/slide.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/collapse/templates/djangocms_frontend/bootstrap5/collapse-trigger.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/admin/code.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/content/templates/djangocms_frontend/bootstrap5/blockquote.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/constants.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/frameworks/foundation6.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/frameworks/foundation6.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_column.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/grid/templates/djangocms_frontend/admin/grid_row.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/conf.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/conf.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/fields.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/ElegantIcons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/feather-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-brand-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/fomantic-ui-outline-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/foundation-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/happy-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/icomoon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.otf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/open-iconic.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/tabler-icons.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/weathericons-regular-webfont.woff2`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.eot`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.ttf`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/fonts/zondicon.woff`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/bootstrap-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/elegant-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/feather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/fomantic-ui.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-brands.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-regular.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome-solid.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/font-awesome.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/foundation-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/happy-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/icomoon.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-filled.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-outlined.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-round.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-sharp.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/material-icons-two-tone.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/open-iconic.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/tabler-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/weather-icons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/icons-libraries/zondicons.min.json`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/magnifying-glass-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/star-of-life-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/images/xmark-solid.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/js/universal-icon-picker.min.js.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/scss/universal-icon-picker.scss`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/elegant-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/feather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/fomantic-ui-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/foundation-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/happy-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/icomoon.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/open-iconic.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/tabler-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/universal-icon-picker.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/weather-icons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/static/djangocms_frontend/icon/vendor/assets/stylesheets/zondicons.min.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templates/djangocms_frontend/admin/widgets/icon_picker.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/icon/templatetags/icon_tags.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/icon/templatetags/icon_tags.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/image/templates/djangocms_frontend/bootstrap5/default/image.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/jumbotron/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/apps.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/apps.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/constants.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/helpers.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/static/djangocms_text_ckeditor/icons/link.svg`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/bootstrap5/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/templates/djangocms_frontend/foundation6/link/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/link/views.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/link/views.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/listgroup/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/listgroup/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/media/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/media/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/default/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/brand.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/dropdown.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/link.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/nav_container.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/navigation/templates/djangocms_frontend/bootstrap5/navigation/offcanvas/navigation.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/constants.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/tabs/templates/djangocms_frontend/bootstrap5/tabs/default/tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/cms_plugins.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/cms_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/forms.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/forms.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/bootstrap5/editor_note.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html` & `djangocms-frontend-1.1.4/djangocms_frontend/contrib/utilities/templates/djangocms_frontend/heading.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/fields.py` & `djangocms-frontend-1.1.4/djangocms_frontend/fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/frameworks/bootstrap5.py` & `djangocms-frontend-1.1.4/djangocms_frontend/frameworks/bootstrap5.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/helpers.py` & `djangocms-frontend-1.1.4/djangocms_frontend/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.4/djangocms_frontend/locale/de/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/locale/de/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.4/djangocms_frontend/locale/de/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/locale/en/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.4/djangocms_frontend/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/locale/fr/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.4/djangocms_frontend/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo` & `djangocms-frontend-1.1.4/djangocms_frontend/locale/sq/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/locale/sq/LC_MESSAGES/django.po` & `djangocms-frontend-1.1.4/djangocms_frontend/locale/sq/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/management/bootstrap4_migration.py` & `djangocms-frontend-1.1.4/djangocms_frontend/management/bootstrap4_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/frontend.py` & `djangocms-frontend-1.1.4/djangocms_frontend/management/commands/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/base.py` & `djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/base.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/frequency_analysis.py` & `djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/frequency_analysis.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/migrate.py` & `djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/migrate.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/stale_references.py` & `djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/stale_references.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/management/commands/subcommands/sync_permissions.py` & `djangocms-frontend-1.1.4/djangocms_frontend/management/commands/subcommands/sync_permissions.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/management/icon_migration.py` & `djangocms-frontend-1.1.4/djangocms_frontend/management/icon_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/management/styled_link_migration.py` & `djangocms-frontend-1.1.4/djangocms_frontend/management/styled_link_migration.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/migrations/0001_initial.py` & `djangocms-frontend-1.1.4/djangocms_frontend/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/models.py` & `djangocms-frontend-1.1.4/djangocms_frontend/models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/settings.py` & `djangocms-frontend-1.1.4/djangocms_frontend/settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/base.css.map` & `djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/base.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/button_group.css` & `djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/button_group.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map` & `djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/button_group.css.map`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/css/select2.css` & `djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/css/select2.css`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/auto_input.js` & `djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/auto_input.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js` & `djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/bundle.base.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js` & `djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/bundle.grid.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js` & `djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/bundle.link.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/static/djangocms_frontend/js/django_select2.js` & `djangocms-frontend-1.1.4/djangocms_frontend/static/djangocms_frontend/js/django_select2.js`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/base.html` & `djangocms-frontend-1.1.4/djangocms_frontend/templates/bootstrap5/base.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templates/bootstrap5/menu.html` & `djangocms-frontend-1.1.4/djangocms_frontend/templates/bootstrap5/menu.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html` & `djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/base-tabs.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html` & `djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/includes/fieldset.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html` & `djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html` & `djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_color_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html` & `djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/button_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html` & `djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend/admin/widgets/icon_group_option.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templates/djangocms_frontend.html` & `djangocms-frontend-1.1.4/djangocms_frontend/templates/djangocms_frontend.html`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend/templatetags/frontend.py` & `djangocms-frontend-1.1.4/djangocms_frontend/templatetags/frontend.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend.egg-info/PKG-INFO` & `djangocms-frontend-1.1.4/djangocms_frontend.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: djangocms-frontend
-Version: 1.1.3
+Version: 1.1.4
 Summary: Adds abstract User Interface items as plugins to django CMS.
 Home-page: https://github.com/django-cms/djangocms-frontend
 Author: fsbraun
 Author-email: fsbraun@gmx.de
 Maintainer: Django CMS Association and contributors
 Maintainer-email: info@django-cms.org
 License: BSD-3-Clause
```

### Comparing `djangocms-frontend-1.1.3/djangocms_frontend.egg-info/SOURCES.txt` & `djangocms-frontend-1.1.4/djangocms_frontend.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/pyproject.toml` & `djangocms-frontend-1.1.4/pyproject.toml`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/setup.py` & `djangocms-frontend-1.1.4/setup.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/accordion/test_models.py` & `djangocms-frontend-1.1.4/tests/accordion/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/accordion/test_plugins.py` & `djangocms-frontend-1.1.4/tests/accordion/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/alert/test_plugins.py` & `djangocms-frontend-1.1.4/tests/alert/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/badge/test_plugins.py` & `djangocms-frontend-1.1.4/tests/badge/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/card/test_models.py` & `djangocms-frontend-1.1.4/tests/card/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/card/test_plugins.py` & `djangocms-frontend-1.1.4/tests/card/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/carousel/test_models.py` & `djangocms-frontend-1.1.4/tests/carousel/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/carousel/test_plugins.py` & `djangocms-frontend-1.1.4/tests/carousel/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/collapse/test_models.py` & `djangocms-frontend-1.1.4/tests/collapse/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/collapse/test_plugins.py` & `djangocms-frontend-1.1.4/tests/collapse/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/content/test_models.py` & `djangocms-frontend-1.1.4/tests/content/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/content/test_plugins.py` & `djangocms-frontend-1.1.4/tests/content/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/fixtures.py` & `djangocms-frontend-1.1.4/tests/fixtures.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/grid/test_models.py` & `djangocms-frontend-1.1.4/tests/grid/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/grid/test_plugins.py` & `djangocms-frontend-1.1.4/tests/grid/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/helpers.py` & `djangocms-frontend-1.1.4/tests/helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/icon/test_models.py` & `djangocms-frontend-1.1.4/tests/icon/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/icon/test_plugins.py` & `djangocms-frontend-1.1.4/tests/icon/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/image/test_plugins.py` & `djangocms-frontend-1.1.4/tests/image/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/jumbotron/test_plugins.py` & `djangocms-frontend-1.1.4/tests/jumbotron/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/link/test_plugins.py` & `djangocms-frontend-1.1.4/tests/link/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/listgroup/test_models.py` & `djangocms-frontend-1.1.4/tests/listgroup/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/listgroup/test_plugins.py` & `djangocms-frontend-1.1.4/tests/listgroup/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/media/test_models.py` & `djangocms-frontend-1.1.4/tests/media/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/media/test_plugins.py` & `djangocms-frontend-1.1.4/tests/media/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/navigation/test_models.py` & `djangocms-frontend-1.1.4/tests/navigation/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/navigation/test_plugins.py` & `djangocms-frontend-1.1.4/tests/navigation/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/tabs/test_models.py` & `djangocms-frontend-1.1.4/tests/tabs/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/tabs/test_plugins.py` & `djangocms-frontend-1.1.4/tests/tabs/test_plugins.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/test_constants.py` & `djangocms-frontend-1.1.4/tests/test_constants.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/test_fields.py` & `djangocms-frontend-1.1.4/tests/test_fields.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/test_helpers.py` & `djangocms-frontend-1.1.4/tests/test_helpers.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/test_migrations.py` & `djangocms-frontend-1.1.4/tests/test_migrations.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/test_settings.py` & `djangocms-frontend-1.1.4/tests/test_settings.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/utilities/test_models.py` & `djangocms-frontend-1.1.4/tests/utilities/test_models.py`

 * *Files identical despite different names*

### Comparing `djangocms-frontend-1.1.3/tests/utilities/test_plugins.py` & `djangocms-frontend-1.1.4/tests/utilities/test_plugins.py`

 * *Files identical despite different names*

