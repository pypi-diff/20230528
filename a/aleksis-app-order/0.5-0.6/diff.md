# Comparing `tmp/aleksis_app_order-0.5.tar.gz` & `tmp/aleksis_app_order-0.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "aleksis_app_order-0.5.tar", max compression
+gzip compressed data, was "aleksis_app_order-0.6.tar", max compression
```

## Comparing `aleksis_app_order-0.5.tar` & `aleksis_app_order-0.6.tar`

### file list

```diff
@@ -1,109 +1,109 @@
--rw-r--r--   0        0        0     2682 2023-03-04 17:04:56.553237 aleksis_app_order-0.5/CHANGELOG.rst
--rw-r--r--   0        0        0    14361 2020-12-13 09:29:37.493364 aleksis_app_order-0.5/LICENCE.rst
--rw-r--r--   0        0        0      863 2023-02-03 09:59:16.579787 aleksis_app_order-0.5/README.rst
--rw-r--r--   0        0        0      213 2020-12-13 09:29:37.525364 aleksis_app_order-0.5/aleksis/apps/order/__init__.py
--rw-r--r--   0        0        0      221 2021-01-21 10:54:27.882115 aleksis_app_order-0.5/aleksis/apps/order/address_label.html
--rw-r--r--   0        0        0      286 2023-03-04 17:04:56.553237 aleksis_app_order-0.5/aleksis/apps/order/address_label_style.css
--rw-r--r--   0        0        0     1339 2023-02-03 09:59:16.579787 aleksis_app_order-0.5/aleksis/apps/order/admin.py
--rw-r--r--   0        0        0      438 2021-04-06 15:19:32.769131 aleksis_app_order-0.5/aleksis/apps/order/apps.py
--rw-r--r--   0        0        0     1407 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/filters.py
--rw-r--r--   0        0        0     2114 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/forms.py
--rw-r--r--   0        0        0     1162 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/ControlRow.vue
--rw-r--r--   0        0        0      750 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/CopyToClipboardButton.vue
--rw-r--r--   0        0        0     1277 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/DigitalProducts.vue
--rw-r--r--   0        0        0     3357 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/DigitalProductsByOrder.vue
--rw-r--r--   0        0        0     1089 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/DigitalProductsPerson.vue
--rw-r--r--   0        0        0      300 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/MainContainer.vue
--rw-r--r--   0        0        0     1086 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OptionRadio.vue
--rw-r--r--   0        0        0      731 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OptionRow.vue
--rw-r--r--   0        0        0      564 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OrderForm.graphql
--rw-r--r--   0        0        0    19618 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OrderForm.vue
--rw-r--r--   0        0        0     2634 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OrderItem.vue
--rw-r--r--   0        0        0      937 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/TotalRow.vue
--rw-r--r--   0        0        0      171 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/createShareMutation.graphql
--rw-r--r--   0        0        0      355 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/digitalProducts.graphql
--rw-r--r--   0        0        0      314 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/digitalProductsPerson.graphql
--rw-r--r--   0        0        0      165 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/orderMutation.graphql
--rw-r--r--   0        0        0      183 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/util.js
--rw-r--r--   0        0        0       71 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/whoAmI.graphql
--rw-r--r--   0        0        0     2830 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/index.js
--rw-r--r--   0        0        0     3762 2023-03-04 17:10:48.917237 aleksis_app_order-0.5/aleksis/apps/order/frontend/messages/de.json
--rw-r--r--   0        0        0     3419 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/frontend/messages/en.json
--rw-r--r--   0        0        0        0 2020-12-13 09:29:37.533364 aleksis_app_order-0.5/aleksis/apps/order/locale/.keepdir
--rw-r--r--   0        0        0      463 2023-03-04 17:11:16.429242 aleksis_app_order-0.5/aleksis/apps/order/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20845 2023-03-04 17:05:51.641228 aleksis_app_order-0.5/aleksis/apps/order/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    14252 2023-03-04 17:11:16.429242 aleksis_app_order-0.5/aleksis/apps/order/locale/de_DE/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    28438 2023-03-04 17:05:51.677228 aleksis_app_order-0.5/aleksis/apps/order/locale/de_DE/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      379 2023-03-04 17:11:16.429242 aleksis_app_order-0.5/aleksis/apps/order/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20761 2023-03-04 17:05:51.657228 aleksis_app_order-0.5/aleksis/apps/order/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-04 17:11:16.425242 aleksis_app_order-0.5/aleksis/apps/order/locale/la/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20715 2023-03-04 17:05:51.601228 aleksis_app_order-0.5/aleksis/apps/order/locale/la/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-04 17:11:16.429242 aleksis_app_order-0.5/aleksis/apps/order/locale/nb_NO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20715 2023-03-04 17:05:51.697228 aleksis_app_order-0.5/aleksis/apps/order/locale/nb_NO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      518 2023-03-04 17:11:16.425242 aleksis_app_order-0.5/aleksis/apps/order/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20905 2023-03-04 17:05:51.697228 aleksis_app_order-0.5/aleksis/apps/order/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      337 2023-03-04 17:11:16.425242 aleksis_app_order-0.5/aleksis/apps/order/locale/tr_TR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20715 2023-03-04 17:05:51.621228 aleksis_app_order-0.5/aleksis/apps/order/locale/tr_TR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      602 2023-03-04 17:11:16.425242 aleksis_app_order-0.5/aleksis/apps/order/locale/uk/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    20992 2023-03-04 17:05:51.641228 aleksis_app_order-0.5/aleksis/apps/order/locale/uk/LC_MESSAGES/django.po
--rw-r--r--   0        0        0     9320 2020-12-15 16:13:44.762850 aleksis_app_order-0.5/aleksis/apps/order/migrations/0001_initial.py
--rw-r--r--   0        0        0      605 2020-12-15 20:36:46.652861 aleksis_app_order-0.5/aleksis/apps/order/migrations/0002_auto_20201215_2136.py
--rw-r--r--   0        0        0      520 2020-12-18 10:53:27.488960 aleksis_app_order-0.5/aleksis/apps/order/migrations/0003_auto_20201218_1153.py
--rw-r--r--   0        0        0      401 2020-12-18 11:32:45.150528 aleksis_app_order-0.5/aleksis/apps/order/migrations/0004_order_notes.py
--rw-r--r--   0        0        0      434 2020-12-18 13:49:20.044658 aleksis_app_order-0.5/aleksis/apps/order/migrations/0005_auto_20201218_1449.py
--rw-r--r--   0        0        0      432 2020-12-18 13:52:45.175634 aleksis_app_order-0.5/aleksis/apps/order/migrations/0006_orderform_access_code.py
--rw-r--r--   0        0        0      516 2021-01-11 13:32:47.520703 aleksis_app_order-0.5/aleksis/apps/order/migrations/0007_auto_20210111_1432.py
--rw-r--r--   0        0        0      491 2021-01-21 10:55:10.729917 aleksis_app_order-0.5/aleksis/apps/order/migrations/0008_auto_20210121_1154.py
--rw-r--r--   0        0        0      525 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0009_auto_20220818_2156.py
--rw-r--r--   0        0        0     1908 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0010_auto_20220819_1717.py
--rw-r--r--   0        0        0     1200 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0011_auto_20220819_1742.py
--rw-r--r--   0        0        0     6704 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0012_auto_20221109_2129.py
--rw-r--r--   0        0        0      638 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0013_auto_20221214_2054.py
--rw-r--r--   0        0        0      511 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0014_order_person.py
--rw-r--r--   0        0        0      395 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0015_item_order.py
--rw-r--r--   0        0        0     2808 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0016_auto_20221231_1319.py
--rw-r--r--   0        0        0     1478 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0017_digitalproductshare.py
--rw-r--r--   0        0        0      769 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/migrations/0018_auto_20221231_1841.py
--rw-r--r--   0        0        0        0 2020-12-13 09:29:37.529364 aleksis_app_order-0.5/aleksis/apps/order/migrations/__init__.py
--rw-r--r--   0        0        0    18024 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/models.py
--rw-r--r--   0        0        0      238 2021-01-13 18:41:17.047705 aleksis_app_order-0.5/aleksis/apps/order/order_label.html
--rw-r--r--   0        0        0      483 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/order_label_style.css
--rw-r--r--   0        0        0     1435 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/pdf.py
--rw-r--r--   0        0        0     1414 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/rules.py
--rw-r--r--   0        0        0     8196 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/schema.py
--rw-r--r--   0        0        0       65 2021-01-13 18:47:44.997137 aleksis_app_order-0.5/aleksis/apps/order/settings.py
--rw-r--r--   0        0        0        0 2020-12-13 09:29:37.533364 aleksis_app_order-0.5/aleksis/apps/order/static/.keepdir
--rw-r--r--   0        0        0      963 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/tables.py
--rw-r--r--   0        0        0      392 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/tasks.py
--rw-r--r--   0        0        0      783 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/templates/order/access.html
--rw-r--r--   0        0        0     1555 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/templates/order/actions.html
--rw-r--r--   0        0        0     2624 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/templates/order/breadcrumbs.html
--rw-r--r--   0        0        0      628 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/templates/order/confirmed.html
--rw-r--r--   0        0        0     1483 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/templates/order/detail.html
--rw-r--r--   0        0        0      384 2021-01-09 15:57:05.698844 aleksis_app_order-0.5/aleksis/apps/order/templates/order/edit.html
--rw-r--r--   0        0        0      742 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/templates/order/finished.html
--rw-r--r--   0        0        0     4493 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/templates/order/list.html
--rw-r--r--   0        0        0     2769 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/templates/order/list_print.html
--rw-r--r--   0        0        0     3235 2023-02-03 09:59:16.583788 aleksis_app_order-0.5/aleksis/apps/order/templates/order/order_details.html
--rw-r--r--   0        0        0     1667 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/order/packing_lists.html
--rw-r--r--   0        0        0     3226 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/order/pickup.html
--rw-r--r--   0        0        0     1451 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/confirmation.email
--rw-r--r--   0        0        0     1775 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/confirmation_reminder.email
--rw-r--r--   0        0        0     1235 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/digital_products.email
--rw-r--r--   0        0        0      965 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/order_details.email
--rw-r--r--   0        0        0     1566 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/order_details.html
--rw-r--r--   0        0        0      983 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/order_email.css
--rw-r--r--   0        0        0       62 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/order_number.email
--rw-r--r--   0        0        0       91 2020-12-19 15:38:33.838961 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/order_number.html
--rw-r--r--   0        0        0     1588 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/overview.email
--rw-r--r--   0        0        0     1303 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/pay_confirmation.email
--rw-r--r--   0        0        0     2069 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/pay_reminder.email
--rw-r--r--   0        0        0      198 2020-12-18 10:48:10.656675 aleksis_app_order-0.5/aleksis/apps/order/templatetags/html2text.py
--rw-r--r--   0        0        0     2063 2023-02-03 09:59:16.587789 aleksis_app_order-0.5/aleksis/apps/order/tests/graphql/test_graphl.py
--rw-r--r--   0        0        0      900 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/urls.py
--rw-r--r--   0        0        0      298 2023-02-17 18:54:26.406959 aleksis_app_order-0.5/aleksis/apps/order/util/predicates.py
--rw-r--r--   0        0        0     7948 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/aleksis/apps/order/views.py
--rw-r--r--   0        0        0     1452 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/pyproject.toml
--rw-r--r--   0        0        0     2730 2023-03-04 17:04:56.557237 aleksis_app_order-0.5/tox.ini
--rw-r--r--   0        0        0     2743 1970-01-01 00:00:00.000000 aleksis_app_order-0.5/setup.py
--rw-r--r--   0        0        0     1915 1970-01-01 00:00:00.000000 aleksis_app_order-0.5/PKG-INFO
+-rw-r--r--   0        0        0     3074 2023-05-28 14:55:11.711737 aleksis_app_order-0.6/CHANGELOG.rst
+-rw-r--r--   0        0        0    14361 2020-12-13 09:29:37.493364 aleksis_app_order-0.6/LICENCE.rst
+-rw-r--r--   0        0        0      863 2023-02-03 09:59:16.579787 aleksis_app_order-0.6/README.rst
+-rw-r--r--   0        0        0      213 2020-12-13 09:29:37.525364 aleksis_app_order-0.6/aleksis/apps/order/__init__.py
+-rw-r--r--   0        0        0      221 2021-01-21 10:54:27.882115 aleksis_app_order-0.6/aleksis/apps/order/address_label.html
+-rw-r--r--   0        0        0      286 2023-03-09 21:14:20.892863 aleksis_app_order-0.6/aleksis/apps/order/address_label_style.css
+-rw-r--r--   0        0        0     1339 2023-05-28 14:50:45.725977 aleksis_app_order-0.6/aleksis/apps/order/admin.py
+-rw-r--r--   0        0        0      438 2021-04-06 15:19:32.769131 aleksis_app_order-0.6/aleksis/apps/order/apps.py
+-rw-r--r--   0        0        0     1407 2023-03-09 21:14:20.892863 aleksis_app_order-0.6/aleksis/apps/order/filters.py
+-rw-r--r--   0        0        0     2114 2023-05-28 14:50:45.729977 aleksis_app_order-0.6/aleksis/apps/order/forms.py
+-rw-r--r--   0        0        0     1162 2023-03-09 21:14:20.892863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/ControlRow.vue
+-rw-r--r--   0        0        0      750 2023-03-09 21:14:20.892863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/CopyToClipboardButton.vue
+-rw-r--r--   0        0        0     1277 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/DigitalProducts.vue
+-rw-r--r--   0        0        0     3357 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/DigitalProductsByOrder.vue
+-rw-r--r--   0        0        0     1089 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/DigitalProductsPerson.vue
+-rw-r--r--   0        0        0      300 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/MainContainer.vue
+-rw-r--r--   0        0        0     1086 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OptionRadio.vue
+-rw-r--r--   0        0        0      731 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OptionRow.vue
+-rw-r--r--   0        0        0      564 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OrderForm.graphql
+-rw-r--r--   0        0        0    19618 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OrderForm.vue
+-rw-r--r--   0        0        0     2634 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OrderItem.vue
+-rw-r--r--   0        0        0      937 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/TotalRow.vue
+-rw-r--r--   0        0        0      171 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/createShareMutation.graphql
+-rw-r--r--   0        0        0      355 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/digitalProducts.graphql
+-rw-r--r--   0        0        0      314 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/digitalProductsPerson.graphql
+-rw-r--r--   0        0        0      165 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/orderMutation.graphql
+-rw-r--r--   0        0        0      183 2023-03-09 21:14:20.896863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/util.js
+-rw-r--r--   0        0        0       71 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/whoAmI.graphql
+-rw-r--r--   0        0        0     2830 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/frontend/index.js
+-rw-r--r--   0        0        0     3762 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/frontend/messages/de.json
+-rw-r--r--   0        0        0     3419 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/frontend/messages/en.json
+-rw-r--r--   0        0        0        0 2020-12-13 09:29:37.533364 aleksis_app_order-0.6/aleksis/apps/order/locale/.keepdir
+-rw-r--r--   0        0        0      463 2023-03-12 13:32:25.556782 aleksis_app_order-0.6/aleksis/apps/order/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20845 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    14252 2023-03-12 13:32:25.560782 aleksis_app_order-0.6/aleksis/apps/order/locale/de_DE/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    28438 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/locale/de_DE/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      379 2023-03-12 13:32:25.556782 aleksis_app_order-0.6/aleksis/apps/order/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20761 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-12 13:32:25.560782 aleksis_app_order-0.6/aleksis/apps/order/locale/la/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20715 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/locale/la/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-12 13:32:25.560782 aleksis_app_order-0.6/aleksis/apps/order/locale/nb_NO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20715 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/locale/nb_NO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      518 2023-03-12 13:32:25.560782 aleksis_app_order-0.6/aleksis/apps/order/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20905 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      337 2023-03-12 13:32:25.560782 aleksis_app_order-0.6/aleksis/apps/order/locale/tr_TR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20715 2023-03-09 21:14:20.900863 aleksis_app_order-0.6/aleksis/apps/order/locale/tr_TR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      602 2023-03-12 13:32:25.556782 aleksis_app_order-0.6/aleksis/apps/order/locale/uk/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    20992 2023-03-09 21:14:20.904863 aleksis_app_order-0.6/aleksis/apps/order/locale/uk/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0     9320 2020-12-15 16:13:44.762850 aleksis_app_order-0.6/aleksis/apps/order/migrations/0001_initial.py
+-rw-r--r--   0        0        0      605 2020-12-15 20:36:46.652861 aleksis_app_order-0.6/aleksis/apps/order/migrations/0002_auto_20201215_2136.py
+-rw-r--r--   0        0        0      520 2020-12-18 10:53:27.488960 aleksis_app_order-0.6/aleksis/apps/order/migrations/0003_auto_20201218_1153.py
+-rw-r--r--   0        0        0      401 2020-12-18 11:32:45.150528 aleksis_app_order-0.6/aleksis/apps/order/migrations/0004_order_notes.py
+-rw-r--r--   0        0        0      434 2020-12-18 13:49:20.044658 aleksis_app_order-0.6/aleksis/apps/order/migrations/0005_auto_20201218_1449.py
+-rw-r--r--   0        0        0      432 2020-12-18 13:52:45.175634 aleksis_app_order-0.6/aleksis/apps/order/migrations/0006_orderform_access_code.py
+-rw-r--r--   0        0        0      516 2021-01-11 13:32:47.520703 aleksis_app_order-0.6/aleksis/apps/order/migrations/0007_auto_20210111_1432.py
+-rw-r--r--   0        0        0      491 2021-01-21 10:55:10.729917 aleksis_app_order-0.6/aleksis/apps/order/migrations/0008_auto_20210121_1154.py
+-rw-r--r--   0        0        0      525 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/migrations/0009_auto_20220818_2156.py
+-rw-r--r--   0        0        0     1908 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/migrations/0010_auto_20220819_1717.py
+-rw-r--r--   0        0        0     1200 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/migrations/0011_auto_20220819_1742.py
+-rw-r--r--   0        0        0     6704 2023-03-09 20:42:01.156249 aleksis_app_order-0.6/aleksis/apps/order/migrations/0012_auto_20221109_2129.py
+-rw-r--r--   0        0        0      638 2023-03-09 20:42:01.156249 aleksis_app_order-0.6/aleksis/apps/order/migrations/0013_auto_20221214_2054.py
+-rw-r--r--   0        0        0      511 2023-03-09 20:42:01.156249 aleksis_app_order-0.6/aleksis/apps/order/migrations/0014_order_person.py
+-rw-r--r--   0        0        0      395 2023-03-09 20:42:01.156249 aleksis_app_order-0.6/aleksis/apps/order/migrations/0015_item_order.py
+-rw-r--r--   0        0        0     2808 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/migrations/0016_auto_20221231_1319.py
+-rw-r--r--   0        0        0     1478 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/migrations/0017_digitalproductshare.py
+-rw-r--r--   0        0        0      769 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/migrations/0018_auto_20221231_1841.py
+-rw-r--r--   0        0        0      630 2023-03-10 15:53:09.031843 aleksis_app_order-0.6/aleksis/apps/order/migrations/0019_auto_20230309_2157.py
+-rw-r--r--   0        0        0        0 2020-12-13 09:29:37.529364 aleksis_app_order-0.6/aleksis/apps/order/migrations/__init__.py
+-rw-r--r--   0        0        0    18014 2023-05-28 14:50:45.729977 aleksis_app_order-0.6/aleksis/apps/order/models.py
+-rw-r--r--   0        0        0      238 2021-01-13 18:41:17.047705 aleksis_app_order-0.6/aleksis/apps/order/order_label.html
+-rw-r--r--   0        0        0      483 2023-03-09 21:14:20.904863 aleksis_app_order-0.6/aleksis/apps/order/order_label_style.css
+-rw-r--r--   0        0        0     1435 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/pdf.py
+-rw-r--r--   0        0        0     1414 2023-03-09 21:14:20.904863 aleksis_app_order-0.6/aleksis/apps/order/rules.py
+-rw-r--r--   0        0        0     8196 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/schema.py
+-rw-r--r--   0        0        0       65 2021-01-13 18:47:44.997137 aleksis_app_order-0.6/aleksis/apps/order/settings.py
+-rw-r--r--   0        0        0        0 2020-12-13 09:29:37.533364 aleksis_app_order-0.6/aleksis/apps/order/static/.keepdir
+-rw-r--r--   0        0        0      963 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/tables.py
+-rw-r--r--   0        0        0      386 2023-03-10 15:53:09.031843 aleksis_app_order-0.6/aleksis/apps/order/tasks.py
+-rw-r--r--   0        0        0      783 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/templates/order/access.html
+-rw-r--r--   0        0        0     1555 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/templates/order/actions.html
+-rw-r--r--   0        0        0     2624 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/templates/order/breadcrumbs.html
+-rw-r--r--   0        0        0      628 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/templates/order/confirmed.html
+-rw-r--r--   0        0        0     1483 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/templates/order/detail.html
+-rw-r--r--   0        0        0      384 2021-01-09 15:57:05.698844 aleksis_app_order-0.6/aleksis/apps/order/templates/order/edit.html
+-rw-r--r--   0        0        0      742 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/templates/order/finished.html
+-rw-r--r--   0        0        0     4493 2023-03-09 21:14:20.904863 aleksis_app_order-0.6/aleksis/apps/order/templates/order/list.html
+-rw-r--r--   0        0        0     2769 2023-02-03 09:59:16.583788 aleksis_app_order-0.6/aleksis/apps/order/templates/order/list_print.html
+-rw-r--r--   0        0        0     3235 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/templates/order/order_details.html
+-rw-r--r--   0        0        0     1667 2023-02-03 09:59:16.587789 aleksis_app_order-0.6/aleksis/apps/order/templates/order/packing_lists.html
+-rw-r--r--   0        0        0     3226 2023-02-03 09:59:16.587789 aleksis_app_order-0.6/aleksis/apps/order/templates/order/pickup.html
+-rw-r--r--   0        0        0     1451 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/confirmation.email
+-rw-r--r--   0        0        0     1775 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/confirmation_reminder.email
+-rw-r--r--   0        0        0     1235 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/digital_products.email
+-rw-r--r--   0        0        0      965 2023-02-03 09:59:16.587789 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/order_details.email
+-rw-r--r--   0        0        0     1566 2023-02-03 09:59:16.587789 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/order_details.html
+-rw-r--r--   0        0        0      983 2023-03-09 21:14:20.904863 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/order_email.css
+-rw-r--r--   0        0        0       62 2023-02-03 09:59:16.587789 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/order_number.email
+-rw-r--r--   0        0        0       91 2020-12-19 15:38:33.838961 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/order_number.html
+-rw-r--r--   0        0        0     1588 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/overview.email
+-rw-r--r--   0        0        0     1303 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/pay_confirmation.email
+-rw-r--r--   0        0        0     2069 2023-03-09 20:42:01.160249 aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/pay_reminder.email
+-rw-r--r--   0        0        0      198 2020-12-18 10:48:10.656675 aleksis_app_order-0.6/aleksis/apps/order/templatetags/html2text.py
+-rw-r--r--   0        0        0     2063 2023-03-09 20:42:01.164249 aleksis_app_order-0.6/aleksis/apps/order/tests/graphql/test_graphl.py
+-rw-r--r--   0        0        0      900 2023-03-09 21:14:20.904863 aleksis_app_order-0.6/aleksis/apps/order/urls.py
+-rw-r--r--   0        0        0      298 2023-02-17 18:54:26.406959 aleksis_app_order-0.6/aleksis/apps/order/util/predicates.py
+-rw-r--r--   0        0        0     7948 2023-03-09 21:14:20.904863 aleksis_app_order-0.6/aleksis/apps/order/views.py
+-rw-r--r--   0        0        0     1450 2023-05-28 16:05:47.255758 aleksis_app_order-0.6/pyproject.toml
+-rw-r--r--   0        0        0     2730 2023-03-09 21:14:20.908863 aleksis_app_order-0.6/tox.ini
+-rw-r--r--   0        0        0     1913 1970-01-01 00:00:00.000000 aleksis_app_order-0.6/PKG-INFO
```

### Comparing `aleksis_app_order-0.5/CHANGELOG.rst` & `aleksis_app_order-0.6/CHANGELOG.rst`

 * *Files 10% similar despite different names*

```diff
@@ -2,29 +2,49 @@
 =========
 
 All notable changes to this project will be documented in this file.
 
 The format is based on `Keep a Changelog`_,
 and this project adheres to `Semantic Versioning`_.
 
-`0.5` - ?
+`0.6`_ - 2023-05-28
+-------------------
+
+Nothing changed.
+
+`0.5.1`_ - 2023-03-09
+---------------------
+
+Fixed
+~~~~~
+
+* Fix tracking of share expirations for digital products.
+
+`0.5`_ - 2023-03-04
 ------------------
 
 This version requires AlekSIS-Core 3.0. It is incompatible with any previous
 version.
 
 Removed
 ~~~~~~~
 
 * Legacy menu integration for AlekSIS-Core pre-3.0
 
 Added
 ~~~~~
 
 * Add SPA support for AlekSIS-Core 3.0
+
+`0.4.1`_ - 2023-03-09
+---------------------
+
+Added
+~~~~~
+
 * Special items (e. g. digital products) can now be excluded 
   from shipping cost calculation.
 * Support digital products via Nextcloud.
 * Items can be excluded from shipping cost calculation (e. g. digital products).
 
 Changed
 ~~~~~~~
@@ -37,19 +57,14 @@
 ~~~~~
 
 * Label buttons in list view didn't work.
 * Text-only emails contained too much whitespace.
 * Make HTML mails compatible with more clients.
 * Layout in order statistics table was broken.
 
-Removed
-~~~~~~~
-
-* Drop compatibility with AlekSIS-Core series 2.x
-
 `0.4`_ - 2022-06-09
 -------------------
 
 Added
 ~~~~~
 
 * Implement special form as an easy way to manage pick up.
@@ -108,8 +123,11 @@
 .. _Semantic Versioning: https://semver.org/spec/v2.0.0.html
 
 .. _0.1b0: https://edugit.org/hansegucker/AlekSIS-App-Order/-/tags/0.1b0
 .. _0.1.1: https://edugit.org/hansegucker/AlekSIS-App-Order/-/tags/0.1.1
 .. _0.2: https://edugit.org/hansegucker/AlekSIS-App-Order/-/tags/0.2
 .. _0.3: https://edugit.org/hansegucker/AlekSIS-App-Order/-/tags/0.3
 .. _0.4: https://edugit.org/hansegucker/AlekSIS-App-Order/-/tags/0.4
+.. _0.4.1: https://edugit.org/hansegucker/AlekSIS-App-Order/-/tags/0.4.1
 .. _0.5: https://edugit.org/hansegucker/AlekSIS-App-Order/-/tags/0.5
+.. _0.5.1: https://edugit.org/hansegucker/AlekSIS-App-Order/-/tags/0.5.1
+.. _0.6: https://edugit.org/hansegucker/AlekSIS-App-Order/-/tags/0.6
```

### Comparing `aleksis_app_order-0.5/LICENCE.rst` & `aleksis_app_order-0.6/LICENCE.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/README.rst` & `aleksis_app_order-0.6/README.rst`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/admin.py` & `aleksis_app_order-0.6/aleksis/apps/order/admin.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/filters.py` & `aleksis_app_order-0.6/aleksis/apps/order/filters.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/forms.py` & `aleksis_app_order-0.6/aleksis/apps/order/forms.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/ControlRow.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/ControlRow.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/CopyToClipboardButton.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/CopyToClipboardButton.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/DigitalProducts.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/DigitalProducts.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/DigitalProductsByOrder.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/DigitalProductsByOrder.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/DigitalProductsPerson.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/DigitalProductsPerson.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OptionRadio.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OptionRadio.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OptionRow.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OptionRow.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OrderForm.graphql` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OrderForm.graphql`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OrderForm.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OrderForm.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/OrderItem.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/OrderItem.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/components/order_form/TotalRow.vue` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/components/order_form/TotalRow.vue`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/index.js` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/index.js`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/messages/de.json` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/messages/de.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/frontend/messages/en.json` & `aleksis_app_order-0.6/aleksis/apps/order/frontend/messages/en.json`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/ar/LC_MESSAGES/django.po` & `aleksis_app_order-0.6/aleksis/apps/order/locale/ar/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/de_DE/LC_MESSAGES/django.mo` & `aleksis_app_order-0.6/aleksis/apps/order/locale/de_DE/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/de_DE/LC_MESSAGES/django.po` & `aleksis_app_order-0.6/aleksis/apps/order/locale/de_DE/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/fr/LC_MESSAGES/django.po` & `aleksis_app_order-0.6/aleksis/apps/order/locale/fr/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/la/LC_MESSAGES/django.po` & `aleksis_app_order-0.6/aleksis/apps/order/locale/la/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/nb_NO/LC_MESSAGES/django.po` & `aleksis_app_order-0.6/aleksis/apps/order/locale/nb_NO/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/ru/LC_MESSAGES/django.mo` & `aleksis_app_order-0.6/aleksis/apps/order/locale/ru/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/ru/LC_MESSAGES/django.po` & `aleksis_app_order-0.6/aleksis/apps/order/locale/ru/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/tr_TR/LC_MESSAGES/django.po` & `aleksis_app_order-0.6/aleksis/apps/order/locale/tr_TR/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/uk/LC_MESSAGES/django.mo` & `aleksis_app_order-0.6/aleksis/apps/order/locale/uk/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/locale/uk/LC_MESSAGES/django.po` & `aleksis_app_order-0.6/aleksis/apps/order/locale/uk/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0001_initial.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0002_auto_20201215_2136.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0002_auto_20201215_2136.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0003_auto_20201218_1153.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0003_auto_20201218_1153.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0007_auto_20210111_1432.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0007_auto_20210111_1432.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0009_auto_20220818_2156.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0009_auto_20220818_2156.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0010_auto_20220819_1717.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0010_auto_20220819_1717.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0011_auto_20220819_1742.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0011_auto_20220819_1742.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0012_auto_20221109_2129.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0012_auto_20221109_2129.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0013_auto_20221214_2054.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0013_auto_20221214_2054.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0016_auto_20221231_1319.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0016_auto_20221231_1319.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0017_digitalproductshare.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0017_digitalproductshare.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/migrations/0018_auto_20221231_1841.py` & `aleksis_app_order-0.6/aleksis/apps/order/migrations/0018_auto_20221231_1841.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/models.py` & `aleksis_app_order-0.6/aleksis/apps/order/models.py`

 * *Files 1% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     """Digital product share."""
 
     order_item = models.ForeignKey(
         "OrderItem", on_delete=models.CASCADE, verbose_name=_("Order item"), related_name="shares"
     )
     share_id = models.CharField(max_length=255, verbose_name=_("Share ID"))
     share_url = models.URLField(verbose_name=_("Share URL"))
-    share_expiration = models.DateField(verbose_name=_("Share expiration"))
+    share_expiration = models.DateTimeField(verbose_name=_("Share expiration"))
 
     def __str__(self):
         return self.share_id
 
     class Meta:
         verbose_name = _("Digital product share")
         verbose_name_plural = _("Digital product shares")
@@ -98,15 +98,15 @@
         xml = self.nextcloud_provider.do_request(
             "/ocs/v1.php/apps/files_sharing/api/v1/shares", method="POST", data=args
         )
         share_id = xml.find("data").find("id").text
         share_url = xml.find("data").find("url").text
         share_expiration = datetime.strptime(
             xml.find("data").find("expiration").text, "%Y-%m-%d %H:%M:%S"
-        ).date()
+        )
 
         return DigitalProductShare.objects.create(
             order_item=order_item,
             share_id=share_id,
             share_url=share_url,
             share_expiration=share_expiration,
         )
@@ -486,15 +486,15 @@
     def create_share(self):
         if self.item.digital_product_object:
             return self.item.digital_product_object.create_share(self)
 
     @property
     def current_shares(self):
         if self.item.digital_product_object:
-            return self.shares.filter(share_expiration__gte=timezone.now().date())
+            return self.shares.filter(share_expiration__gte=timezone.now())
         return self.shares.none()
 
     @property
     def shares_left(self) -> int:
         shares_left = self.count - self.current_shares.count()
         return shares_left if shares_left > 0 else 0
```

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/pdf.py` & `aleksis_app_order-0.6/aleksis/apps/order/pdf.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/rules.py` & `aleksis_app_order-0.6/aleksis/apps/order/rules.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/schema.py` & `aleksis_app_order-0.6/aleksis/apps/order/schema.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/tables.py` & `aleksis_app_order-0.6/aleksis/apps/order/tables.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/access.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/access.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/actions.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/actions.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/breadcrumbs.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/breadcrumbs.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/confirmed.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/confirmed.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/detail.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/detail.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/finished.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/finished.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/list.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/list.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/list_print.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/list_print.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/order_details.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/order_details.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/packing_lists.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/packing_lists.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/order/pickup.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/order/pickup.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/confirmation.email` & `aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/confirmation.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/confirmation_reminder.email` & `aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/confirmation_reminder.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/digital_products.email` & `aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/digital_products.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/order_details.email` & `aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/order_details.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/order_details.html` & `aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/order_details.html`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/order_email.css` & `aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/order_email.css`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/overview.email` & `aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/overview.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/pay_confirmation.email` & `aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/pay_confirmation.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/templates/templated_email/pay_reminder.email` & `aleksis_app_order-0.6/aleksis/apps/order/templates/templated_email/pay_reminder.email`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/tests/graphql/test_graphl.py` & `aleksis_app_order-0.6/aleksis/apps/order/tests/graphql/test_graphl.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/urls.py` & `aleksis_app_order-0.6/aleksis/apps/order/urls.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/aleksis/apps/order/views.py` & `aleksis_app_order-0.6/aleksis/apps/order/views.py`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/pyproject.toml` & `aleksis_app_order-0.6/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "AlekSIS-App-Order"
-version = "0.5"
+version = "0.6"
 packages = [
     { include = "aleksis" }
 ]
 readme = "README.rst"
 include = [
     { path = "aleksis/**/*.mo", format = ["sdist", "wheel"] },
     { path = "*.rst", format = "sdist" },
@@ -31,15 +31,15 @@
 [[tool.poetry.source]]
 name = "gitlab"
 url = "https://edugit.org/api/v4/projects/461/packages/pypi/simple"
 secondary = true
 
 [tool.poetry.dependencies]
 python = "^3.9"
-aleksis-core = "^3.0b0"
+aleksis-core = "^3.0"
 html2text = "^2020.1.16"
 blabel = "^0.1.4"
 defusedxml = "^0.7.1"
 
 [tool.poetry.dev-dependencies]
 aleksis-builddeps = "*"
```

### Comparing `aleksis_app_order-0.5/tox.ini` & `aleksis_app_order-0.6/tox.ini`

 * *Files identical despite different names*

### Comparing `aleksis_app_order-0.5/PKG-INFO` & `aleksis_app_order-0.6/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aleksis-app-order
-Version: 0.5
+Version: 0.6
 Summary: AlekSIS (School Information System) — App Order (Manage orders)
 Home-page: https://edugit.org/hansegucker/AlekSIS-App-Order
 License: EUPL-1.2
 Author: Jonathan Weth
 Author-email: dev@jonathanweth.de
 Maintainer: Jonathan Weth
 Maintainer-email: dev@jonathanweth.de
@@ -13,15 +13,15 @@
 Classifier: Intended Audience :: Education
 Classifier: License :: OSI Approved :: European Union Public Licence 1.2 (EUPL 1.2)
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Education
-Requires-Dist: aleksis-core (>=3.0b0,<4.0)
+Requires-Dist: aleksis-core (>=3.0,<4.0)
 Requires-Dist: blabel (>=0.1.4,<0.2.0)
 Requires-Dist: defusedxml (>=0.7.1,<0.8.0)
 Requires-Dist: html2text (>=2020.1.16,<2021.0.0)
 Project-URL: Repository, https://edugit.org/hansegucker/AlekSIS-App-Order
 Description-Content-Type: text/x-rst
 
 AlekSIS — Unofficial App Order (Manage orders)
```

