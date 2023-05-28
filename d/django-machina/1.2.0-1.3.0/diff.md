# Comparing `tmp/django-machina-1.2.0.tar.gz` & `tmp/django_machina-1.3.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-machina-1.2.0.tar", max compression
+gzip compressed data, was "django_machina-1.3.0.tar", max compression
```

## Comparing `django-machina-1.2.0.tar` & `django_machina-1.3.0.tar`

### file list

```diff
@@ -1,325 +1,331 @@
--rw-r--r--   0        0        0      483 2021-12-11 21:41:38.728460 django-machina-1.2.0/AUTHORS
--rw-r--r--   0        0        0      209 2021-12-11 21:41:38.728521 django-machina-1.2.0/CHANGELOG.rst
--rw-r--r--   0        0        0      280 2021-12-11 21:41:38.728580 django-machina-1.2.0/CONTRIBUTING.rst
--rw-r--r--   0        0        0     1515 2022-01-01 14:09:44.179684 django-machina-1.2.0/LICENSE
--rw-r--r--   0        0        0     1525 2022-05-16 22:53:00.256133 django-machina-1.2.0/README.rst
--rw-r--r--   0        0        0      516 2021-12-11 21:41:38.736589 django-machina-1.2.0/machina/__init__.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.736652 django-machina-1.2.0/machina/apps/__init__.py
--rw-r--r--   0        0        0        0 2022-04-24 02:23:54.035719 django-machina-1.2.0/machina/apps/forum/__init__.py
--rw-r--r--   0        0        0     8200 2021-12-11 21:41:38.736832 django-machina-1.2.0/machina/apps/forum/abstract_models.py
--rw-r--r--   0        0        0    20089 2022-04-24 02:08:48.835350 django-machina-1.2.0/machina/apps/forum/admin.py
--rw-r--r--   0        0        0      614 2021-12-11 21:41:38.736999 django-machina-1.2.0/machina/apps/forum/apps.py
--rw-r--r--   0        0        0     4255 2021-12-11 21:41:38.737073 django-machina-1.2.0/machina/apps/forum/forms.py
--rw-r--r--   0        0        0     3267 2021-12-11 21:41:38.737188 django-machina-1.2.0/machina/apps/forum/migrations/0001_initial.py
--rw-r--r--   0        0        0      423 2021-12-11 21:41:38.737250 django-machina-1.2.0/machina/apps/forum/migrations/0002_auto_20150725_0512.py
--rw-r--r--   0        0        0      392 2021-12-11 21:41:38.737307 django-machina-1.2.0/machina/apps/forum/migrations/0003_remove_forum_is_active.py
--rw-r--r--   0        0        0      772 2021-12-11 21:41:38.737364 django-machina-1.2.0/machina/apps/forum/migrations/0004_auto_20170504_2108.py
--rw-r--r--   0        0        0      847 2021-12-11 21:41:38.737422 django-machina-1.2.0/machina/apps/forum/migrations/0005_auto_20170504_2113.py
--rw-r--r--   0        0        0      503 2021-12-11 21:41:38.737474 django-machina-1.2.0/machina/apps/forum/migrations/0006_auto_20170523_2036.py
--rw-r--r--   0        0        0      748 2021-12-11 21:41:38.737528 django-machina-1.2.0/machina/apps/forum/migrations/0007_auto_20170523_2140.py
--rw-r--r--   0        0        0      686 2021-12-11 21:41:38.737579 django-machina-1.2.0/machina/apps/forum/migrations/0008_forum_last_post.py
--rw-r--r--   0        0        0      789 2021-12-11 21:41:38.737635 django-machina-1.2.0/machina/apps/forum/migrations/0009_auto_20170928_2327.py
--rw-r--r--   0        0        0      577 2021-12-11 21:41:38.737695 django-machina-1.2.0/machina/apps/forum/migrations/0010_auto_20181103_1401.py
--rw-r--r--   0        0        0      717 2021-12-11 21:41:38.737747 django-machina-1.2.0/machina/apps/forum/migrations/0011_auto_20190627_2132.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.737771 django-machina-1.2.0/machina/apps/forum/migrations/__init__.py
--rw-r--r--   0        0        0      264 2021-12-11 21:41:38.737836 django-machina-1.2.0/machina/apps/forum/models.py
--rw-r--r--   0        0        0      565 2021-12-11 21:41:38.737893 django-machina-1.2.0/machina/apps/forum/receivers.py
--rw-r--r--   0        0        0      324 2022-04-24 02:08:01.104191 django-machina-1.2.0/machina/apps/forum/signals.py
--rw-r--r--   0        0        0      945 2021-12-11 21:41:38.738007 django-machina-1.2.0/machina/apps/forum/urls.py
--rw-r--r--   0        0        0     4546 2021-12-11 21:41:38.738103 django-machina-1.2.0/machina/apps/forum/views.py
--rw-r--r--   0        0        0     9198 2021-12-11 21:41:38.738195 django-machina-1.2.0/machina/apps/forum/visibility.py
--rw-r--r--   0        0        0        0 2022-04-24 02:23:56.281039 django-machina-1.2.0/machina/apps/forum_conversation/__init__.py
--rw-r--r--   0        0        0    13112 2021-12-11 21:41:38.738395 django-machina-1.2.0/machina/apps/forum_conversation/abstract_models.py
--rw-r--r--   0        0        0     1443 2021-12-11 21:41:38.738458 django-machina-1.2.0/machina/apps/forum_conversation/admin.py
--rw-r--r--   0        0        0      692 2021-12-11 21:41:38.738508 django-machina-1.2.0/machina/apps/forum_conversation/apps.py
--rw-r--r--   0        0        0     9260 2022-05-14 00:32:35.714100 django-machina-1.2.0/machina/apps/forum_conversation/forms.py
--rw-r--r--   0        0        0        0 2022-04-24 02:23:58.539579 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/__init__.py
--rw-r--r--   0        0        0     1564 2021-12-11 21:41:38.738709 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/abstract_models.py
--rw-r--r--   0        0        0      608 2021-12-11 21:41:38.738769 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/admin.py
--rw-r--r--   0        0        0      558 2021-12-11 21:41:38.738821 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/apps.py
--rw-r--r--   0        0        0     4544 2021-12-11 21:41:38.738896 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/cache.py
--rw-r--r--   0        0        0     1275 2021-12-11 21:41:38.738963 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/forms.py
--rw-r--r--   0        0        0     1004 2021-12-11 21:41:38.739061 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/migrations/0001_initial.py
--rw-r--r--   0        0        0      573 2021-12-11 21:41:38.739119 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/migrations/0002_auto_20181103_1404.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.739141 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/migrations/__init__.py
--rw-r--r--   0        0        0      346 2021-12-11 21:41:38.739195 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/models.py
--rw-r--r--   0        0        0      854 2021-12-11 21:41:38.739249 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/urls.py
--rw-r--r--   0        0        0     1522 2021-12-11 21:41:38.739315 django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/views.py
--rw-r--r--   0        0        0        0 2022-04-24 02:24:00.838464 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/__init__.py
--rw-r--r--   0        0        0     4155 2021-12-11 21:41:38.739492 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/abstract_models.py
--rw-r--r--   0        0        0     1275 2021-12-11 21:41:38.739557 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/admin.py
--rw-r--r--   0        0        0      522 2021-12-11 21:41:38.739609 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/apps.py
--rw-r--r--   0        0        0     4507 2021-12-11 21:41:38.739686 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/forms.py
--rw-r--r--   0        0        0     3237 2021-12-11 21:41:38.739780 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/migrations/0001_initial.py
--rw-r--r--   0        0        0      777 2021-12-11 21:41:38.739834 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/migrations/0002_auto_20151105_0029.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.739857 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/migrations/__init__.py
--rw-r--r--   0        0        0      485 2021-12-11 21:41:38.739908 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/models.py
--rw-r--r--   0        0        0      817 2021-12-11 21:41:38.739965 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/urls.py
--rw-r--r--   0        0        0      375 2021-12-11 21:41:38.740025 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/validators.py
--rw-r--r--   0        0        0     3338 2021-12-11 21:41:38.740103 django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/views.py
--rw-r--r--   0        0        0      400 2021-12-11 21:41:38.740160 django-machina-1.2.0/machina/apps/forum_conversation/managers.py
--rw-r--r--   0        0        0     4686 2021-12-11 21:41:38.740239 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0001_initial.py
--rw-r--r--   0        0        0      470 2021-12-11 21:41:38.740293 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0002_post_anonymous_key.py
--rw-r--r--   0        0        0      637 2021-12-11 21:41:38.740349 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0003_auto_20160228_2051.py
--rw-r--r--   0        0        0      594 2021-12-11 21:41:38.740398 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0004_auto_20160427_0502.py
--rw-r--r--   0        0        0      699 2021-12-11 21:41:38.740460 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0005_auto_20160607_0455.py
--rw-r--r--   0        0        0      519 2021-12-11 21:41:38.740529 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0006_post_enable_signature.py
--rw-r--r--   0        0        0      942 2021-12-11 21:41:38.740588 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0007_auto_20160903_0450.py
--rw-r--r--   0        0        0      902 2021-12-11 21:41:38.740646 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0008_auto_20160903_0512.py
--rw-r--r--   0        0        0      481 2021-12-11 21:41:38.740698 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0009_auto_20160925_2126.py
--rw-r--r--   0        0        0      644 2021-12-11 21:41:38.740748 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0010_auto_20170120_0224.py
--rw-r--r--   0        0        0      340 2021-12-11 21:41:38.740806 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0011_remove_post_poster_ip.py
--rw-r--r--   0        0        0      575 2021-12-11 21:41:38.740864 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0012_auto_20200423_1049.py
--rw-r--r--   0        0        0     1043 2021-12-11 21:41:38.740936 django-machina-1.2.0/machina/apps/forum_conversation/migrations/0013_auto_20201220_1745.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.740966 django-machina-1.2.0/machina/apps/forum_conversation/migrations/__init__.py
--rw-r--r--   0        0        0      365 2021-12-11 21:41:38.741038 django-machina-1.2.0/machina/apps/forum_conversation/models.py
--rw-r--r--   0        0        0      543 2021-12-11 21:41:38.741106 django-machina-1.2.0/machina/apps/forum_conversation/receivers.py
--rw-r--r--   0        0        0      271 2021-12-11 21:41:38.741166 django-machina-1.2.0/machina/apps/forum_conversation/signals.py
--rw-r--r--   0        0        0     3903 2021-12-11 21:41:38.741240 django-machina-1.2.0/machina/apps/forum_conversation/urls.py
--rw-r--r--   0        0        0    29544 2021-12-11 21:41:38.741360 django-machina-1.2.0/machina/apps/forum_conversation/views.py
--rw-r--r--   0        0        0        0 2022-04-24 02:24:05.990706 django-machina-1.2.0/machina/apps/forum_feeds/__init__.py
--rw-r--r--   0        0        0      503 2021-12-11 21:41:38.741533 django-machina-1.2.0/machina/apps/forum_feeds/apps.py
--rw-r--r--   0        0        0     2326 2021-12-11 21:41:38.741613 django-machina-1.2.0/machina/apps/forum_feeds/feeds.py
--rw-r--r--   0        0        0     1246 2021-12-11 21:41:38.741680 django-machina-1.2.0/machina/apps/forum_feeds/urls.py
--rw-r--r--   0        0        0        0 2022-04-24 02:24:08.124945 django-machina-1.2.0/machina/apps/forum_member/__init__.py
--rw-r--r--   0        0        0     2192 2021-12-11 21:41:38.741879 django-machina-1.2.0/machina/apps/forum_member/abstract_models.py
--rw-r--r--   0        0        0      835 2021-12-11 21:41:38.741994 django-machina-1.2.0/machina/apps/forum_member/admin.py
--rw-r--r--   0        0        0      656 2021-12-11 21:41:38.742066 django-machina-1.2.0/machina/apps/forum_member/apps.py
--rw-r--r--   0        0        0      628 2021-12-11 21:41:38.742129 django-machina-1.2.0/machina/apps/forum_member/forms.py
--rw-r--r--   0        0        0     1410 2021-12-11 21:41:38.742235 django-machina-1.2.0/machina/apps/forum_member/migrations/0001_initial.py
--rw-r--r--   0        0        0      644 2021-12-11 21:41:38.742310 django-machina-1.2.0/machina/apps/forum_member/migrations/0002_auto_20160225_0515.py
--rw-r--r--   0        0        0      665 2021-12-11 21:41:38.742368 django-machina-1.2.0/machina/apps/forum_member/migrations/0003_auto_20160227_2122.py
--rw-r--r--   0        0        0      604 2021-12-11 21:41:38.742425 django-machina-1.2.0/machina/apps/forum_member/migrations/0004_auto_20181103_1406.py
--rw-r--r--   0        0        0      600 2021-12-11 21:41:38.742485 django-machina-1.2.0/machina/apps/forum_member/migrations/0005_auto_20200423_1049.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.742512 django-machina-1.2.0/machina/apps/forum_member/migrations/__init__.py
--rw-r--r--   0        0        0      313 2021-12-11 21:41:38.742570 django-machina-1.2.0/machina/apps/forum_member/models.py
--rw-r--r--   0        0        0     3883 2022-01-30 20:21:22.499709 django-machina-1.2.0/machina/apps/forum_member/receivers.py
--rw-r--r--   0        0        0      395 2021-12-11 21:41:38.742715 django-machina-1.2.0/machina/apps/forum_member/shortcuts.py
--rw-r--r--   0        0        0     2185 2021-12-11 21:41:38.742780 django-machina-1.2.0/machina/apps/forum_member/urls.py
--rw-r--r--   0        0        0     8767 2021-12-11 21:41:38.742880 django-machina-1.2.0/machina/apps/forum_member/views.py
--rw-r--r--   0        0        0        0 2022-04-24 02:24:10.082345 django-machina-1.2.0/machina/apps/forum_moderation/__init__.py
--rw-r--r--   0        0        0      533 2021-12-11 21:41:38.743067 django-machina-1.2.0/machina/apps/forum_moderation/apps.py
--rw-r--r--   0        0        0     2022 2021-12-11 21:41:38.743148 django-machina-1.2.0/machina/apps/forum_moderation/forms.py
--rw-r--r--   0        0        0     3608 2021-12-11 21:41:38.743215 django-machina-1.2.0/machina/apps/forum_moderation/urls.py
--rw-r--r--   0        0        0    17440 2021-12-11 21:41:38.743372 django-machina-1.2.0/machina/apps/forum_moderation/views.py
--rw-r--r--   0        0        0        0 2022-04-24 02:24:12.220784 django-machina-1.2.0/machina/apps/forum_permission/__init__.py
--rw-r--r--   0        0        0     4489 2021-12-11 21:41:38.743570 django-machina-1.2.0/machina/apps/forum_permission/abstract_models.py
--rw-r--r--   0        0        0     1623 2021-12-11 21:41:38.743647 django-machina-1.2.0/machina/apps/forum_permission/admin.py
--rw-r--r--   0        0        0      680 2021-12-11 21:41:38.743704 django-machina-1.2.0/machina/apps/forum_permission/apps.py
--rw-r--r--   0        0        0    15495 2021-12-11 21:41:38.743850 django-machina-1.2.0/machina/apps/forum_permission/checker.py
--rw-r--r--   0        0        0     4045 2021-12-11 21:41:38.743918 django-machina-1.2.0/machina/apps/forum_permission/defaults.py
--rw-r--r--   0        0        0    16447 2021-12-11 21:41:38.744082 django-machina-1.2.0/machina/apps/forum_permission/handler.py
--rw-r--r--   0        0        0     1631 2021-12-11 21:41:38.744169 django-machina-1.2.0/machina/apps/forum_permission/middleware.py
--rw-r--r--   0        0        0     3646 2021-12-11 21:41:38.744277 django-machina-1.2.0/machina/apps/forum_permission/migrations/0001_initial.py
--rw-r--r--   0        0        0     1749 2021-12-11 21:41:38.744344 django-machina-1.2.0/machina/apps/forum_permission/migrations/0002_auto_20160607_0500.py
--rw-r--r--   0        0        0      407 2021-12-11 21:41:38.744407 django-machina-1.2.0/machina/apps/forum_permission/migrations/0003_remove_forumpermission_name.py
--rw-r--r--   0        0        0      472 2021-12-11 21:41:38.744475 django-machina-1.2.0/machina/apps/forum_permission/migrations/0004_auto_20190319_2240.py
--rw-r--r--   0        0        0      478 2021-12-11 21:41:38.744539 django-machina-1.2.0/machina/apps/forum_permission/migrations/0005_userforumpermission_authenticated_user.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.744562 django-machina-1.2.0/machina/apps/forum_permission/migrations/__init__.py
--rw-r--r--   0        0        0      537 2021-12-11 21:41:38.744621 django-machina-1.2.0/machina/apps/forum_permission/models.py
--rw-r--r--   0        0        0      924 2021-12-11 21:41:38.744675 django-machina-1.2.0/machina/apps/forum_permission/receivers.py
--rw-r--r--   0        0        0     3919 2021-12-11 21:41:38.744752 django-machina-1.2.0/machina/apps/forum_permission/shortcuts.py
--rw-r--r--   0        0        0     4529 2021-12-11 21:41:38.744829 django-machina-1.2.0/machina/apps/forum_permission/viewmixins.py
--rw-r--r--   0        0        0        0 2022-04-24 02:24:17.017613 django-machina-1.2.0/machina/apps/forum_search/__init__.py
--rw-r--r--   0        0        0      511 2021-12-11 21:41:38.744973 django-machina-1.2.0/machina/apps/forum_search/apps.py
--rw-r--r--   0        0        0     2810 2021-12-11 21:41:38.745046 django-machina-1.2.0/machina/apps/forum_search/forms.py
--rw-r--r--   0        0        0     1873 2021-12-11 21:41:38.745121 django-machina-1.2.0/machina/apps/forum_search/search_indexes.py
--rw-r--r--   0        0        0     1032 2021-12-11 21:41:38.745185 django-machina-1.2.0/machina/apps/forum_search/urls.py
--rw-r--r--   0        0        0      421 2021-12-11 21:41:38.745243 django-machina-1.2.0/machina/apps/forum_search/views.py
--rw-r--r--   0        0        0        0 2022-04-24 02:24:20.827183 django-machina-1.2.0/machina/apps/forum_tracking/__init__.py
--rw-r--r--   0        0        0     2050 2021-12-11 21:41:38.745412 django-machina-1.2.0/machina/apps/forum_tracking/abstract_models.py
--rw-r--r--   0        0        0      890 2021-12-11 21:41:38.745478 django-machina-1.2.0/machina/apps/forum_tracking/admin.py
--rw-r--r--   0        0        0      667 2021-12-11 21:41:38.745532 django-machina-1.2.0/machina/apps/forum_tracking/apps.py
--rw-r--r--   0        0        0     7949 2021-12-11 21:41:38.745625 django-machina-1.2.0/machina/apps/forum_tracking/handler.py
--rw-r--r--   0        0        0     1796 2021-12-11 21:41:38.745707 django-machina-1.2.0/machina/apps/forum_tracking/managers.py
--rw-r--r--   0        0        0     2189 2021-12-11 21:41:38.745857 django-machina-1.2.0/machina/apps/forum_tracking/migrations/0001_initial.py
--rw-r--r--   0        0        0      659 2021-12-11 21:41:38.745919 django-machina-1.2.0/machina/apps/forum_tracking/migrations/0002_auto_20160607_0502.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.745947 django-machina-1.2.0/machina/apps/forum_tracking/migrations/__init__.py
--rw-r--r--   0        0        0      414 2021-12-11 21:41:38.746012 django-machina-1.2.0/machina/apps/forum_tracking/models.py
--rw-r--r--   0        0        0      682 2021-12-11 21:41:38.746091 django-machina-1.2.0/machina/apps/forum_tracking/receivers.py
--rw-r--r--   0        0        0     1597 2021-12-11 21:41:38.746149 django-machina-1.2.0/machina/apps/forum_tracking/urls.py
--rw-r--r--   0        0        0     5469 2021-12-11 21:41:38.746241 django-machina-1.2.0/machina/apps/forum_tracking/views.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.746310 django-machina-1.2.0/machina/conf/__init__.py
--rw-r--r--   0        0        0     4061 2021-12-11 21:41:38.746409 django-machina-1.2.0/machina/conf/settings.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.746522 django-machina-1.2.0/machina/core/__init__.py
--rw-r--r--   0        0        0      605 2021-12-11 21:41:38.746587 django-machina-1.2.0/machina/core/compat.py
--rw-r--r--   0        0        0      304 2021-12-11 21:41:38.746653 django-machina-1.2.0/machina/core/context_processors.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.746716 django-machina-1.2.0/machina/core/db/__init__.py
--rw-r--r--   0        0        0     2225 2021-12-11 21:41:38.746807 django-machina-1.2.0/machina/core/db/models.py
--rw-r--r--   0        0        0     3900 2021-12-11 21:41:38.746886 django-machina-1.2.0/machina/core/loading.py
--rw-r--r--   0        0        0      176 2021-12-11 21:41:38.746945 django-machina-1.2.0/machina/core/markdown.py
--rw-r--r--   0        0        0      360 2021-12-11 21:41:38.747008 django-machina-1.2.0/machina/core/shortcuts.py
--rw-r--r--   0        0        0     1373 2021-12-11 21:41:38.747077 django-machina-1.2.0/machina/core/urls.py
--rw-r--r--   0        0        0     1956 2021-12-11 21:41:38.747139 django-machina-1.2.0/machina/core/validators.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.747197 django-machina-1.2.0/machina/forms/__init__.py
--rw-r--r--   0        0        0     1481 2021-12-11 21:41:38.747280 django-machina-1.2.0/machina/forms/widgets.py
--rw-r--r--   0        0        0     2067 2021-12-11 21:41:38.747458 django-machina-1.2.0/machina/locale/ar/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    17717 2021-12-11 21:41:38.747733 django-machina-1.2.0/machina/locale/ar/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      444 2021-12-11 21:41:38.747987 django-machina-1.2.0/machina/locale/ca/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16437 2021-12-11 21:41:38.748057 django-machina-1.2.0/machina/locale/ca/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    20471 2021-12-11 21:41:38.748300 django-machina-1.2.0/machina/locale/de/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23935 2021-12-11 21:41:38.748491 django-machina-1.2.0/machina/locale/de/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      362 2021-12-11 21:41:38.748621 django-machina-1.2.0/machina/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16378 2021-12-11 21:41:38.748680 django-machina-1.2.0/machina/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    25282 2021-12-11 21:41:38.749005 django-machina-1.2.0/machina/locale/es/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    25969 2021-12-11 21:41:38.749191 django-machina-1.2.0/machina/locale/es/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    27130 2021-12-11 21:41:38.749404 django-machina-1.2.0/machina/locale/fr/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    27205 2021-12-11 21:41:38.749557 django-machina-1.2.0/machina/locale/fr/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    23202 2021-12-11 21:41:38.749718 django-machina-1.2.0/machina/locale/fr_CA/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    25235 2021-12-11 21:41:38.749808 django-machina-1.2.0/machina/locale/fr_CA/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    25007 2021-12-11 21:41:38.750126 django-machina-1.2.0/machina/locale/hu/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    26084 2021-12-11 21:41:38.750264 django-machina-1.2.0/machina/locale/hu/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      479 2021-12-11 21:41:38.750394 django-machina-1.2.0/machina/locale/it/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16472 2021-12-11 21:41:38.750462 django-machina-1.2.0/machina/locale/it/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    24954 2021-12-11 21:41:38.750748 django-machina-1.2.0/machina/locale/ja_JP/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    26429 2021-12-11 21:41:38.750874 django-machina-1.2.0/machina/locale/ja_JP/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    23737 2021-12-11 21:41:38.751164 django-machina-1.2.0/machina/locale/nb/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    24884 2021-12-11 21:41:38.751287 django-machina-1.2.0/machina/locale/nb/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    26378 2021-12-11 21:41:38.751621 django-machina-1.2.0/machina/locale/nl_NL/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    26217 2021-12-11 21:41:38.751745 django-machina-1.2.0/machina/locale/nl_NL/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    23952 2021-12-11 21:41:38.751909 django-machina-1.2.0/machina/locale/pl/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    25214 2021-12-11 21:41:38.751978 django-machina-1.2.0/machina/locale/pl/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      496 2021-12-11 21:41:38.752078 django-machina-1.2.0/machina/locale/pt_BR/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16489 2021-12-11 21:41:38.752132 django-machina-1.2.0/machina/locale/pt_BR/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      521 2021-12-11 21:41:38.752233 django-machina-1.2.0/machina/locale/ro/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16605 2021-12-11 21:41:38.752284 django-machina-1.2.0/machina/locale/ro/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      537 2021-12-11 21:41:38.752383 django-machina-1.2.0/machina/locale/ro_RO/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16621 2021-12-11 21:41:38.752436 django-machina-1.2.0/machina/locale/ro_RO/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    34933 2021-12-11 21:41:38.752663 django-machina-1.2.0/machina/locale/ru/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    34982 2021-12-11 21:41:38.752759 django-machina-1.2.0/machina/locale/ru/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    15365 2021-12-11 21:41:38.752865 django-machina-1.2.0/machina/locale/sl_SI/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    21561 2021-12-11 21:41:38.752930 django-machina-1.2.0/machina/locale/sl_SI/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      472 2021-12-11 21:41:38.753048 django-machina-1.2.0/machina/locale/zh/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16374 2021-12-11 21:41:38.753101 django-machina-1.2.0/machina/locale/zh/LC_MESSAGES/django.po
--rw-r--r--   0        0        0    21955 2021-12-11 21:41:38.753346 django-machina-1.2.0/machina/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    23128 2021-12-11 21:41:38.753512 django-machina-1.2.0/machina/locale/zh_CN/LC_MESSAGES/django.po
--rw-r--r--   0        0        0      487 2021-12-11 21:41:38.753615 django-machina-1.2.0/machina/locale/zh_TW/LC_MESSAGES/django.mo
--rw-r--r--   0        0        0    16389 2021-12-11 21:41:38.753669 django-machina-1.2.0/machina/locale/zh_TW/LC_MESSAGES/django.po
--rw-r--r--   0        0        0       64 2021-12-11 21:41:38.753782 django-machina-1.2.0/machina/models/__init__.py
--rw-r--r--   0        0        0      510 2021-12-11 21:41:38.753839 django-machina-1.2.0/machina/models/abstract_models.py
--rw-r--r--   0        0        0    10513 2021-12-11 21:41:38.753940 django-machina-1.2.0/machina/models/fields.py
--rw-r--r--   0        0        0      131 2021-12-11 21:41:38.754065 django-machina-1.2.0/machina/static/machina/build/README.rst
--rw-r--r--   0        0        0    42739 2021-12-11 21:41:38.754470 django-machina-1.2.0/machina/static/machina/build/css/machina.admin_theme.min.css
--rw-r--r--   0        0        0     4383 2021-12-11 21:41:38.754563 django-machina-1.2.0/machina/static/machina/build/css/machina.board_theme.min.css
--rw-r--r--   0        0        0   181605 2021-12-11 21:41:38.754902 django-machina-1.2.0/machina/static/machina/build/css/machina.board_theme.vendor.min.css
--rw-r--r--   0        0        0    11349 2021-12-11 21:41:38.755031 django-machina-1.2.0/machina/static/machina/build/css/vendor/easymde.min.css
--rw-r--r--   0        0        0   111620 2021-12-11 21:41:38.755673 django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.eot
--rw-r--r--   0        0        0   599658 2021-12-11 21:41:38.757507 django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.svg
--rw-r--r--   0        0        0   111384 2021-12-11 21:41:38.758126 django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.ttf
--rw-r--r--   0        0        0    71560 2021-12-11 21:41:38.758296 django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.woff
--rw-r--r--   0        0        0    61336 2021-12-11 21:41:38.758394 django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.woff2
--rw-r--r--   0        0        0    31272 2021-12-11 21:41:38.758569 django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.eot
--rw-r--r--   0        0        0   104530 2021-12-11 21:41:38.758976 django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.svg
--rw-r--r--   0        0        0    31044 2021-12-11 21:41:38.759164 django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.ttf
--rw-r--r--   0        0        0    14724 2021-12-11 21:41:38.759273 django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.woff
--rw-r--r--   0        0        0    12168 2021-12-11 21:41:38.759324 django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.woff2
--rw-r--r--   0        0        0   133140 2021-12-11 21:41:38.759905 django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.eot
--rw-r--r--   0        0        0   488219 2021-12-11 21:41:38.761393 django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.svg
--rw-r--r--   0        0        0   132920 2021-12-11 21:41:38.762004 django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.ttf
--rw-r--r--   0        0        0    63836 2021-12-11 21:41:38.762153 django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.woff
--rw-r--r--   0        0        0    50388 2021-12-11 21:41:38.762292 django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.woff2
--rw-r--r--   0        0        0      530 2021-12-11 21:41:38.762382 django-machina-1.2.0/machina/static/machina/build/js/machina.editor.min.js
--rw-r--r--   0        0        0     1027 2021-12-11 21:41:38.762437 django-machina-1.2.0/machina/static/machina/build/js/machina.min.js
--rw-r--r--   0        0        0   170131 2021-12-11 21:41:38.763525 django-machina-1.2.0/machina/static/machina/build/js/machina.packages.min.js
--rw-r--r--   0        0        0   311129 2021-12-11 21:41:38.765215 django-machina-1.2.0/machina/static/machina/build/js/vendor/easymde.min.js
--rw-r--r--   0        0        0      821 2021-12-11 21:41:38.765309 django-machina-1.2.0/machina/static/machina/js/editor.js
--rw-r--r--   0        0        0     1911 2021-12-11 21:41:38.765369 django-machina-1.2.0/machina/static/machina/js/ui.js
--rw-r--r--   0        0        0      437 2021-12-11 21:41:38.765472 django-machina-1.2.0/machina/static/machina/sass/admin_pages/forum_change_list.scss
--rw-r--r--   0        0        0     1120 2021-12-11 21:41:38.765526 django-machina-1.2.0/machina/static/machina/sass/admin_pages/forum_permissions.scss
--rw-r--r--   0        0        0      565 2021-12-11 21:41:38.765583 django-machina-1.2.0/machina/static/machina/sass/admin_theme.scss
--rw-r--r--   0        0        0      761 2021-12-11 21:41:38.765668 django-machina-1.2.0/machina/static/machina/sass/board_pages/conversation_post_edit.scss
--rw-r--r--   0        0        0      973 2021-12-11 21:41:38.765726 django-machina-1.2.0/machina/static/machina/sass/board_pages/conversation_topic_detail.scss
--rw-r--r--   0        0        0      829 2021-12-11 21:41:38.765789 django-machina-1.2.0/machina/static/machina/sass/board_pages/forum_detail.scss
--rw-r--r--   0        0        0      815 2021-12-11 21:41:38.765837 django-machina-1.2.0/machina/static/machina/sass/board_pages/forum_lists.scss
--rw-r--r--   0        0        0      687 2021-12-11 21:41:38.765891 django-machina-1.2.0/machina/static/machina/sass/board_pages/member_profile.scss
--rw-r--r--   0        0        0      584 2021-12-11 21:41:38.765958 django-machina-1.2.0/machina/static/machina/sass/board_pages/moderation.scss
--rw-r--r--   0        0        0      578 2021-12-11 21:41:38.766015 django-machina-1.2.0/machina/static/machina/sass/board_pages/search.scss
--rw-r--r--   0        0        0      439 2021-12-11 21:41:38.766078 django-machina-1.2.0/machina/static/machina/sass/board_theme.scss
--rw-r--r--   0        0        0      434 2021-12-11 21:41:38.766131 django-machina-1.2.0/machina/static/machina/sass/board_theme.vendor.scss
--rw-r--r--   0        0        0      759 2021-12-11 21:41:38.766190 django-machina-1.2.0/machina/static/machina/sass/variables.scss
--rw-r--r--   0        0        0      259 2021-12-11 21:41:38.766375 django-machina-1.2.0/machina/templates/admin/forum/forum/change_form.html
--rw-r--r--   0        0        0      913 2021-12-11 21:41:38.766455 django-machina-1.2.0/machina/templates/admin/forum/forum/change_list.html
--rw-r--r--   0        0        0     3525 2021-12-11 21:41:38.766531 django-machina-1.2.0/machina/templates/admin/forum/forum/change_list_table.html
--rw-r--r--   0        0        0      159 2021-12-11 21:41:38.766594 django-machina-1.2.0/machina/templates/admin/forum/forum/editpermissions_anonymous_user.html
--rw-r--r--   0        0        0      174 2021-12-11 21:41:38.766654 django-machina-1.2.0/machina/templates/admin/forum/forum/editpermissions_authenticated_user.html
--rw-r--r--   0        0        0     3344 2021-12-11 21:41:38.766746 django-machina-1.2.0/machina/templates/admin/forum/forum/editpermissions_form.html
--rw-r--r--   0        0        0      160 2021-12-11 21:41:38.766828 django-machina-1.2.0/machina/templates/admin/forum/forum/editpermissions_group.html
--rw-r--r--   0        0        0     6006 2021-12-11 21:41:38.766915 django-machina-1.2.0/machina/templates/admin/forum/forum/editpermissions_index.html
--rw-r--r--   0        0        0      159 2021-12-11 21:41:38.766969 django-machina-1.2.0/machina/templates/admin/forum/forum/editpermissions_user.html
--rw-r--r--   0        0        0     1190 2021-12-11 21:41:38.767078 django-machina-1.2.0/machina/templates/machina/_base.html
--rw-r--r--   0        0        0     3262 2021-12-11 21:41:38.767141 django-machina-1.2.0/machina/templates/machina/board_base.html
--rw-r--r--   0        0        0     2837 2021-12-11 21:41:38.767253 django-machina-1.2.0/machina/templates/machina/forum/forum_detail.html
--rw-r--r--   0        0        0    10802 2021-12-11 21:41:38.767382 django-machina-1.2.0/machina/templates/machina/forum/forum_list.html
--rw-r--r--   0        0        0     1012 2021-12-11 21:41:38.767593 django-machina-1.2.0/machina/templates/machina/forum/index.html
--rw-r--r--   0        0        0     1593 2021-12-11 21:41:38.767738 django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_attachments/attachment_formset.html
--rw-r--r--   0        0        0      809 2021-12-11 21:41:38.767804 django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_attachments/attachments_detail.html
--rw-r--r--   0        0        0      622 2021-12-11 21:41:38.767869 django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_attachments/attachments_preview.html
--rw-r--r--   0        0        0     2129 2021-12-11 21:41:38.767978 django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_detail.html
--rw-r--r--   0        0        0     1013 2021-12-11 21:41:38.768051 django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_option_formset.html
--rw-r--r--   0        0        0     2046 2021-12-11 21:41:38.768117 django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_preview.html
--rw-r--r--   0        0        0      635 2021-12-11 21:41:38.768182 django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_results.html
--rw-r--r--   0        0        0     1152 2021-12-11 21:41:38.768248 django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_vote_form.html
--rw-r--r--   0        0        0     2170 2021-12-11 21:41:38.768380 django-machina-1.2.0/machina/templates/machina/forum_conversation/partials/post_form.html
--rw-r--r--   0        0        0     4241 2021-12-11 21:41:38.768459 django-machina-1.2.0/machina/templates/machina/forum_conversation/partials/topic_detail_actions.html
--rw-r--r--   0        0        0     4032 2021-12-11 21:41:38.768543 django-machina-1.2.0/machina/templates/machina/forum_conversation/partials/topic_form.html
--rw-r--r--   0        0        0     3197 2021-12-11 21:41:38.768620 django-machina-1.2.0/machina/templates/machina/forum_conversation/post_create.html
--rw-r--r--   0        0        0      956 2021-12-11 21:41:38.768709 django-machina-1.2.0/machina/templates/machina/forum_conversation/post_delete.html
--rw-r--r--   0        0        0      648 2021-12-11 21:41:38.768772 django-machina-1.2.0/machina/templates/machina/forum_conversation/post_preview.html
--rw-r--r--   0        0        0     1324 2021-12-11 21:41:38.768830 django-machina-1.2.0/machina/templates/machina/forum_conversation/post_update.html
--rw-r--r--   0        0        0     1046 2021-12-11 21:41:38.768881 django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_create.html
--rw-r--r--   0        0        0     5810 2021-12-11 21:41:38.768971 django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_detail.html
--rw-r--r--   0        0        0     4424 2021-12-11 21:41:38.769046 django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_list.html
--rw-r--r--   0        0        0      566 2021-12-11 21:41:38.769112 django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_pages_inline_list.html
--rw-r--r--   0        0        0     1032 2021-12-11 21:41:38.769180 django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_update.html
--rw-r--r--   0        0        0      321 2021-12-11 21:41:38.769276 django-machina-1.2.0/machina/templates/machina/forum_feeds/topics_description.html
--rw-r--r--   0        0        0       42 2021-12-11 21:41:38.769331 django-machina-1.2.0/machina/templates/machina/forum_feeds/topics_title.html
--rw-r--r--   0        0        0     3611 2021-12-11 21:41:38.769450 django-machina-1.2.0/machina/templates/machina/forum_member/forum_profile_detail.html
--rw-r--r--   0        0        0     1992 2021-12-11 21:41:38.769505 django-machina-1.2.0/machina/templates/machina/forum_member/forum_profile_update.html
--rw-r--r--   0        0        0     1259 2021-12-11 21:41:38.769571 django-machina-1.2.0/machina/templates/machina/forum_member/subscription_topic_list.html
--rw-r--r--   0        0        0      970 2021-12-11 21:41:38.769632 django-machina-1.2.0/machina/templates/machina/forum_member/topic_subscribe.html
--rw-r--r--   0        0        0      982 2021-12-11 21:41:38.769692 django-machina-1.2.0/machina/templates/machina/forum_member/topic_unsubscribe.html
--rw-r--r--   0        0        0     3364 2021-12-11 21:41:38.769752 django-machina-1.2.0/machina/templates/machina/forum_member/user_posts_list.html
--rw-r--r--   0        0        0     6990 2021-12-11 21:41:38.769919 django-machina-1.2.0/machina/templates/machina/forum_moderation/moderation_queue/detail.html
--rw-r--r--   0        0        0     3720 2021-12-11 21:41:38.770003 django-machina-1.2.0/machina/templates/machina/forum_moderation/moderation_queue/list.html
--rw-r--r--   0        0        0      918 2021-12-11 21:41:38.770059 django-machina-1.2.0/machina/templates/machina/forum_moderation/moderation_queue/post_approve.html
--rw-r--r--   0        0        0      904 2021-12-11 21:41:38.770115 django-machina-1.2.0/machina/templates/machina/forum_moderation/moderation_queue/post_disapprove.html
--rw-r--r--   0        0        0      960 2021-12-11 21:41:38.770170 django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_delete.html
--rw-r--r--   0        0        0      952 2021-12-11 21:41:38.770227 django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_lock.html
--rw-r--r--   0        0        0     1068 2021-12-11 21:41:38.770282 django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_move.html
--rw-r--r--   0        0        0      960 2021-12-11 21:41:38.770367 django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_unlock.html
--rw-r--r--   0        0        0      932 2021-12-11 21:41:38.770421 django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_update_type.html
--rw-r--r--   0        0        0     1962 2022-01-16 23:11:03.535945 django-machina-1.2.0/machina/templates/machina/forum_search/pagination.html
--rw-r--r--   0        0        0       51 2021-12-11 21:41:38.770559 django-machina-1.2.0/machina/templates/machina/forum_search/post_text.txt
--rw-r--r--   0        0        0     4126 2021-12-11 21:41:38.770629 django-machina-1.2.0/machina/templates/machina/forum_search/search.html
--rw-r--r--   0        0        0      888 2021-12-11 21:41:38.770716 django-machina-1.2.0/machina/templates/machina/forum_tracking/mark_forums_read.html
--rw-r--r--   0        0        0      878 2021-12-11 21:41:38.770773 django-machina-1.2.0/machina/templates/machina/forum_tracking/mark_topics_read.html
--rw-r--r--   0        0        0     1218 2021-12-11 21:41:38.770842 django-machina-1.2.0/machina/templates/machina/forum_tracking/unread_topic_list.html
--rw-r--r--   0        0        0      271 2021-12-11 21:41:38.770941 django-machina-1.2.0/machina/templates/machina/partials/avatar.html
--rw-r--r--   0        0        0      737 2021-12-11 21:41:38.771014 django-machina-1.2.0/machina/templates/machina/partials/breadcrumb.html
--rw-r--r--   0        0        0      647 2021-12-11 21:41:38.771074 django-machina-1.2.0/machina/templates/machina/partials/form_field.html
--rw-r--r--   0        0        0      329 2021-12-11 21:41:38.771138 django-machina-1.2.0/machina/templates/machina/partials/messages.html
--rw-r--r--   0        0        0     1993 2021-12-11 21:41:38.771191 django-machina-1.2.0/machina/templates/machina/partials/pagination.html
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.771246 django-machina-1.2.0/machina/templatetags/__init__.py
--rw-r--r--   0        0        0     1010 2021-12-11 21:41:38.771322 django-machina-1.2.0/machina/templatetags/forum_conversation_tags.py
--rw-r--r--   0        0        0      261 2021-12-11 21:41:38.771378 django-machina-1.2.0/machina/templatetags/forum_markup_tags.py
--rw-r--r--   0        0        0      448 2021-12-11 21:41:38.771431 django-machina-1.2.0/machina/templatetags/forum_member_tags.py
--rw-r--r--   0        0        0     1120 2021-12-11 21:41:38.771494 django-machina-1.2.0/machina/templatetags/forum_permission_tags.py
--rw-r--r--   0        0        0      938 2021-12-11 21:41:38.771547 django-machina-1.2.0/machina/templatetags/forum_polls_tags.py
--rw-r--r--   0        0        0     2609 2021-12-11 21:41:38.771605 django-machina-1.2.0/machina/templatetags/forum_tags.py
--rw-r--r--   0        0        0      574 2021-12-11 21:41:38.771658 django-machina-1.2.0/machina/templatetags/forum_tracking_tags.py
--rw-r--r--   0        0        0        0 2021-12-11 21:41:38.771707 django-machina-1.2.0/machina/test/__init__.py
--rw-r--r--   0        0        0      955 2021-12-11 21:41:38.771778 django-machina-1.2.0/machina/test/context_managers.py
--rw-r--r--   0        0        0      248 2021-12-11 21:41:38.771868 django-machina-1.2.0/machina/test/factories/__init__.py
--rw-r--r--   0        0        0      474 2021-12-11 21:41:38.771935 django-machina-1.2.0/machina/test/factories/attachments.py
--rw-r--r--   0        0        0      879 2021-12-11 21:41:38.771992 django-machina-1.2.0/machina/test/factories/auth.py
--rw-r--r--   0        0        0     1410 2021-12-11 21:41:38.772049 django-machina-1.2.0/machina/test/factories/conversation.py
--rw-r--r--   0        0        0     1630 2021-12-11 21:41:38.772098 django-machina-1.2.0/machina/test/factories/forum.py
--rw-r--r--   0        0        0      853 2021-12-11 21:41:38.772144 django-machina-1.2.0/machina/test/factories/permission.py
--rw-r--r--   0        0        0     1023 2021-12-11 21:41:38.772189 django-machina-1.2.0/machina/test/factories/polls.py
--rw-r--r--   0        0        0      782 2021-12-11 21:41:38.772239 django-machina-1.2.0/machina/test/factories/tracking.py
--rw-r--r--   0        0        0      888 2021-12-11 21:41:38.772292 django-machina-1.2.0/machina/test/mixins.py
--rw-r--r--   0        0        0     1420 2021-12-11 21:41:38.772357 django-machina-1.2.0/machina/test/testcases.py
--rw-r--r--   0        0        0     1882 2022-04-24 02:08:26.857790 django-machina-1.2.0/machina/urls.py
--rw-r--r--   0        0        0     1849 2022-05-16 22:40:21.329915 django-machina-1.2.0/pyproject.toml
--rw-r--r--   0        0        0     5298 2022-05-16 22:53:28.039606 django-machina-1.2.0/setup.py
--rw-r--r--   0        0        0     2857 2022-05-16 22:53:28.039809 django-machina-1.2.0/PKG-INFO
+-rw-r--r--   0        0        0      483 2021-12-11 21:41:38.728460 django_machina-1.3.0/AUTHORS
+-rw-r--r--   0        0        0      209 2021-12-11 21:41:38.728521 django_machina-1.3.0/CHANGELOG.rst
+-rw-r--r--   0        0        0      280 2021-12-11 21:41:38.728580 django_machina-1.3.0/CONTRIBUTING.rst
+-rw-r--r--   0        0        0     1515 2023-02-16 11:13:42.000000 django_machina-1.3.0/LICENSE
+-rw-r--r--   0        0        0     1540 2023-05-28 01:15:00.427069 django_machina-1.3.0/README.rst
+-rw-r--r--   0        0        0      516 2021-12-11 21:41:38.736589 django_machina-1.3.0/machina/__init__.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.736652 django_machina-1.3.0/machina/apps/__init__.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:23:54.035719 django_machina-1.3.0/machina/apps/forum/__init__.py
+-rw-r--r--   0        0        0     8200 2021-12-11 21:41:38.736832 django_machina-1.3.0/machina/apps/forum/abstract_models.py
+-rw-r--r--   0        0        0    20089 2022-04-24 02:08:48.835350 django_machina-1.3.0/machina/apps/forum/admin.py
+-rw-r--r--   0        0        0      614 2021-12-11 21:41:38.736999 django_machina-1.3.0/machina/apps/forum/apps.py
+-rw-r--r--   0        0        0     4255 2021-12-11 21:41:38.737073 django_machina-1.3.0/machina/apps/forum/forms.py
+-rw-r--r--   0        0        0     3267 2021-12-11 21:41:38.737188 django_machina-1.3.0/machina/apps/forum/migrations/0001_initial.py
+-rw-r--r--   0        0        0      423 2021-12-11 21:41:38.737250 django_machina-1.3.0/machina/apps/forum/migrations/0002_auto_20150725_0512.py
+-rw-r--r--   0        0        0      392 2021-12-11 21:41:38.737307 django_machina-1.3.0/machina/apps/forum/migrations/0003_remove_forum_is_active.py
+-rw-r--r--   0        0        0      772 2021-12-11 21:41:38.737364 django_machina-1.3.0/machina/apps/forum/migrations/0004_auto_20170504_2108.py
+-rw-r--r--   0        0        0      847 2021-12-11 21:41:38.737422 django_machina-1.3.0/machina/apps/forum/migrations/0005_auto_20170504_2113.py
+-rw-r--r--   0        0        0      503 2021-12-11 21:41:38.737474 django_machina-1.3.0/machina/apps/forum/migrations/0006_auto_20170523_2036.py
+-rw-r--r--   0        0        0      748 2021-12-11 21:41:38.737528 django_machina-1.3.0/machina/apps/forum/migrations/0007_auto_20170523_2140.py
+-rw-r--r--   0        0        0      686 2021-12-11 21:41:38.737579 django_machina-1.3.0/machina/apps/forum/migrations/0008_forum_last_post.py
+-rw-r--r--   0        0        0      789 2021-12-11 21:41:38.737635 django_machina-1.3.0/machina/apps/forum/migrations/0009_auto_20170928_2327.py
+-rw-r--r--   0        0        0      577 2021-12-11 21:41:38.737695 django_machina-1.3.0/machina/apps/forum/migrations/0010_auto_20181103_1401.py
+-rw-r--r--   0        0        0      717 2021-12-11 21:41:38.737747 django_machina-1.3.0/machina/apps/forum/migrations/0011_auto_20190627_2132.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.737771 django_machina-1.3.0/machina/apps/forum/migrations/__init__.py
+-rw-r--r--   0        0        0      264 2021-12-11 21:41:38.737836 django_machina-1.3.0/machina/apps/forum/models.py
+-rw-r--r--   0        0        0      565 2021-12-11 21:41:38.737893 django_machina-1.3.0/machina/apps/forum/receivers.py
+-rw-r--r--   0        0        0      324 2022-04-24 02:08:01.104191 django_machina-1.3.0/machina/apps/forum/signals.py
+-rw-r--r--   0        0        0      945 2021-12-11 21:41:38.738007 django_machina-1.3.0/machina/apps/forum/urls.py
+-rw-r--r--   0        0        0     4546 2021-12-11 21:41:38.738103 django_machina-1.3.0/machina/apps/forum/views.py
+-rw-r--r--   0        0        0     9198 2021-12-11 21:41:38.738195 django_machina-1.3.0/machina/apps/forum/visibility.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:23:56.281039 django_machina-1.3.0/machina/apps/forum_conversation/__init__.py
+-rw-r--r--   0        0        0    13112 2021-12-11 21:41:38.738395 django_machina-1.3.0/machina/apps/forum_conversation/abstract_models.py
+-rw-r--r--   0        0        0     1443 2021-12-11 21:41:38.738458 django_machina-1.3.0/machina/apps/forum_conversation/admin.py
+-rw-r--r--   0        0        0      692 2021-12-11 21:41:38.738508 django_machina-1.3.0/machina/apps/forum_conversation/apps.py
+-rw-r--r--   0        0        0     9626 2022-10-13 18:52:02.265712 django_machina-1.3.0/machina/apps/forum_conversation/forms.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:23:58.539579 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/__init__.py
+-rw-r--r--   0        0        0     1564 2021-12-11 21:41:38.738709 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/abstract_models.py
+-rw-r--r--   0        0        0      608 2021-12-11 21:41:38.738769 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/admin.py
+-rw-r--r--   0        0        0      558 2021-12-11 21:41:38.738821 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/apps.py
+-rw-r--r--   0        0        0     4544 2021-12-11 21:41:38.738896 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/cache.py
+-rw-r--r--   0        0        0     1275 2021-12-11 21:41:38.738963 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/forms.py
+-rw-r--r--   0        0        0     1004 2021-12-11 21:41:38.739061 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/migrations/0001_initial.py
+-rw-r--r--   0        0        0      573 2021-12-11 21:41:38.739119 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/migrations/0002_auto_20181103_1404.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.739141 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/migrations/__init__.py
+-rw-r--r--   0        0        0      346 2021-12-11 21:41:38.739195 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/models.py
+-rw-r--r--   0        0        0      854 2021-12-11 21:41:38.739249 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/urls.py
+-rw-r--r--   0        0        0     1522 2021-12-11 21:41:38.739315 django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/views.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:24:00.838464 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/__init__.py
+-rw-r--r--   0        0        0     4296 2022-10-13 18:52:02.265845 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/abstract_models.py
+-rw-r--r--   0        0        0     1290 2022-10-13 18:52:02.265963 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/admin.py
+-rw-r--r--   0        0        0      522 2021-12-11 21:41:38.739609 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/apps.py
+-rw-r--r--   0        0        0     4624 2022-10-13 18:52:02.266080 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/forms.py
+-rw-r--r--   0        0        0     3237 2021-12-11 21:41:38.739780 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/migrations/0001_initial.py
+-rw-r--r--   0        0        0      777 2021-12-11 21:41:38.739834 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/migrations/0002_auto_20151105_0029.py
+-rw-r--r--   0        0        0      430 2022-10-13 18:52:02.266169 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/migrations/0003_topicpoll_hide_results.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.739857 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/migrations/__init__.py
+-rw-r--r--   0        0        0      485 2021-12-11 21:41:38.739908 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/models.py
+-rw-r--r--   0        0        0      817 2021-12-11 21:41:38.739965 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/urls.py
+-rw-r--r--   0        0        0      375 2021-12-11 21:41:38.740025 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/validators.py
+-rw-r--r--   0        0        0     3338 2021-12-11 21:41:38.740103 django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/views.py
+-rw-r--r--   0        0        0      400 2021-12-11 21:41:38.740160 django_machina-1.3.0/machina/apps/forum_conversation/managers.py
+-rw-r--r--   0        0        0     4686 2021-12-11 21:41:38.740239 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0001_initial.py
+-rw-r--r--   0        0        0      470 2021-12-11 21:41:38.740293 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0002_post_anonymous_key.py
+-rw-r--r--   0        0        0      637 2021-12-11 21:41:38.740349 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0003_auto_20160228_2051.py
+-rw-r--r--   0        0        0      594 2021-12-11 21:41:38.740398 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0004_auto_20160427_0502.py
+-rw-r--r--   0        0        0      699 2021-12-11 21:41:38.740460 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0005_auto_20160607_0455.py
+-rw-r--r--   0        0        0      519 2021-12-11 21:41:38.740529 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0006_post_enable_signature.py
+-rw-r--r--   0        0        0      942 2021-12-11 21:41:38.740588 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0007_auto_20160903_0450.py
+-rw-r--r--   0        0        0      902 2021-12-11 21:41:38.740646 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0008_auto_20160903_0512.py
+-rw-r--r--   0        0        0      481 2021-12-11 21:41:38.740698 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0009_auto_20160925_2126.py
+-rw-r--r--   0        0        0      644 2021-12-11 21:41:38.740748 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0010_auto_20170120_0224.py
+-rw-r--r--   0        0        0      340 2021-12-11 21:41:38.740806 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0011_remove_post_poster_ip.py
+-rw-r--r--   0        0        0      575 2021-12-11 21:41:38.740864 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0012_auto_20200423_1049.py
+-rw-r--r--   0        0        0     1043 2021-12-11 21:41:38.740936 django_machina-1.3.0/machina/apps/forum_conversation/migrations/0013_auto_20201220_1745.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.740966 django_machina-1.3.0/machina/apps/forum_conversation/migrations/__init__.py
+-rw-r--r--   0        0        0      365 2021-12-11 21:41:38.741038 django_machina-1.3.0/machina/apps/forum_conversation/models.py
+-rw-r--r--   0        0        0      543 2021-12-11 21:41:38.741106 django_machina-1.3.0/machina/apps/forum_conversation/receivers.py
+-rw-r--r--   0        0        0      271 2021-12-11 21:41:38.741166 django_machina-1.3.0/machina/apps/forum_conversation/signals.py
+-rw-r--r--   0        0        0     3903 2021-12-11 21:41:38.741240 django_machina-1.3.0/machina/apps/forum_conversation/urls.py
+-rw-r--r--   0        0        0    29633 2022-10-13 18:52:02.266342 django_machina-1.3.0/machina/apps/forum_conversation/views.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:24:05.990706 django_machina-1.3.0/machina/apps/forum_feeds/__init__.py
+-rw-r--r--   0        0        0      503 2021-12-11 21:41:38.741533 django_machina-1.3.0/machina/apps/forum_feeds/apps.py
+-rw-r--r--   0        0        0     2326 2021-12-11 21:41:38.741613 django_machina-1.3.0/machina/apps/forum_feeds/feeds.py
+-rw-r--r--   0        0        0     1246 2021-12-11 21:41:38.741680 django_machina-1.3.0/machina/apps/forum_feeds/urls.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:24:08.124945 django_machina-1.3.0/machina/apps/forum_member/__init__.py
+-rw-r--r--   0        0        0     2192 2021-12-11 21:41:38.741879 django_machina-1.3.0/machina/apps/forum_member/abstract_models.py
+-rw-r--r--   0        0        0      835 2021-12-11 21:41:38.741994 django_machina-1.3.0/machina/apps/forum_member/admin.py
+-rw-r--r--   0        0        0      656 2021-12-11 21:41:38.742066 django_machina-1.3.0/machina/apps/forum_member/apps.py
+-rw-r--r--   0        0        0      628 2021-12-11 21:41:38.742129 django_machina-1.3.0/machina/apps/forum_member/forms.py
+-rw-r--r--   0        0        0     1410 2021-12-11 21:41:38.742235 django_machina-1.3.0/machina/apps/forum_member/migrations/0001_initial.py
+-rw-r--r--   0        0        0      644 2021-12-11 21:41:38.742310 django_machina-1.3.0/machina/apps/forum_member/migrations/0002_auto_20160225_0515.py
+-rw-r--r--   0        0        0      665 2021-12-11 21:41:38.742368 django_machina-1.3.0/machina/apps/forum_member/migrations/0003_auto_20160227_2122.py
+-rw-r--r--   0        0        0      604 2021-12-11 21:41:38.742425 django_machina-1.3.0/machina/apps/forum_member/migrations/0004_auto_20181103_1406.py
+-rw-r--r--   0        0        0      600 2021-12-11 21:41:38.742485 django_machina-1.3.0/machina/apps/forum_member/migrations/0005_auto_20200423_1049.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.742512 django_machina-1.3.0/machina/apps/forum_member/migrations/__init__.py
+-rw-r--r--   0        0        0      313 2021-12-11 21:41:38.742570 django_machina-1.3.0/machina/apps/forum_member/models.py
+-rw-r--r--   0        0        0     3883 2022-01-30 20:21:22.499709 django_machina-1.3.0/machina/apps/forum_member/receivers.py
+-rw-r--r--   0        0        0      395 2021-12-11 21:41:38.742715 django_machina-1.3.0/machina/apps/forum_member/shortcuts.py
+-rw-r--r--   0        0        0     2185 2021-12-11 21:41:38.742780 django_machina-1.3.0/machina/apps/forum_member/urls.py
+-rw-r--r--   0        0        0     8767 2021-12-11 21:41:38.742880 django_machina-1.3.0/machina/apps/forum_member/views.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:24:10.082345 django_machina-1.3.0/machina/apps/forum_moderation/__init__.py
+-rw-r--r--   0        0        0      533 2021-12-11 21:41:38.743067 django_machina-1.3.0/machina/apps/forum_moderation/apps.py
+-rw-r--r--   0        0        0     2022 2021-12-11 21:41:38.743148 django_machina-1.3.0/machina/apps/forum_moderation/forms.py
+-rw-r--r--   0        0        0     3608 2021-12-11 21:41:38.743215 django_machina-1.3.0/machina/apps/forum_moderation/urls.py
+-rw-r--r--   0        0        0    17440 2021-12-11 21:41:38.743372 django_machina-1.3.0/machina/apps/forum_moderation/views.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:24:12.220784 django_machina-1.3.0/machina/apps/forum_permission/__init__.py
+-rw-r--r--   0        0        0     4489 2021-12-11 21:41:38.743570 django_machina-1.3.0/machina/apps/forum_permission/abstract_models.py
+-rw-r--r--   0        0        0     1623 2021-12-11 21:41:38.743647 django_machina-1.3.0/machina/apps/forum_permission/admin.py
+-rw-r--r--   0        0        0      680 2021-12-11 21:41:38.743704 django_machina-1.3.0/machina/apps/forum_permission/apps.py
+-rw-r--r--   0        0        0    15495 2021-12-11 21:41:38.743850 django_machina-1.3.0/machina/apps/forum_permission/checker.py
+-rw-r--r--   0        0        0     4045 2021-12-11 21:41:38.743918 django_machina-1.3.0/machina/apps/forum_permission/defaults.py
+-rw-r--r--   0        0        0    16447 2021-12-11 21:41:38.744082 django_machina-1.3.0/machina/apps/forum_permission/handler.py
+-rw-r--r--   0        0        0     1631 2021-12-11 21:41:38.744169 django_machina-1.3.0/machina/apps/forum_permission/middleware.py
+-rw-r--r--   0        0        0     3646 2021-12-11 21:41:38.744277 django_machina-1.3.0/machina/apps/forum_permission/migrations/0001_initial.py
+-rw-r--r--   0        0        0     1749 2021-12-11 21:41:38.744344 django_machina-1.3.0/machina/apps/forum_permission/migrations/0002_auto_20160607_0500.py
+-rw-r--r--   0        0        0      407 2021-12-11 21:41:38.744407 django_machina-1.3.0/machina/apps/forum_permission/migrations/0003_remove_forumpermission_name.py
+-rw-r--r--   0        0        0      472 2021-12-11 21:41:38.744475 django_machina-1.3.0/machina/apps/forum_permission/migrations/0004_auto_20190319_2240.py
+-rw-r--r--   0        0        0      478 2021-12-11 21:41:38.744539 django_machina-1.3.0/machina/apps/forum_permission/migrations/0005_userforumpermission_authenticated_user.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.744562 django_machina-1.3.0/machina/apps/forum_permission/migrations/__init__.py
+-rw-r--r--   0        0        0      537 2021-12-11 21:41:38.744621 django_machina-1.3.0/machina/apps/forum_permission/models.py
+-rw-r--r--   0        0        0      924 2021-12-11 21:41:38.744675 django_machina-1.3.0/machina/apps/forum_permission/receivers.py
+-rw-r--r--   0        0        0     3919 2021-12-11 21:41:38.744752 django_machina-1.3.0/machina/apps/forum_permission/shortcuts.py
+-rw-r--r--   0        0        0     4529 2021-12-11 21:41:38.744829 django_machina-1.3.0/machina/apps/forum_permission/viewmixins.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:24:17.017613 django_machina-1.3.0/machina/apps/forum_search/__init__.py
+-rw-r--r--   0        0        0      511 2021-12-11 21:41:38.744973 django_machina-1.3.0/machina/apps/forum_search/apps.py
+-rw-r--r--   0        0        0     2810 2021-12-11 21:41:38.745046 django_machina-1.3.0/machina/apps/forum_search/forms.py
+-rw-r--r--   0        0        0     1873 2021-12-11 21:41:38.745121 django_machina-1.3.0/machina/apps/forum_search/search_indexes.py
+-rw-r--r--   0        0        0     1032 2021-12-11 21:41:38.745185 django_machina-1.3.0/machina/apps/forum_search/urls.py
+-rw-r--r--   0        0        0      421 2021-12-11 21:41:38.745243 django_machina-1.3.0/machina/apps/forum_search/views.py
+-rw-r--r--   0        0        0        0 2022-04-24 02:24:20.827183 django_machina-1.3.0/machina/apps/forum_tracking/__init__.py
+-rw-r--r--   0        0        0     2050 2021-12-11 21:41:38.745412 django_machina-1.3.0/machina/apps/forum_tracking/abstract_models.py
+-rw-r--r--   0        0        0      890 2021-12-11 21:41:38.745478 django_machina-1.3.0/machina/apps/forum_tracking/admin.py
+-rw-r--r--   0        0        0      667 2021-12-11 21:41:38.745532 django_machina-1.3.0/machina/apps/forum_tracking/apps.py
+-rw-r--r--   0        0        0     7949 2021-12-11 21:41:38.745625 django_machina-1.3.0/machina/apps/forum_tracking/handler.py
+-rw-r--r--   0        0        0     1796 2021-12-11 21:41:38.745707 django_machina-1.3.0/machina/apps/forum_tracking/managers.py
+-rw-r--r--   0        0        0     2189 2021-12-11 21:41:38.745857 django_machina-1.3.0/machina/apps/forum_tracking/migrations/0001_initial.py
+-rw-r--r--   0        0        0      659 2021-12-11 21:41:38.745919 django_machina-1.3.0/machina/apps/forum_tracking/migrations/0002_auto_20160607_0502.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.745947 django_machina-1.3.0/machina/apps/forum_tracking/migrations/__init__.py
+-rw-r--r--   0        0        0      414 2021-12-11 21:41:38.746012 django_machina-1.3.0/machina/apps/forum_tracking/models.py
+-rw-r--r--   0        0        0      682 2021-12-11 21:41:38.746091 django_machina-1.3.0/machina/apps/forum_tracking/receivers.py
+-rw-r--r--   0        0        0     1597 2021-12-11 21:41:38.746149 django_machina-1.3.0/machina/apps/forum_tracking/urls.py
+-rw-r--r--   0        0        0     5469 2021-12-11 21:41:38.746241 django_machina-1.3.0/machina/apps/forum_tracking/views.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.746310 django_machina-1.3.0/machina/conf/__init__.py
+-rw-r--r--   0        0        0     4061 2021-12-11 21:41:38.746409 django_machina-1.3.0/machina/conf/settings.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.746522 django_machina-1.3.0/machina/core/__init__.py
+-rw-r--r--   0        0        0      605 2021-12-11 21:41:38.746587 django_machina-1.3.0/machina/core/compat.py
+-rw-r--r--   0        0        0      304 2021-12-11 21:41:38.746653 django_machina-1.3.0/machina/core/context_processors.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.746716 django_machina-1.3.0/machina/core/db/__init__.py
+-rw-r--r--   0        0        0     2225 2021-12-11 21:41:38.746807 django_machina-1.3.0/machina/core/db/models.py
+-rw-r--r--   0        0        0     4028 2023-02-19 21:44:06.934620 django_machina-1.3.0/machina/core/loading.py
+-rw-r--r--   0        0        0      176 2021-12-11 21:41:38.746945 django_machina-1.3.0/machina/core/markdown.py
+-rw-r--r--   0        0        0      360 2021-12-11 21:41:38.747008 django_machina-1.3.0/machina/core/shortcuts.py
+-rw-r--r--   0        0        0     1373 2021-12-11 21:41:38.747077 django_machina-1.3.0/machina/core/urls.py
+-rw-r--r--   0        0        0     1956 2021-12-11 21:41:38.747139 django_machina-1.3.0/machina/core/validators.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.747197 django_machina-1.3.0/machina/forms/__init__.py
+-rw-r--r--   0        0        0     1481 2021-12-11 21:41:38.747280 django_machina-1.3.0/machina/forms/widgets.py
+-rw-r--r--   0        0        0     2067 2023-02-19 21:58:33.438043 django_machina-1.3.0/machina/locale/ar/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    18001 2023-02-19 21:58:13.896185 django_machina-1.3.0/machina/locale/ar/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      444 2023-02-19 21:58:33.418185 django_machina-1.3.0/machina/locale/ca/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16788 2023-02-19 21:58:13.702809 django_machina-1.3.0/machina/locale/ca/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      522 2023-02-19 21:58:33.461512 django_machina-1.3.0/machina/locale/cs/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    17048 2023-02-19 21:58:13.731360 django_machina-1.3.0/machina/locale/cs/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    20471 2023-02-19 21:58:33.409222 django_machina-1.3.0/machina/locale/de/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    24321 2023-02-19 21:58:13.948262 django_machina-1.3.0/machina/locale/de/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      442 2023-02-19 21:58:33.421971 django_machina-1.3.0/machina/locale/el/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16786 2023-02-19 21:58:13.673233 django_machina-1.3.0/machina/locale/el/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      362 2023-02-19 21:58:33.496103 django_machina-1.3.0/machina/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16729 2023-02-19 21:58:14.003936 django_machina-1.3.0/machina/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    25282 2023-02-19 21:58:33.417819 django_machina-1.3.0/machina/locale/es/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    26646 2023-02-19 21:58:13.986523 django_machina-1.3.0/machina/locale/es/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    27102 2023-02-19 21:58:33.409272 django_machina-1.3.0/machina/locale/fr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27874 2023-02-19 21:58:13.966436 django_machina-1.3.0/machina/locale/fr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    23202 2023-02-19 21:58:33.423346 django_machina-1.3.0/machina/locale/fr_CA/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    25912 2023-02-19 21:58:13.764503 django_machina-1.3.0/machina/locale/fr_CA/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    25007 2023-02-19 21:58:33.425485 django_machina-1.3.0/machina/locale/hu/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    26787 2023-02-19 21:58:13.914886 django_machina-1.3.0/machina/locale/hu/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      479 2023-02-19 21:58:33.437530 django_machina-1.3.0/machina/locale/it/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16823 2023-02-19 21:58:13.687887 django_machina-1.3.0/machina/locale/it/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    24954 2023-02-19 21:58:33.437940 django_machina-1.3.0/machina/locale/ja_JP/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    27110 2023-02-19 21:58:13.826027 django_machina-1.3.0/machina/locale/ja_JP/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    23737 2023-02-19 21:58:33.416386 django_machina-1.3.0/machina/locale/nb/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    25561 2023-02-19 21:58:13.931018 django_machina-1.3.0/machina/locale/nb/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    26378 2023-02-19 21:58:33.461896 django_machina-1.3.0/machina/locale/nl_NL/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    26854 2023-02-19 21:58:13.864116 django_machina-1.3.0/machina/locale/nl_NL/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    23952 2023-02-19 21:58:33.427541 django_machina-1.3.0/machina/locale/pl/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    25893 2023-02-19 21:58:13.644846 django_machina-1.3.0/machina/locale/pl/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      496 2023-02-19 21:58:33.495759 django_machina-1.3.0/machina/locale/pt_BR/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16840 2023-02-19 21:58:13.658084 django_machina-1.3.0/machina/locale/pt_BR/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      521 2023-02-19 21:58:33.525215 django_machina-1.3.0/machina/locale/ro/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16956 2023-02-19 21:58:13.794138 django_machina-1.3.0/machina/locale/ro/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      537 2023-02-19 21:58:33.461288 django_machina-1.3.0/machina/locale/ro_RO/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16972 2023-02-19 21:58:13.809158 django_machina-1.3.0/machina/locale/ro_RO/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    34933 2023-02-19 21:58:33.496386 django_machina-1.3.0/machina/locale/ru/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    35738 2023-02-19 21:58:13.748867 django_machina-1.3.0/machina/locale/ru/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    15365 2023-02-19 21:58:33.429187 django_machina-1.3.0/machina/locale/sl_SI/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    22010 2023-02-19 21:58:13.779649 django_machina-1.3.0/machina/locale/sl_SI/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      443 2023-02-19 21:58:33.424502 django_machina-1.3.0/machina/locale/tr/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16787 2023-02-19 21:58:14.018710 django_machina-1.3.0/machina/locale/tr/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      472 2023-02-19 21:58:33.409057 django_machina-1.3.0/machina/locale/zh/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16725 2023-02-19 21:58:13.880043 django_machina-1.3.0/machina/locale/zh/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0    21955 2023-02-19 21:58:33.415694 django_machina-1.3.0/machina/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    23778 2023-02-19 21:58:13.846794 django_machina-1.3.0/machina/locale/zh_CN/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0      487 2023-02-19 21:58:33.409056 django_machina-1.3.0/machina/locale/zh_TW/LC_MESSAGES/django.mo
+-rw-r--r--   0        0        0    16740 2023-02-19 21:58:13.717238 django_machina-1.3.0/machina/locale/zh_TW/LC_MESSAGES/django.po
+-rw-r--r--   0        0        0       64 2021-12-11 21:41:38.753782 django_machina-1.3.0/machina/models/__init__.py
+-rw-r--r--   0        0        0      510 2021-12-11 21:41:38.753839 django_machina-1.3.0/machina/models/abstract_models.py
+-rw-r--r--   0        0        0    10513 2021-12-11 21:41:38.753940 django_machina-1.3.0/machina/models/fields.py
+-rw-r--r--   0        0        0      131 2021-12-11 21:41:38.754065 django_machina-1.3.0/machina/static/machina/build/README.rst
+-rw-r--r--   0        0        0    42739 2021-12-11 21:41:38.754470 django_machina-1.3.0/machina/static/machina/build/css/machina.admin_theme.min.css
+-rw-r--r--   0        0        0     4383 2021-12-11 21:41:38.754563 django_machina-1.3.0/machina/static/machina/build/css/machina.board_theme.min.css
+-rw-r--r--   0        0        0   181605 2021-12-11 21:41:38.754902 django_machina-1.3.0/machina/static/machina/build/css/machina.board_theme.vendor.min.css
+-rw-r--r--   0        0        0    11349 2021-12-11 21:41:38.755031 django_machina-1.3.0/machina/static/machina/build/css/vendor/easymde.min.css
+-rw-r--r--   0        0        0   111620 2021-12-11 21:41:38.755673 django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.eot
+-rw-r--r--   0        0        0   599658 2021-12-11 21:41:38.757507 django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.svg
+-rw-r--r--   0        0        0   111384 2021-12-11 21:41:38.758126 django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.ttf
+-rw-r--r--   0        0        0    71560 2021-12-11 21:41:38.758296 django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.woff
+-rw-r--r--   0        0        0    61336 2021-12-11 21:41:38.758394 django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.woff2
+-rw-r--r--   0        0        0    31272 2021-12-11 21:41:38.758569 django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.eot
+-rw-r--r--   0        0        0   104530 2021-12-11 21:41:38.758976 django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.svg
+-rw-r--r--   0        0        0    31044 2021-12-11 21:41:38.759164 django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.ttf
+-rw-r--r--   0        0        0    14724 2021-12-11 21:41:38.759273 django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.woff
+-rw-r--r--   0        0        0    12168 2021-12-11 21:41:38.759324 django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.woff2
+-rw-r--r--   0        0        0   133140 2021-12-11 21:41:38.759905 django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.eot
+-rw-r--r--   0        0        0   488219 2021-12-11 21:41:38.761393 django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.svg
+-rw-r--r--   0        0        0   132920 2021-12-11 21:41:38.762004 django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.ttf
+-rw-r--r--   0        0        0    63836 2021-12-11 21:41:38.762153 django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.woff
+-rw-r--r--   0        0        0    50388 2021-12-11 21:41:38.762292 django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.woff2
+-rw-r--r--   0        0        0      530 2021-12-11 21:41:38.762382 django_machina-1.3.0/machina/static/machina/build/js/machina.editor.min.js
+-rw-r--r--   0        0        0     1027 2021-12-11 21:41:38.762437 django_machina-1.3.0/machina/static/machina/build/js/machina.min.js
+-rw-r--r--   0        0        0   170131 2021-12-11 21:41:38.763525 django_machina-1.3.0/machina/static/machina/build/js/machina.packages.min.js
+-rw-r--r--   0        0        0   311129 2021-12-11 21:41:38.765215 django_machina-1.3.0/machina/static/machina/build/js/vendor/easymde.min.js
+-rw-r--r--   0        0        0      821 2021-12-11 21:41:38.765309 django_machina-1.3.0/machina/static/machina/js/editor.js
+-rw-r--r--   0        0        0     1911 2021-12-11 21:41:38.765369 django_machina-1.3.0/machina/static/machina/js/ui.js
+-rw-r--r--   0        0        0      437 2021-12-11 21:41:38.765472 django_machina-1.3.0/machina/static/machina/sass/admin_pages/forum_change_list.scss
+-rw-r--r--   0        0        0     1120 2021-12-11 21:41:38.765526 django_machina-1.3.0/machina/static/machina/sass/admin_pages/forum_permissions.scss
+-rw-r--r--   0        0        0      565 2021-12-11 21:41:38.765583 django_machina-1.3.0/machina/static/machina/sass/admin_theme.scss
+-rw-r--r--   0        0        0      761 2021-12-11 21:41:38.765668 django_machina-1.3.0/machina/static/machina/sass/board_pages/conversation_post_edit.scss
+-rw-r--r--   0        0        0      973 2021-12-11 21:41:38.765726 django_machina-1.3.0/machina/static/machina/sass/board_pages/conversation_topic_detail.scss
+-rw-r--r--   0        0        0      829 2021-12-11 21:41:38.765789 django_machina-1.3.0/machina/static/machina/sass/board_pages/forum_detail.scss
+-rw-r--r--   0        0        0      815 2021-12-11 21:41:38.765837 django_machina-1.3.0/machina/static/machina/sass/board_pages/forum_lists.scss
+-rw-r--r--   0        0        0      687 2021-12-11 21:41:38.765891 django_machina-1.3.0/machina/static/machina/sass/board_pages/member_profile.scss
+-rw-r--r--   0        0        0      584 2021-12-11 21:41:38.765958 django_machina-1.3.0/machina/static/machina/sass/board_pages/moderation.scss
+-rw-r--r--   0        0        0      578 2021-12-11 21:41:38.766015 django_machina-1.3.0/machina/static/machina/sass/board_pages/search.scss
+-rw-r--r--   0        0        0      439 2021-12-11 21:41:38.766078 django_machina-1.3.0/machina/static/machina/sass/board_theme.scss
+-rw-r--r--   0        0        0      434 2021-12-11 21:41:38.766131 django_machina-1.3.0/machina/static/machina/sass/board_theme.vendor.scss
+-rw-r--r--   0        0        0      759 2021-12-11 21:41:38.766190 django_machina-1.3.0/machina/static/machina/sass/variables.scss
+-rw-r--r--   0        0        0      259 2021-12-11 21:41:38.766375 django_machina-1.3.0/machina/templates/admin/forum/forum/change_form.html
+-rw-r--r--   0        0        0      913 2021-12-11 21:41:38.766455 django_machina-1.3.0/machina/templates/admin/forum/forum/change_list.html
+-rw-r--r--   0        0        0     3525 2021-12-11 21:41:38.766531 django_machina-1.3.0/machina/templates/admin/forum/forum/change_list_table.html
+-rw-r--r--   0        0        0      159 2021-12-11 21:41:38.766594 django_machina-1.3.0/machina/templates/admin/forum/forum/editpermissions_anonymous_user.html
+-rw-r--r--   0        0        0      174 2021-12-11 21:41:38.766654 django_machina-1.3.0/machina/templates/admin/forum/forum/editpermissions_authenticated_user.html
+-rw-r--r--   0        0        0     3344 2021-12-11 21:41:38.766746 django_machina-1.3.0/machina/templates/admin/forum/forum/editpermissions_form.html
+-rw-r--r--   0        0        0      160 2021-12-11 21:41:38.766828 django_machina-1.3.0/machina/templates/admin/forum/forum/editpermissions_group.html
+-rw-r--r--   0        0        0     6006 2021-12-11 21:41:38.766915 django_machina-1.3.0/machina/templates/admin/forum/forum/editpermissions_index.html
+-rw-r--r--   0        0        0      159 2021-12-11 21:41:38.766969 django_machina-1.3.0/machina/templates/admin/forum/forum/editpermissions_user.html
+-rw-r--r--   0        0        0     1190 2021-12-11 21:41:38.767078 django_machina-1.3.0/machina/templates/machina/_base.html
+-rw-r--r--   0        0        0     3262 2021-12-11 21:41:38.767141 django_machina-1.3.0/machina/templates/machina/board_base.html
+-rw-r--r--   0        0        0     2837 2021-12-11 21:41:38.767253 django_machina-1.3.0/machina/templates/machina/forum/forum_detail.html
+-rw-r--r--   0        0        0    10802 2021-12-11 21:41:38.767382 django_machina-1.3.0/machina/templates/machina/forum/forum_list.html
+-rw-r--r--   0        0        0     1012 2021-12-11 21:41:38.767593 django_machina-1.3.0/machina/templates/machina/forum/index.html
+-rw-r--r--   0        0        0     1593 2021-12-11 21:41:38.767738 django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_attachments/attachment_formset.html
+-rw-r--r--   0        0        0      809 2021-12-11 21:41:38.767804 django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_attachments/attachments_detail.html
+-rw-r--r--   0        0        0      622 2021-12-11 21:41:38.767869 django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_attachments/attachments_preview.html
+-rw-r--r--   0        0        0     2129 2021-12-11 21:41:38.767978 django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_detail.html
+-rw-r--r--   0        0        0     1013 2021-12-11 21:41:38.768051 django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_option_formset.html
+-rw-r--r--   0        0        0     2046 2021-12-11 21:41:38.768117 django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_preview.html
+-rw-r--r--   0        0        0      937 2022-10-13 18:52:02.266482 django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_results.html
+-rw-r--r--   0        0        0     1152 2021-12-11 21:41:38.768248 django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_vote_form.html
+-rw-r--r--   0        0        0     2170 2021-12-11 21:41:38.768380 django_machina-1.3.0/machina/templates/machina/forum_conversation/partials/post_form.html
+-rw-r--r--   0        0        0     4241 2021-12-11 21:41:38.768459 django_machina-1.3.0/machina/templates/machina/forum_conversation/partials/topic_detail_actions.html
+-rw-r--r--   0        0        0     4406 2022-10-13 18:52:02.266605 django_machina-1.3.0/machina/templates/machina/forum_conversation/partials/topic_form.html
+-rw-r--r--   0        0        0     3197 2021-12-11 21:41:38.768620 django_machina-1.3.0/machina/templates/machina/forum_conversation/post_create.html
+-rw-r--r--   0        0        0      956 2021-12-11 21:41:38.768709 django_machina-1.3.0/machina/templates/machina/forum_conversation/post_delete.html
+-rw-r--r--   0        0        0      648 2021-12-11 21:41:38.768772 django_machina-1.3.0/machina/templates/machina/forum_conversation/post_preview.html
+-rw-r--r--   0        0        0     1324 2021-12-11 21:41:38.768830 django_machina-1.3.0/machina/templates/machina/forum_conversation/post_update.html
+-rw-r--r--   0        0        0     1046 2021-12-11 21:41:38.768881 django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_create.html
+-rw-r--r--   0        0        0     5810 2021-12-11 21:41:38.768971 django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_detail.html
+-rw-r--r--   0        0        0     4424 2021-12-11 21:41:38.769046 django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_list.html
+-rw-r--r--   0        0        0      566 2021-12-11 21:41:38.769112 django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_pages_inline_list.html
+-rw-r--r--   0        0        0     1032 2021-12-11 21:41:38.769180 django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_update.html
+-rw-r--r--   0        0        0      321 2021-12-11 21:41:38.769276 django_machina-1.3.0/machina/templates/machina/forum_feeds/topics_description.html
+-rw-r--r--   0        0        0       42 2021-12-11 21:41:38.769331 django_machina-1.3.0/machina/templates/machina/forum_feeds/topics_title.html
+-rw-r--r--   0        0        0     3611 2021-12-11 21:41:38.769450 django_machina-1.3.0/machina/templates/machina/forum_member/forum_profile_detail.html
+-rw-r--r--   0        0        0     1992 2021-12-11 21:41:38.769505 django_machina-1.3.0/machina/templates/machina/forum_member/forum_profile_update.html
+-rw-r--r--   0        0        0     1259 2021-12-11 21:41:38.769571 django_machina-1.3.0/machina/templates/machina/forum_member/subscription_topic_list.html
+-rw-r--r--   0        0        0      970 2021-12-11 21:41:38.769632 django_machina-1.3.0/machina/templates/machina/forum_member/topic_subscribe.html
+-rw-r--r--   0        0        0      982 2021-12-11 21:41:38.769692 django_machina-1.3.0/machina/templates/machina/forum_member/topic_unsubscribe.html
+-rw-r--r--   0        0        0     3364 2021-12-11 21:41:38.769752 django_machina-1.3.0/machina/templates/machina/forum_member/user_posts_list.html
+-rw-r--r--   0        0        0     6990 2021-12-11 21:41:38.769919 django_machina-1.3.0/machina/templates/machina/forum_moderation/moderation_queue/detail.html
+-rw-r--r--   0        0        0     3720 2021-12-11 21:41:38.770003 django_machina-1.3.0/machina/templates/machina/forum_moderation/moderation_queue/list.html
+-rw-r--r--   0        0        0      918 2021-12-11 21:41:38.770059 django_machina-1.3.0/machina/templates/machina/forum_moderation/moderation_queue/post_approve.html
+-rw-r--r--   0        0        0      904 2021-12-11 21:41:38.770115 django_machina-1.3.0/machina/templates/machina/forum_moderation/moderation_queue/post_disapprove.html
+-rw-r--r--   0        0        0      960 2021-12-11 21:41:38.770170 django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_delete.html
+-rw-r--r--   0        0        0      952 2021-12-11 21:41:38.770227 django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_lock.html
+-rw-r--r--   0        0        0     1068 2021-12-11 21:41:38.770282 django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_move.html
+-rw-r--r--   0        0        0      960 2021-12-11 21:41:38.770367 django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_unlock.html
+-rw-r--r--   0        0        0      932 2021-12-11 21:41:38.770421 django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_update_type.html
+-rw-r--r--   0        0        0     1962 2022-01-16 23:11:03.535945 django_machina-1.3.0/machina/templates/machina/forum_search/pagination.html
+-rw-r--r--   0        0        0       51 2021-12-11 21:41:38.770559 django_machina-1.3.0/machina/templates/machina/forum_search/post_text.txt
+-rw-r--r--   0        0        0     4126 2021-12-11 21:41:38.770629 django_machina-1.3.0/machina/templates/machina/forum_search/search.html
+-rw-r--r--   0        0        0      888 2021-12-11 21:41:38.770716 django_machina-1.3.0/machina/templates/machina/forum_tracking/mark_forums_read.html
+-rw-r--r--   0        0        0      878 2021-12-11 21:41:38.770773 django_machina-1.3.0/machina/templates/machina/forum_tracking/mark_topics_read.html
+-rw-r--r--   0        0        0     1218 2021-12-11 21:41:38.770842 django_machina-1.3.0/machina/templates/machina/forum_tracking/unread_topic_list.html
+-rw-r--r--   0        0        0      271 2021-12-11 21:41:38.770941 django_machina-1.3.0/machina/templates/machina/partials/avatar.html
+-rw-r--r--   0        0        0      737 2021-12-11 21:41:38.771014 django_machina-1.3.0/machina/templates/machina/partials/breadcrumb.html
+-rw-r--r--   0        0        0      647 2021-12-11 21:41:38.771074 django_machina-1.3.0/machina/templates/machina/partials/form_field.html
+-rw-r--r--   0        0        0      329 2021-12-11 21:41:38.771138 django_machina-1.3.0/machina/templates/machina/partials/messages.html
+-rw-r--r--   0        0        0     1993 2021-12-11 21:41:38.771191 django_machina-1.3.0/machina/templates/machina/partials/pagination.html
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.771246 django_machina-1.3.0/machina/templatetags/__init__.py
+-rw-r--r--   0        0        0     1010 2021-12-11 21:41:38.771322 django_machina-1.3.0/machina/templatetags/forum_conversation_tags.py
+-rw-r--r--   0        0        0      261 2021-12-11 21:41:38.771378 django_machina-1.3.0/machina/templatetags/forum_markup_tags.py
+-rw-r--r--   0        0        0      448 2021-12-11 21:41:38.771431 django_machina-1.3.0/machina/templatetags/forum_member_tags.py
+-rw-r--r--   0        0        0     1120 2021-12-11 21:41:38.771494 django_machina-1.3.0/machina/templatetags/forum_permission_tags.py
+-rw-r--r--   0        0        0      938 2021-12-11 21:41:38.771547 django_machina-1.3.0/machina/templatetags/forum_polls_tags.py
+-rw-r--r--   0        0        0     2609 2021-12-11 21:41:38.771605 django_machina-1.3.0/machina/templatetags/forum_tags.py
+-rw-r--r--   0        0        0      574 2021-12-11 21:41:38.771658 django_machina-1.3.0/machina/templatetags/forum_tracking_tags.py
+-rw-r--r--   0        0        0        0 2021-12-11 21:41:38.771707 django_machina-1.3.0/machina/test/__init__.py
+-rw-r--r--   0        0        0      955 2021-12-11 21:41:38.771778 django_machina-1.3.0/machina/test/context_managers.py
+-rw-r--r--   0        0        0      248 2021-12-11 21:41:38.771868 django_machina-1.3.0/machina/test/factories/__init__.py
+-rw-r--r--   0        0        0      474 2021-12-11 21:41:38.771935 django_machina-1.3.0/machina/test/factories/attachments.py
+-rw-r--r--   0        0        0      879 2021-12-11 21:41:38.771992 django_machina-1.3.0/machina/test/factories/auth.py
+-rw-r--r--   0        0        0     1404 2023-05-28 00:44:13.048009 django_machina-1.3.0/machina/test/factories/conversation.py
+-rw-r--r--   0        0        0     1630 2021-12-11 21:41:38.772098 django_machina-1.3.0/machina/test/factories/forum.py
+-rw-r--r--   0        0        0      853 2021-12-11 21:41:38.772144 django_machina-1.3.0/machina/test/factories/permission.py
+-rw-r--r--   0        0        0     1023 2021-12-11 21:41:38.772189 django_machina-1.3.0/machina/test/factories/polls.py
+-rw-r--r--   0        0        0      782 2021-12-11 21:41:38.772239 django_machina-1.3.0/machina/test/factories/tracking.py
+-rw-r--r--   0        0        0      888 2021-12-11 21:41:38.772292 django_machina-1.3.0/machina/test/mixins.py
+-rw-r--r--   0        0        0     1420 2021-12-11 21:41:38.772357 django_machina-1.3.0/machina/test/testcases.py
+-rw-r--r--   0        0        0     1882 2022-04-24 02:08:26.857790 django_machina-1.3.0/machina/urls.py
+-rw-r--r--   0        0        0     1886 2023-05-28 01:07:31.317667 django_machina-1.3.0/pyproject.toml
+-rw-r--r--   0        0        0     3273 1970-01-01 00:00:00.000000 django_machina-1.3.0/PKG-INFO
```

### Comparing `django-machina-1.2.0/LICENSE` & `django_machina-1.3.0/LICENSE`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-Copyright (c) 2013-2022, Morgan Aubert and contributors.
+Copyright (c) 2013-2023, Morgan Aubert and contributors.
 All rights reserved.
 
 Redistribution and use in source and binary forms, with or without
 modification, are permitted provided that the following conditions are met:
 
  * Redistributions of source code must retain the above copyright notice, this
    list of conditions and the following disclaimer.
```

### Comparing `django-machina-1.2.0/README.rst` & `django_machina-1.3.0/README.rst`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+##############
 Django-machina
 ##############
 
 Django-machina is a forum framework for Django providing a way to build community-driven websites.
 It offers a full-featured yet very extensible forum solution:
 
 * Topic and post editing
```

### Comparing `django-machina-1.2.0/machina/__init__.py` & `django_machina-1.3.0/machina/__init__.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/abstract_models.py` & `django_machina-1.3.0/machina/apps/forum/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/admin.py` & `django_machina-1.3.0/machina/apps/forum/admin.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/apps.py` & `django_machina-1.3.0/machina/apps/forum/apps.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/forms.py` & `django_machina-1.3.0/machina/apps/forum/forms.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/migrations/0001_initial.py` & `django_machina-1.3.0/machina/apps/forum/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/migrations/0004_auto_20170504_2108.py` & `django_machina-1.3.0/machina/apps/forum/migrations/0004_auto_20170504_2108.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/migrations/0005_auto_20170504_2113.py` & `django_machina-1.3.0/machina/apps/forum/migrations/0005_auto_20170504_2113.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/migrations/0007_auto_20170523_2140.py` & `django_machina-1.3.0/machina/apps/forum/migrations/0007_auto_20170523_2140.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/migrations/0008_forum_last_post.py` & `django_machina-1.3.0/machina/apps/forum/migrations/0008_forum_last_post.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/migrations/0009_auto_20170928_2327.py` & `django_machina-1.3.0/machina/apps/forum/migrations/0009_auto_20170928_2327.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/migrations/0010_auto_20181103_1401.py` & `django_machina-1.3.0/machina/apps/forum/migrations/0010_auto_20181103_1401.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/migrations/0011_auto_20190627_2132.py` & `django_machina-1.3.0/machina/apps/forum/migrations/0011_auto_20190627_2132.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/receivers.py` & `django_machina-1.3.0/machina/apps/forum/receivers.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/urls.py` & `django_machina-1.3.0/machina/apps/forum/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/views.py` & `django_machina-1.3.0/machina/apps/forum/views.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum/visibility.py` & `django_machina-1.3.0/machina/apps/forum/visibility.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/abstract_models.py` & `django_machina-1.3.0/machina/apps/forum_conversation/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/admin.py` & `django_machina-1.3.0/machina/apps/forum_conversation/admin.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/apps.py` & `django_machina-1.3.0/machina/apps/forum_conversation/apps.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forms.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forms.py`

 * *Files 2% similar despite different names*

```diff
@@ -172,25 +172,30 @@
                 min_value=0, initial=0,
             )
             self.fields['poll_user_changes'] = forms.BooleanField(
                 label=_('Allow re-voting?'), required=False,
                 help_text=_('If enabled users are able to change their vote.'),
                 initial=False,
             )
-
+            self.fields['poll_hide_results'] = forms.BooleanField(
+                label=_('Hide results?'), required=False,
+                help_text=_('If enabled results are hidden to everyone except topic creator.'),
+                initial=False,
+            )
         # Set the initial values
         try:
             if hasattr(self.instance, 'topic'):
                 self.fields['topic_type'].initial = self.instance.topic.type
 
                 if self.can_create_polls and self.instance.topic.poll is not None:
                     self.fields['poll_question'].initial = self.instance.topic.poll.question
                     self.fields['poll_max_options'].initial = self.instance.topic.poll.max_options
                     self.fields['poll_duration'].initial = self.instance.topic.poll.duration
                     self.fields['poll_user_changes'].initial = self.instance.topic.poll.user_changes
+                    self.fields['poll_hide_results'].initial = self.instance.topic.poll.hide_results
         except ObjectDoesNotExist:
             pass
 
     def clean(self):
         """ Validates the form. """
         if self.cleaned_data.get('poll_question', None) \
                 and not self.cleaned_data.get('poll_max_options', None):
```

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/abstract_models.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/admin.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/admin.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/apps.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/apps.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/cache.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/cache.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/forms.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/forms.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/migrations/0001_initial.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/migrations/0002_auto_20181103_1404.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/migrations/0002_auto_20181103_1404.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/urls.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_attachments/views.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_attachments/views.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/abstract_models.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/abstract_models.py`

 * *Files 4% similar despite different names*

```diff
@@ -37,14 +37,17 @@
         verbose_name=_('Maximum number of poll options per user'),
         validators=validators.poll_max_options, default=1,
     )
 
     # Are users allowed to change their votes ?
     user_changes = models.BooleanField(verbose_name=_('Allow vote changes'), default=False)
 
+    # Hide results to everyone except topic creator ?
+    hide_results = models.BooleanField(verbose_name=_('Hide results'), default=False)
+
     class Meta:
         abstract = True
         app_label = 'forum_polls'
         ordering = ['-updated', ]
         get_latest_by = 'updated'
         verbose_name = _('Topic poll')
         verbose_name_plural = _('Topic polls')
```

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/admin.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/admin.py`

 * *Files 5% similar despite different names*

```diff
@@ -28,15 +28,15 @@
     search_fields = ('text',)
 
 
 class TopicPollAdmin(admin.ModelAdmin):
     """ The Topic Poll model admin. """
 
     inlines = (TopicPollOptionInline,)
-    list_display = ('topic', 'duration', 'max_options', 'user_changes',)
+    list_display = ('topic', 'duration', 'max_options', 'user_changes', 'hide_results')
     list_filter = ('created', 'updated',)
     search_fields = ('topic__subject',)
 
 
 class TopicPollVoteAdmin(admin.ModelAdmin):
     """ The Topic Poll Vote model admin. """
```

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/apps.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/apps.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/forms.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/forms.py`

 * *Files 7% similar despite different names*

```diff
@@ -77,22 +77,24 @@
             raise forms.ValidationError('At least two poll options must be defined.')
 
     def save(self, commit=True, **kwargs):
         poll_question = kwargs.pop('poll_question', None)
         poll_max_options = kwargs.pop('poll_max_options', None)
         poll_duration = kwargs.pop('poll_duration', None)
         poll_user_changes = kwargs.pop('poll_user_changes', False)
+        poll_hide_results = kwargs.pop('poll_hide_results', False)
 
         if self.poll is None:
             poll, _ = TopicPoll.objects.get_or_create(topic=self.topic)
 
             poll.question = poll_question
             poll.duration = poll_duration
             poll.max_options = poll_max_options
             poll.user_changes = poll_user_changes
+            poll.hide_results = poll_hide_results
             poll.save()
 
             for form in self.forms:
                 form.instance.poll = poll
         super().save(commit)
```

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/migrations/0001_initial.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/migrations/0002_auto_20151105_0029.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/migrations/0002_auto_20151105_0029.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/urls.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/forum_polls/views.py` & `django_machina-1.3.0/machina/apps/forum_conversation/forum_polls/views.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0001_initial.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0003_auto_20160228_2051.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0003_auto_20160228_2051.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0004_auto_20160427_0502.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0004_auto_20160427_0502.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0005_auto_20160607_0455.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0005_auto_20160607_0455.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0006_post_enable_signature.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0006_post_enable_signature.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0007_auto_20160903_0450.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0007_auto_20160903_0450.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0008_auto_20160903_0512.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0008_auto_20160903_0512.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0010_auto_20170120_0224.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0010_auto_20170120_0224.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0012_auto_20200423_1049.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0012_auto_20200423_1049.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/migrations/0013_auto_20201220_1745.py` & `django_machina-1.3.0/machina/apps/forum_conversation/migrations/0013_auto_20201220_1745.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/receivers.py` & `django_machina-1.3.0/machina/apps/forum_conversation/receivers.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/urls.py` & `django_machina-1.3.0/machina/apps/forum_conversation/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_conversation/views.py` & `django_machina-1.3.0/machina/apps/forum_conversation/views.py`

 * *Files 0% similar despite different names*

```diff
@@ -507,14 +507,15 @@
         if save_poll_option_formset:
             poll_option_formset.topic = self.forum_post.topic
             poll_option_formset.save(
                 poll_question=post_form.cleaned_data.pop('poll_question', None),
                 poll_max_options=post_form.cleaned_data.pop('poll_max_options', None),
                 poll_duration=post_form.cleaned_data.pop('poll_duration', None),
                 poll_user_changes=post_form.cleaned_data.pop('poll_user_changes', None),
+                poll_hide_results=post_form.cleaned_data.pop('poll_hide_results', None),
             )
 
         return valid
 
     def form_invalid(self, post_form, attachment_formset, poll_option_formset, **kwargs):
         """ Processes invalid forms. """
         poll_errors = [k for k in post_form.errors.keys() if k.startswith('poll_')]
```

### Comparing `django-machina-1.2.0/machina/apps/forum_feeds/feeds.py` & `django_machina-1.3.0/machina/apps/forum_feeds/feeds.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_feeds/urls.py` & `django_machina-1.3.0/machina/apps/forum_feeds/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/abstract_models.py` & `django_machina-1.3.0/machina/apps/forum_member/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/admin.py` & `django_machina-1.3.0/machina/apps/forum_member/admin.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/apps.py` & `django_machina-1.3.0/machina/apps/forum_member/apps.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/forms.py` & `django_machina-1.3.0/machina/apps/forum_member/forms.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/migrations/0001_initial.py` & `django_machina-1.3.0/machina/apps/forum_member/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/migrations/0002_auto_20160225_0515.py` & `django_machina-1.3.0/machina/apps/forum_member/migrations/0002_auto_20160225_0515.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/migrations/0003_auto_20160227_2122.py` & `django_machina-1.3.0/machina/apps/forum_member/migrations/0003_auto_20160227_2122.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/migrations/0004_auto_20181103_1406.py` & `django_machina-1.3.0/machina/apps/forum_member/migrations/0004_auto_20181103_1406.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/migrations/0005_auto_20200423_1049.py` & `django_machina-1.3.0/machina/apps/forum_member/migrations/0005_auto_20200423_1049.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/receivers.py` & `django_machina-1.3.0/machina/apps/forum_member/receivers.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/urls.py` & `django_machina-1.3.0/machina/apps/forum_member/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_member/views.py` & `django_machina-1.3.0/machina/apps/forum_member/views.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_moderation/apps.py` & `django_machina-1.3.0/machina/apps/forum_moderation/apps.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_moderation/forms.py` & `django_machina-1.3.0/machina/apps/forum_moderation/forms.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_moderation/urls.py` & `django_machina-1.3.0/machina/apps/forum_moderation/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_moderation/views.py` & `django_machina-1.3.0/machina/apps/forum_moderation/views.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/abstract_models.py` & `django_machina-1.3.0/machina/apps/forum_permission/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/admin.py` & `django_machina-1.3.0/machina/apps/forum_permission/admin.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/apps.py` & `django_machina-1.3.0/machina/apps/forum_permission/apps.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/checker.py` & `django_machina-1.3.0/machina/apps/forum_permission/checker.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/defaults.py` & `django_machina-1.3.0/machina/apps/forum_permission/defaults.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/handler.py` & `django_machina-1.3.0/machina/apps/forum_permission/handler.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/middleware.py` & `django_machina-1.3.0/machina/apps/forum_permission/middleware.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/migrations/0001_initial.py` & `django_machina-1.3.0/machina/apps/forum_permission/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/migrations/0002_auto_20160607_0500.py` & `django_machina-1.3.0/machina/apps/forum_permission/migrations/0002_auto_20160607_0500.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/models.py` & `django_machina-1.3.0/machina/apps/forum_permission/models.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/receivers.py` & `django_machina-1.3.0/machina/apps/forum_permission/receivers.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/shortcuts.py` & `django_machina-1.3.0/machina/apps/forum_permission/shortcuts.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_permission/viewmixins.py` & `django_machina-1.3.0/machina/apps/forum_permission/viewmixins.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_search/forms.py` & `django_machina-1.3.0/machina/apps/forum_search/forms.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_search/search_indexes.py` & `django_machina-1.3.0/machina/apps/forum_search/search_indexes.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_search/urls.py` & `django_machina-1.3.0/machina/apps/forum_search/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/abstract_models.py` & `django_machina-1.3.0/machina/apps/forum_tracking/abstract_models.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/admin.py` & `django_machina-1.3.0/machina/apps/forum_tracking/admin.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/apps.py` & `django_machina-1.3.0/machina/apps/forum_tracking/apps.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/handler.py` & `django_machina-1.3.0/machina/apps/forum_tracking/handler.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/managers.py` & `django_machina-1.3.0/machina/apps/forum_tracking/managers.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/migrations/0001_initial.py` & `django_machina-1.3.0/machina/apps/forum_tracking/migrations/0001_initial.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/migrations/0002_auto_20160607_0502.py` & `django_machina-1.3.0/machina/apps/forum_tracking/migrations/0002_auto_20160607_0502.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/receivers.py` & `django_machina-1.3.0/machina/apps/forum_tracking/receivers.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/urls.py` & `django_machina-1.3.0/machina/apps/forum_tracking/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/apps/forum_tracking/views.py` & `django_machina-1.3.0/machina/apps/forum_tracking/views.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/conf/settings.py` & `django_machina-1.3.0/machina/conf/settings.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/core/compat.py` & `django_machina-1.3.0/machina/core/compat.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/core/db/models.py` & `django_machina-1.3.0/machina/core/db/models.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/core/loading.py` & `django_machina-1.3.0/machina/core/loading.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,8 +102,11 @@
     """ Given a module label, loop over the apps specified in the INSTALLED_APPS to find the
         corresponding application module path.
     """
     app_name = module_label.rsplit('.', 1)[0]
     for app in settings.INSTALLED_APPS:
         if app.endswith('.' + app_name) or app == app_name:
             return app
+        path = app.split('.')
+        if len(path) >= 3 and path[-2] == 'apps' and path[-3] == app_name:
+            return app
     return None
```

### Comparing `django-machina-1.2.0/machina/core/urls.py` & `django_machina-1.3.0/machina/core/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/core/validators.py` & `django_machina-1.3.0/machina/core/validators.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/forms/widgets.py` & `django_machina-1.3.0/machina/forms/widgets.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/ar/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/ar/LC_MESSAGES/django.mo`

 * *Files 5% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2020-04-26 17:48+0000\n"
 "Last-Translator: Brahim Bouslim <bouslim007@gmail.com>\n"
 "Language-Team: Arabic (http://www.transifex.com/django-machina-team/django-"
 "machina/language/ar/)\n"
+"Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 "
 "&& n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Category forum"
 msgstr "فئة المنتدى"
```

### Comparing `django-machina-1.2.0/machina/locale/ar/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/ar/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Brahim Bouslim <bouslim007@gmail.com>, 2020
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2020-04-26 17:48+0000\n"
 "Last-Translator: Brahim Bouslim <bouslim007@gmail.com>\n"
 "Language-Team: Arabic (http://www.transifex.com/django-machina-team/django-machina/language/ar/)\n"
+"Language: ar\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ar\n"
 "Plural-Forms: nplurals=6; plural=n==0 ? 0 : n==1 ? 1 : n==2 ? 2 : n%100>=3 && n%100<=10 ? 3 : n%100>=11 && n%100<=99 ? 4 : 5;\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
 msgstr "الأب"
 
 msgid "Name"
@@ -66,16 +66,15 @@
 
 msgid "Last post added on"
 msgstr "أضيفت آخر مشاركة في"
 
 msgid "Display in parent-forums legend"
 msgstr "العرض في العنوان التفسيري للمنتديات الأب"
 
-msgid ""
-"Displays this forum on the legend of its parent-forum (sub forums list)"
+msgid "Displays this forum on the legend of its parent-forum (sub forums list)"
 msgstr "يعرض هذا المنتدى على العنوان التفسيرى للمنتدى الأب(قائمة المنتديات الفرعية)"
 
 msgid "Forum"
 msgstr "منتدى"
 
 msgid "Forums"
 msgstr "المنتديات"
@@ -124,30 +123,24 @@
 
 msgid "Machina: Forum"
 msgstr ""
 
 msgid "Anonymous"
 msgstr ""
 
-msgid ""
-"Please select this option if you want to edit the permissions of the "
-"anonymous user"
+msgid "Please select this option if you want to edit the permissions of the anonymous user"
 msgstr ""
 
 msgid "Authenticated"
 msgstr ""
 
-msgid ""
-"Please select this option if you want to edit the permissions of every (non-"
-"specific) logged in user"
+msgid "Please select this option if you want to edit the permissions of every (non-specific) logged in user"
 msgstr ""
 
-msgid ""
-"Choose either a user ID or check either the anonymous or authenticated user "
-"checkbox"
+msgid "Choose either a user ID or check either the anonymous or authenticated user checkbox"
 msgstr ""
 
 msgid "Not set"
 msgstr ""
 
 msgid "Granted"
 msgstr ""
@@ -199,14 +192,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr ""
 
+msgid "Creation date"
+msgstr ""
+
+msgid "Update date"
+msgstr ""
+
 msgid "Topic"
 msgstr ""
 
 msgid "Topics"
 msgstr ""
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -238,16 +237,15 @@
 
 msgid "Posts"
 msgstr ""
 
 msgid "A user id or an anonymous key must be associated with a post."
 msgstr ""
 
-msgid ""
-"A user id or an anonymous key must be associated with a post, but not both."
+msgid "A user id or an anonymous key must be associated with a post, but not both."
 msgstr ""
 
 msgid "A username must be specified if the poster is anonymous"
 msgstr ""
 
 msgid "Machina: Forum conversations"
 msgstr ""
@@ -266,17 +264,15 @@
 
 msgid "Post topic as"
 msgstr ""
 
 msgid "Poll question"
 msgstr ""
 
-msgid ""
-"Enter a question to associate a poll with the topic or leave blank to not "
-"create a poll."
+msgid "Enter a question to associate a poll with the topic or leave blank to not create a poll."
 msgstr ""
 
 msgid "Maximum number of poll options per user"
 msgstr ""
 
 msgid "This is the number of options each user may select when voting."
 msgstr ""
@@ -289,16 +285,21 @@
 
 msgid "Allow re-voting?"
 msgstr ""
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
-msgid ""
-"You must set the maximum number of poll options per user when creating polls"
+msgid "Hide results?"
+msgstr ""
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
+msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr ""
 
 msgid "Comment"
 msgstr ""
@@ -314,14 +315,17 @@
 
 msgid "Poll duration, in days"
 msgstr ""
 
 msgid "Allow vote changes"
 msgstr ""
 
+msgid "Hide results"
+msgstr ""
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -482,17 +486,15 @@
 
 msgid "User forum permission"
 msgstr ""
 
 msgid "User forum permissions"
 msgstr ""
 
-msgid ""
-"A permission should target either a specific user, an anonymous user or any "
-"authenticated user"
+msgid "A permission should target either a specific user, an anonymous user or any authenticated user"
 msgstr ""
 
 msgid "Group"
 msgstr ""
 
 msgid "Group forum permission"
 msgstr ""
@@ -607,40 +609,36 @@
 
 msgid "Topics have been marked read."
 msgstr ""
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
 msgstr ""
 
-msgid "Update date"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
 
 msgid "MACHINA_MARKUP_LANGUAGE setting is required"
 msgstr ""
 
 msgid "Files of size greater than {} are not allowed. Your file is {}"
 msgstr ""
 
-msgid ""
-"Images of width lesser than {}px or greater than {}px or are not allowed. "
-"The width of your image is {}px"
+msgid "Images of width lesser than {}px or greater than {}px or are not allowed. The width of your image is {}px"
 msgstr ""
 
-msgid ""
-"Images of height lesser than {}px or greater than {}px or are not allowed. "
-"The height of your image is {}px"
+msgid "Images of height lesser than {}px or greater than {}px or are not allowed. The height of your image is {}px"
 msgstr ""
 
 msgid "List of forums"
 msgstr ""
 
 msgid "Quick actions"
 msgstr ""
@@ -704,17 +702,15 @@
 
 msgid "Please select a group in order to update its permissions"
 msgstr ""
 
 msgid "Copy permissions from another forum"
 msgstr ""
 
-msgid ""
-"Please select a forum in order to copy its permissions configuration to the "
-"current forum"
+msgid "Please select a forum in order to copy its permissions configuration to the current forum"
 msgstr ""
 
 msgid "Copy"
 msgstr ""
 
 msgid "Search"
 msgstr ""
@@ -805,22 +801,23 @@
 
 msgid "Poll options"
 msgstr ""
 
 msgid "Add a poll option"
 msgstr ""
 
-msgid ""
-"<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the "
-"associated votes."
+msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr ""
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr ""
 
 msgid "Submit"
 msgstr ""
 
 msgid "View results"
@@ -1058,16 +1055,15 @@
 
 msgid "Are you sure you want to approve this post?"
 msgstr ""
 
 msgid "Disapprove post"
 msgstr ""
 
-msgid ""
-"Are you sure you want to disapprove this post? This post will be deleted."
+msgid "Are you sure you want to disapprove this post? This post will be deleted."
 msgstr ""
 
 msgid "Are you sure you want to delete this topic?"
 msgstr ""
 
 msgid "Are you sure you want to lock this topic?"
 msgstr ""
```

### Comparing `django-machina-1.2.0/machina/locale/ca/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/el/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2016-02-23 03:25+0000\n"
 "Last-Translator: \n"
-"Language-Team: Catalan (http://www.transifex.com/django-machina-team/django-machina/language/ca/)\n"
-"Language: ca\n"
+"Language-Team: Greek (http://www.transifex.com/django-machina-team/django-machina/language/el/)\n"
+"Language: el\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
@@ -191,14 +191,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr ""
 
+msgid "Creation date"
+msgstr ""
+
+msgid "Update date"
+msgstr ""
+
 msgid "Topic"
 msgstr ""
 
 msgid "Topics"
 msgstr ""
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -278,14 +284,20 @@
 
 msgid "Allow re-voting?"
 msgstr ""
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
+msgid "Hide results?"
+msgstr ""
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr ""
 
 msgid "Comment"
@@ -302,14 +314,17 @@
 
 msgid "Poll duration, in days"
 msgstr ""
 
 msgid "Allow vote changes"
 msgstr ""
 
+msgid "Hide results"
+msgstr ""
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -593,18 +608,18 @@
 
 msgid "Topics have been marked read."
 msgstr ""
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
 msgstr ""
 
-msgid "Update date"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
@@ -791,14 +806,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr ""
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr ""
 
 msgid "Submit"
 msgstr ""
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/de/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/de/LC_MESSAGES/django.mo`

 * *Files 1% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2020-04-02 17:18+0000\n"
 "Last-Translator: m.g <markus.gellrich@gmx.net>\n"
 "Language-Team: German (http://www.transifex.com/django-machina-team/django-"
 "machina/language/de/)\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "%(counter)s post found"
 msgid_plural "%(counter)s posts found"
 msgstr[0] "%(counter)s Beitrag gefunden"
 msgstr[1] "%(counter)s Beiträge gefunden"
```

### Comparing `django-machina-1.2.0/machina/locale/de/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/de/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Marcel Lambert <marcel.lambert@wesualize.com>, 2017
 # m.g <markus.gellrich@gmx.net>, 2020
 # Robert Gutschale <r.gutschale@blueshoe.de>, 2018
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2020-04-02 17:18+0000\n"
 "Last-Translator: m.g <markus.gellrich@gmx.net>\n"
 "Language-Team: German (http://www.transifex.com/django-machina-team/django-machina/language/de/)\n"
+"Language: de\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: de\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
 msgstr "Übergeordnetes Forum"
 
 msgid "Name"
@@ -68,16 +68,15 @@
 
 msgid "Last post added on"
 msgstr "Letzter Beitrag hinzugefügt am"
 
 msgid "Display in parent-forums legend"
 msgstr "In Legende des übergeordneten Forum anzeigen"
 
-msgid ""
-"Displays this forum on the legend of its parent-forum (sub forums list)"
+msgid "Displays this forum on the legend of its parent-forum (sub forums list)"
 msgstr "Zeigt dieses Forum in der Legende seines übergeordneten Forums an (Subforen-Liste)"
 
 msgid "Forum"
 msgstr "Forum"
 
 msgid "Forums"
 msgstr "Foren"
@@ -126,30 +125,24 @@
 
 msgid "Machina: Forum"
 msgstr ""
 
 msgid "Anonymous"
 msgstr "Anonym"
 
-msgid ""
-"Please select this option if you want to edit the permissions of the "
-"anonymous user"
+msgid "Please select this option if you want to edit the permissions of the anonymous user"
 msgstr "Bitte wähle diese Option, um die Berechtigungen anonymer Nutzer zu bearbeiten"
 
 msgid "Authenticated"
 msgstr ""
 
-msgid ""
-"Please select this option if you want to edit the permissions of every (non-"
-"specific) logged in user"
+msgid "Please select this option if you want to edit the permissions of every (non-specific) logged in user"
 msgstr ""
 
-msgid ""
-"Choose either a user ID or check either the anonymous or authenticated user "
-"checkbox"
+msgid "Choose either a user ID or check either the anonymous or authenticated user checkbox"
 msgstr ""
 
 msgid "Not set"
 msgstr "Nicht festgelegt"
 
 msgid "Granted"
 msgstr "Gestattet"
@@ -201,14 +194,20 @@
 
 msgid "First post"
 msgstr "Erster Beitrag"
 
 msgid "Subscribers"
 msgstr "Abonnenten"
 
+msgid "Creation date"
+msgstr "Erstellungsdatum"
+
+msgid "Update date"
+msgstr "Aktualisierungsdatum"
+
 msgid "Topic"
 msgstr "Thema"
 
 msgid "Topics"
 msgstr "Themen"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -240,16 +239,15 @@
 
 msgid "Posts"
 msgstr "Beiträge"
 
 msgid "A user id or an anonymous key must be associated with a post."
 msgstr ""
 
-msgid ""
-"A user id or an anonymous key must be associated with a post, but not both."
+msgid "A user id or an anonymous key must be associated with a post, but not both."
 msgstr ""
 
 msgid "A username must be specified if the poster is anonymous"
 msgstr ""
 
 msgid "Machina: Forum conversations"
 msgstr ""
@@ -268,17 +266,15 @@
 
 msgid "Post topic as"
 msgstr "Thema veröffentlichen als"
 
 msgid "Poll question"
 msgstr "Abstimmungsfrage"
 
-msgid ""
-"Enter a question to associate a poll with the topic or leave blank to not "
-"create a poll."
+msgid "Enter a question to associate a poll with the topic or leave blank to not create a poll."
 msgstr "Hier kannst du eine Frage zu deiner Abstimmung eingeben."
 
 msgid "Maximum number of poll options per user"
 msgstr "Maximale Stimmenzahl pro Nutzer"
 
 msgid "This is the number of options each user may select when voting."
 msgstr "Dies ist die Anzahl der Optionen, die ein Nutzer bei der Abstimmung auswählen kann."
@@ -291,16 +287,23 @@
 
 msgid "Allow re-voting?"
 msgstr "Ändern der Abstimmung erlauben?"
 
 msgid "If enabled users are able to change their vote."
 msgstr "Ist diese Option ausgewählt, können Nutzer ihre Abstimmung nachträglich ändern"
 
-msgid ""
-"You must set the maximum number of poll options per user when creating polls"
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Ergebnisse ansehen"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
+msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "Es muss eine maximale Stimmenzahl pro Nutzer angegeben werden"
 
 msgid "File"
 msgstr "Datei"
 
 msgid "Comment"
 msgstr "Kommentar"
@@ -316,14 +319,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Umfragedauer, in Tagen"
 
 msgid "Allow vote changes"
 msgstr "Änderung der Abstimmung erlauben"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Ergebnisse ansehen"
+
 msgid "Topic poll"
 msgstr "Umfrage"
 
 msgid "Topic polls"
 msgstr "Umfragen"
 
 msgid "Poll"
@@ -484,17 +492,15 @@
 
 msgid "User forum permission"
 msgstr ""
 
 msgid "User forum permissions"
 msgstr ""
 
-msgid ""
-"A permission should target either a specific user, an anonymous user or any "
-"authenticated user"
+msgid "A permission should target either a specific user, an anonymous user or any authenticated user"
 msgstr ""
 
 msgid "Group"
 msgstr "Gruppe"
 
 msgid "Group forum permission"
 msgstr "Gruppenbefugniss"
@@ -609,40 +615,36 @@
 
 msgid "Topics have been marked read."
 msgstr "Themen wurden als gelesen markiert."
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Weder Pillow noch PIL konnten importiert werden: {}"
 
-msgid "Creation date"
-msgstr "Erstellungsdatum"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr ""
 
-msgid "Update date"
-msgstr "Aktualisierungsdatum"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
 
 msgid "MACHINA_MARKUP_LANGUAGE setting is required"
 msgstr ""
 
 msgid "Files of size greater than {} are not allowed. Your file is {}"
 msgstr "Dateien mit mehr als {} sind nicht zulässig. Datei ist {} groß."
 
-msgid ""
-"Images of width lesser than {}px or greater than {}px or are not allowed. "
-"The width of your image is {}px"
+msgid "Images of width lesser than {}px or greater than {}px or are not allowed. The width of your image is {}px"
 msgstr "Bilder mit einer Breite von weniger als {}px oder mehr als {}px sind nicht zulässig. Dein Bild hat eine Breite von {}px."
 
-msgid ""
-"Images of height lesser than {}px or greater than {}px or are not allowed. "
-"The height of your image is {}px"
+msgid "Images of height lesser than {}px or greater than {}px or are not allowed. The height of your image is {}px"
 msgstr "Bilder mit einer Höhe von weniger als {}px oder mehr als {}px sind nicht zulässig. Dein Bild hat eine Höhe von {}px."
 
 msgid "List of forums"
 msgstr "Forenliste"
 
 msgid "Quick actions"
 msgstr "Schnellzugriff"
@@ -706,17 +708,15 @@
 
 msgid "Please select a group in order to update its permissions"
 msgstr "Bitte eine Gruppe auswählen für die die Berechtigungen geändert werden sollen"
 
 msgid "Copy permissions from another forum"
 msgstr "Berechtigungen eines anderen Forums übernehmen"
 
-msgid ""
-"Please select a forum in order to copy its permissions configuration to the "
-"current forum"
+msgid "Please select a forum in order to copy its permissions configuration to the current forum"
 msgstr "Bitte ein Forum auswählen um dessen Berechtigungseinstellungen für das aktuelle Forum zu übernehmen"
 
 msgid "Copy"
 msgstr "Kopieren"
 
 msgid "Search"
 msgstr "Suche"
@@ -807,22 +807,23 @@
 
 msgid "Poll options"
 msgstr "Abstimmungsoptionen"
 
 msgid "Add a poll option"
 msgstr "Abstimmungsoption hinzufügen"
 
-msgid ""
-"<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the "
-"associated votes."
+msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "<b>Hinweis:</b>&nbsp;Beim Löschen von Abstimmungsoptionen in bestehenden Umfragen werden die zugehörigen Stimmen gelöscht."
 
 msgid "Preview:"
 msgstr "Vorschau:"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Stimmen gesamt:"
 
 msgid "Submit"
 msgstr "Absenden"
 
 msgid "View results"
@@ -1040,16 +1041,15 @@
 
 msgid "Are you sure you want to approve this post?"
 msgstr "Bist du sicher, dass du diesen Beitrag zulassen möchtest?"
 
 msgid "Disapprove post"
 msgstr "Beitrag ablehnen"
 
-msgid ""
-"Are you sure you want to disapprove this post? This post will be deleted."
+msgid "Are you sure you want to disapprove this post? This post will be deleted."
 msgstr "Bist du sicher, dass du diesen Beitrag ablehnen möchtest? Der Beitrag wird damit gelöscht."
 
 msgid "Are you sure you want to delete this topic?"
 msgstr "Bist du sicher, dass du das Thema löschen möchtest?"
 
 msgid "Are you sure you want to lock this topic?"
 msgstr "Bist du sicher, dass du das Thema schließen möchtest?"
```

### Comparing `django-machina-1.2.0/machina/locale/en/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/tr/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# FIRST AUTHOR <EMAIL@ADDRESS>, YEAR.
 #
+# Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
-"PO-Revision-Date: 2016-02-22 22:24-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
+"PO-Revision-Date: 2016-02-23 03:25+0000\n"
 "Last-Translator: \n"
-"Language-Team: \n"
-"Language: en\n"
+"Language-Team: Turkish (http://www.transifex.com/django-machina-team/django-machina/language/tr/)\n"
+"Language: tr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
 msgstr ""
 
 msgid "Name"
 msgstr ""
@@ -191,14 +191,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr ""
 
+msgid "Creation date"
+msgstr ""
+
+msgid "Update date"
+msgstr ""
+
 msgid "Topic"
 msgstr ""
 
 msgid "Topics"
 msgstr ""
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -278,14 +284,20 @@
 
 msgid "Allow re-voting?"
 msgstr ""
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
+msgid "Hide results?"
+msgstr ""
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr ""
 
 msgid "Comment"
@@ -302,14 +314,17 @@
 
 msgid "Poll duration, in days"
 msgstr ""
 
 msgid "Allow vote changes"
 msgstr ""
 
+msgid "Hide results"
+msgstr ""
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -593,18 +608,18 @@
 
 msgid "Topics have been marked read."
 msgstr ""
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
 msgstr ""
 
-msgid "Update date"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
@@ -791,14 +806,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr ""
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr ""
 
 msgid "Submit"
 msgstr ""
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/es/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/es/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/es/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/es/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Translators:
 # Davinia MC, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: Spanish (http://www.transifex.com/django-machina-team/django-machina/language/es/)\n"
 "Language: es\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -192,14 +192,20 @@
 
 msgid "First post"
 msgstr "Primer mensaje"
 
 msgid "Subscribers"
 msgstr "Suscriptores"
 
+msgid "Creation date"
+msgstr "Fecha de creación"
+
+msgid "Update date"
+msgstr "Fecha de actualización"
+
 msgid "Topic"
 msgstr "Hilo"
 
 msgid "Topics"
 msgstr "Hilos"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -279,14 +285,22 @@
 
 msgid "Allow re-voting?"
 msgstr "¿Permitir volver a votar?"
 
 msgid "If enabled users are able to change their vote."
 msgstr "Si está activo, los usuarios pueden cambiar su voto."
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Ver resultados"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "Debes seleccionar el número máximo de opciones por usuario cuando creas una encuesta"
 
 msgid "File"
 msgstr "Fichero"
 
 msgid "Comment"
@@ -303,14 +317,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Duración de la encuesta, en días"
 
 msgid "Allow vote changes"
 msgstr "Permitir cambiar el voto"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Ver resultados"
+
 msgid "Topic poll"
 msgstr "Encuesta sobre el hilo"
 
 msgid "Topic polls"
 msgstr "Encuesta sobre los hilos"
 
 msgid "Poll"
@@ -594,19 +613,23 @@
 
 msgid "Topics have been marked read."
 msgstr "Los hilos se han marcado como leídos."
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "No se puede importar ni Pillow ni PIL: {}"
 
-msgid "Creation date"
-msgstr "Fecha de creación"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "No se puede importar MACHINA_MARKUP_LANGUAGE {}: {}"
 
-msgid "Update date"
-msgstr "Fecha de actualización"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "Se requiere el parámetro MACHINA_MARKUP_LANGUAGE"
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "No se puede importar MACHINA_MARKUP_WIDGET {}: {}"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "No se puede importar MACHINA_MARKUP_LANGUAGE {}: {}"
 
@@ -792,14 +815,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "Nota:</b>&nbsp;Borrar las opciones de una encuestra existente borrará los votos asociados."
 
 msgid "Preview:"
 msgstr "Previsualización:"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Votos totales:"
 
 msgid "Submit"
 msgstr "Enviar"
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/fr/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/fr/LC_MESSAGES/django.mo`

 * *Files 4% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,31 +1,31 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"PO-Revision-Date: 2020-04-26 20:18+0000\n"
-"Last-Translator: Tutur L <arthur.lerou@gmail.com>\n"
+"PO-Revision-Date: 2021-06-21 20:18+0000\n"
+"Last-Translator: Gaget L <lauri.gaget@opencop.fr>\n"
 "Language-Team: French (http://www.transifex.com/django-machina-team/django-"
 "machina/language/fr/)\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "%(counter)s post found"
 msgid_plural "%(counter)s posts found"
-msgstr[0] "%(counter)s post trouvé"
-msgstr[1] "%(counter)s posts trouvés"
+msgstr[0] "%(counter)s message trouvé"
+msgstr[1] "%(counter)s messages trouvés"
 
 msgid "%(counter)s topic found"
 msgid_plural "%(counter)s topics found"
-msgstr[0] "%(counter)s thème trouvé"
-msgstr[1] "%(counter)s thèmes trouvés"
+msgstr[0] "%(counter)s sujet trouvé"
+msgstr[1] "%(counter)s sujets trouvés"
 
 msgid "%(topic_length)s posts found"
 msgstr "%(topic_length)s posts trouvés"
 
 msgid "%(username)s profile"
 msgstr "Profile de %(username)s"
 
@@ -68,24 +68,24 @@
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Topics</small></p>"
 msgstr[0] ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "<p><small>Sujet</small></p>"
 msgstr[1] ""
 "<h2><strong>%(counter)s</strong></h2>\n"
-"<p class=\"mb-1\"><small>Sujets</small></p>"
+"<p class=\"mb-1\"><small>sujet</small></p>"
 
 msgid "A category can not have another category as parent"
-msgstr " Une catégorie ne peut pas avoir une autre catégorie comme parent"
+msgstr "Une catégorie ne peut pas avoir une autre catégorie comme parent"
 
 msgid "A forum can not have a link forum as parent"
-msgstr " Un forum ne peut pas avoir un lien comme parent"
+msgstr "Un forum ne peut pas avoir un lien comme parent"
 
 msgid "A link forum must have a link associated with it"
-msgstr " Un forum lien doit être associé à une URL"
+msgstr "Un forum lien doit être associé à une URL"
 
 msgid ""
 "A permission should target either a specific user, an anonymous user or any "
 "authenticated user"
 msgstr ""
 "Une permission devrait cibler soit un utilisateur spécifique, un utilisateur "
 "anonyme ou n’importe quel utilisateur authentifié"
@@ -148,44 +148,45 @@
 msgid "Anonymous user forum key"
 msgstr "Clé de l'utilisateur anonyme"
 
 msgid "Approve"
 msgstr "Approuver"
 
 msgid "Approve post"
-msgstr "Approuver le post"
+msgstr "Approuver le message"
 
 msgid "Approved"
 msgstr "Approuvé"
 
 msgid "Are you sure you want to approve this post?"
-msgstr "Êtes-vous sûr de vouloir approuver ce post ?"
+msgstr "Êtes-vous sûr de vouloir approuver ce message ?"
 
 msgid "Are you sure you want to delete this post?"
-msgstr "Êtes-vous sûr de vouloir supprimer ce post ?"
+msgstr "Êtes-vous sûr de vouloir supprimer ce message ?"
 
 msgid "Are you sure you want to delete this topic?"
-msgstr "Êtes-vous sûr de vouloir supprimer ce thème ?"
+msgstr "Êtes-vous sûr de vouloir supprimer ce sujet ?"
 
 msgid ""
 "Are you sure you want to disapprove this post? This post will be deleted."
 msgstr ""
-"Êtes-vous sûr de vouloir désapprouver ce post ? Celui-ci sera donc supprimé."
+"Êtes-vous sûr de vouloir désapprouver ce message ? Celui-ci sera donc "
+"supprimé."
 
 msgid "Are you sure you want to lock this topic?"
-msgstr "Êtes-vous sûr de vouloir verrouiller ce thème ?"
+msgstr "Êtes-vous sûr de vouloir verrouiller ce sujet ?"
 
 msgid "Are you sure you want to mark forums read?"
 msgstr "Êtes-vous sûr de vouloir marquer ces forums comme 'lu' ?"
 
 msgid "Are you sure you want to mark topics read?"
-msgstr "Êtes-vous sûr de vouloir marquer ces thèmes comme 'lu' ?"
+msgstr "Êtes-vous sûr de vouloir marquer ces sujets comme 'lu' ?"
 
 msgid "Are you sure you want to unlock this topic?"
-msgstr "Êtes-vous certain de vouloir déverouiller ce thème ?"
+msgstr "Êtes-vous certain de vouloir déverrouiller ce sujet ?"
 
 msgid "Attach a signature"
 msgstr "Attacher une signature"
 
 msgid "Attachment"
 msgstr "Pièce jointe"
 
@@ -198,21 +199,21 @@
 msgid "Authenticated user"
 msgstr "Utilisateur authentifié"
 
 msgid "Avatar"
 msgstr "Avatar"
 
 msgid "By: %(poster_username)s"
-msgstr "By: %(poster_username)s"
+msgstr "Par : %(poster_username)s"
 
 msgid "By: %(poster_username)s on %(creation_date)s"
 msgstr "Par : %(poster_username)s le %(creation_date)s"
 
 msgid "By: <a href=\"%(poster_url)s\">%(username)s</a>"
-msgstr "By: <a href=\"%(poster_url)s\">%(username)s</a>"
+msgstr "Par: <a href=\"%(poster_url)s\">%(username)s</a>"
 
 msgid "By: <a href=\"%(poster_url)s\">%(username)s</a> on %(creation_date)s"
 msgstr "Par: <a href=\"%(poster_url)s\">%(username)s</a> le %(creation_date)s"
 
 msgid "Can add posts in locked topics"
 msgstr "Peut ajouter des publications dans des sujets verrouillés"
 
@@ -234,27 +235,27 @@
 msgid "Can download file"
 msgstr "Peut télécharger le fichier"
 
 msgid "Can edit own posts"
 msgstr "Peut éditer ses propres messages"
 
 msgid "Can edit posts"
-msgstr "Peut éditer des posts"
+msgstr "Peut éditer des messages"
 
 msgid "Can lock topics"
 msgstr "Peut verrouiller les sujets"
 
 msgid "Can move topics"
 msgstr "Peut déplacer des sujets"
 
 msgid "Can post announcements"
 msgstr "Peut poster des annonces"
 
 msgid "Can post stickies"
-msgstr "Peut poster des stickies"
+msgstr "Peut poster des sujets épinglé"
 
 msgid "Can post without approval"
 msgstr "Peut poster sans approbation"
 
 msgid "Can read forum"
 msgstr "Peut lire le forum"
 
@@ -273,21 +274,21 @@
 msgid "Category forum"
 msgstr "Catégorie"
 
 msgid "Change to announce"
 msgstr "Changer en annonce"
 
 msgid "Change to standard topic"
-msgstr "Changer en un thème standard"
+msgstr "Changer en un sujet standard"
 
 msgid "Change to sticky topic"
-msgstr "Mettre le thème toujours en haut"
+msgstr "Épingler ce sujet"
 
 msgid "Change topic type"
-msgstr "Changer le type du thème"
+msgstr "Changer le type du sujet"
 
 msgid "Change your vote"
 msgstr "Changer votre vote"
 
 msgid "Choose a group ID"
 msgstr "Choisir un ID de groupe"
 
@@ -330,18 +331,18 @@
 msgid "Default topic"
 msgstr "Sujet par défaut"
 
 msgid "Delete"
 msgstr "Supprimer"
 
 msgid "Delete post"
-msgstr "Supprimer le post"
+msgstr "Supprimer le message"
 
 msgid "Delete topic"
-msgstr "Supprimer le thème"
+msgstr "Supprimer le sujet"
 
 msgid "Description"
 msgstr "Description"
 
 msgid "Details"
 msgstr "Détails"
 
@@ -351,18 +352,18 @@
 msgid "Direct number of topics"
 msgstr "Nombre direct de sujets"
 
 msgid "Disapprove"
 msgstr "Désapprouver"
 
 msgid "Disapprove post"
-msgstr "Désapprouver ce post"
+msgstr "Désapprouver ce message"
 
 msgid "Display in parent-forums legend"
-msgstr " Affichage dans la légende des forums-parents"
+msgstr "Affichage dans la légende des forums-parents"
 
 msgid "Displays this forum on the legend of its parent-forum (sub forums list)"
 msgstr ""
 " Affiche ce forum dans la légende de son forum-parent (dans la liste des "
 "forums)"
 
 msgid "Edit"
@@ -374,15 +375,15 @@
 msgid "Edit forum profile"
 msgstr "Modifier le profile"
 
 msgid "Edit group permissions"
 msgstr "Modifier les permissions de groupe"
 
 msgid "Edit post"
-msgstr "Éditer le post"
+msgstr "Éditer le message"
 
 msgid "Edit profile"
 msgstr "Modifier le profile"
 
 msgid "Edit user permissions"
 msgstr "Modifier les permissions de l'utilisateur"
 
@@ -462,15 +463,15 @@
 msgid "Forum type"
 msgstr "Type de forum"
 
 msgid "Forums"
 msgstr "Forums"
 
 msgid "Forums have been marked read."
-msgstr "Les forums ont été marqués comme prêts."
+msgstr "Les forums ont été marqués comme lus."
 
 msgid "Global forum permissions"
 msgstr "Permissions globales du forum"
 
 msgid "Go to the page:"
 msgstr "Aller à la page :"
 
@@ -586,78 +587,78 @@
 msgid "Mark forums read"
 msgstr "Marquer les forums comme 'lu'"
 
 msgid "Mark subforums read"
 msgstr "Marquer le sous-forum comme 'lu'"
 
 msgid "Mark topics read"
-msgstr "Marquer le thème comme 'lu'"
+msgstr "Marquer le sujet comme 'lu'"
 
 msgid "Maximum number of poll options per user"
 msgstr "Nombre maximum de choix possibles par utilisateur"
 
 msgid "Message"
 msgstr "Message"
 
 msgid "Moderation queue"
 msgstr "File de modération"
 
 msgid "Move down"
 msgstr "Déplacer vers le bas"
 
 msgid "Move topic"
-msgstr "Déplacer le thème"
+msgstr "Déplacer le sujet"
 
 msgid "Move up"
 msgstr "Déplacer vers le haut"
 
 msgid "My messages"
 msgstr "Mes messages"
 
 msgid "Name"
 msgstr "Nom"
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Ni Pillow ou PIL a pu être importé : {}"
 
 msgid "New post"
-msgstr "Nouveau post"
+msgstr "Nouveau message"
 
 msgid "New search"
 msgstr "Nouvelle recherche"
 
 msgid "New topic"
-msgstr "Nouveau thème"
+msgstr "Nouveau sujet"
 
 msgid "No forums."
 msgstr "Aucun forum."
 
 msgid "No posts"
-msgstr "Aucun post"
+msgstr "Aucun message"
 
 msgid "No posts awaiting approval."
-msgstr "Aucun post en attente d'approbation"
+msgstr "Aucun message en attente d'approbation"
 
 msgid "No posts found"
-msgstr "Aucun post trouvé"
+msgstr "Aucun message trouvé"
 
 msgid "No results."
 msgstr "Aucun résultat."
 
 msgid "No, take me back"
 msgstr "Non, ramène moi"
 
 msgid "Not granted"
 msgstr "Refusée"
 
 msgid "Not set"
 msgstr "Non définie"
 
 msgid "Not topics found."
-msgstr "Aucun thème trouvé."
+msgstr "Aucun sujet trouvé."
 
 msgid "On %(creation_date)s"
 msgstr "Le %(creation_date)s"
 
 msgid "Options"
 msgstr "Options"
 
@@ -670,15 +671,15 @@
 msgid "Permission codename"
 msgstr "Nom de code de la permission"
 
 msgid "Permissions successfully applied"
 msgstr " Permissions appliquées avec succès"
 
 msgid "Permissions successfully copied"
-msgstr " Permissions copiées avec succès"
+msgstr "Permissions copiées avec succès"
 
 msgid "Please correct the error below."
 msgstr "Merci de bien vouloir corriger l'erreur ci-dessous"
 
 msgid "Please correct the errors below."
 msgstr "Merci de bien vouloir corriger les erreurs ci-dessous"
 
@@ -746,24 +747,24 @@
 msgid "Posted by"
 msgstr "Posté par"
 
 msgid "Poster"
 msgstr "Auteur"
 
 msgid "Poster name"
-msgstr "Nom d'auteur de post"
+msgstr "Nom d'auteur du message"
 
 msgid "Posts"
 msgstr "Messages"
 
 msgid "Posts count"
 msgstr "Nombre de messages"
 
 msgid "Posts:"
-msgstr "Posts :"
+msgstr "Messages :"
 
 msgid "Preview"
 msgstr "Aperçu"
 
 msgid "Preview:"
 msgstr "Aperçu :"
 
@@ -773,18 +774,18 @@
 msgid "RSS feed"
 msgstr "Flux RSS"
 
 msgid "Reason:"
 msgstr "Raison :"
 
 msgid "Recent posts"
-msgstr "Posts récents"
+msgstr "Messages récents"
 
 msgid "Records the number of times a forum link was clicked"
-msgstr " Enregistre le nombre de clics sur le lien du forum"
+msgstr "Enregistre le nombre de clics sur le lien du forum"
 
 msgid "Replies"
 msgstr "Réponses"
 
 msgid "Results"
 msgstr "Résultats"
 
@@ -794,24 +795,24 @@
 msgid "Search"
 msgstr "Rechercher"
 
 msgid "Search for keywords"
 msgstr "Rechercher par mots clés"
 
 msgid "Search for poster"
-msgstr "Rechercher un auteur de post"
+msgstr "Rechercher un auteur de message"
 
 msgid "Search forums"
 msgstr "Rechercher des forums"
 
 msgid "Search in specific forums"
 msgstr "Rechercher dans un forum spécifique"
 
 msgid "Search only in topic subjects"
-msgstr "Rechercher seulement dans les sujets des thèmes"
+msgstr "Rechercher seulement dans les sujets des sujets"
 
 msgid "Select"
 msgstr "Sélectionner"
 
 msgid "Select a destination forum"
 msgstr "Sélectionner le forum de destination"
 
@@ -839,36 +840,36 @@
 msgid "Submit"
 msgstr "Soumettre"
 
 msgid "Subscribe"
 msgstr "Souscrire"
 
 msgid "Subscribe to topic"
-msgstr "Souscrire au thème"
+msgstr "S'abonner au sujet"
 
 msgid "Subscribers"
 msgstr "Abonnés"
 
 msgid "Subscriptions"
-msgstr "Souscriptions"
+msgstr "Abonnements"
 
 msgid "Target anonymous user"
 msgstr "Cibler un utilisateur anonyme"
 
 msgid "Target any logged in user"
 msgstr "Cibler tous les utilisateurs authentifiés"
 
 msgid "The profile has been edited successfully."
 msgstr "Le profil a été édité avec succès."
 
 msgid "There are no topics in this forum."
-msgstr "Il n'y a pas de thème dans ce forum."
+msgstr "Il n'y a pas de sujet dans ce forum."
 
 msgid "There are no unread topics."
-msgstr "Il n'y a aucun thème non lu."
+msgstr "Il n'y a aucun sujet non lu."
 
 msgid "There are some errors in the attachments you submitted."
 msgstr "Il y a des erreurs dans les pièces jointes soumises."
 
 msgid "There are some errors in the poll options you submitted."
 msgstr "Il y a des erreurs dans les choix du sondage."
 
@@ -892,30 +893,30 @@
 msgid "This post has been approved successfully."
 msgstr "Ce post a été approuvé avec succès."
 
 msgid "This post has been disapproved successfully."
 msgstr "Ce post a été désapprouvé avec succès."
 
 msgid "This topic has been deleted successfully."
-msgstr "Ce thème a été supprimé avec succès."
+msgstr "Ce sujet a été supprimé avec succès."
 
 msgid "This topic has been locked successfully."
-msgstr "Ce thème a été verrouillé avec succès"
+msgstr "Ce sujet a été verrouillé avec succès"
 
 msgid "This topic has been moved successfully."
-msgstr "Ce thème a été déplacé avec succès"
+msgstr "Ce sujet a été déplacé avec succès"
 
 msgid "This topic has been unlocked successfully."
-msgstr "Ce thème a été déverrouillé avec succès"
+msgstr "Ce sujet a été déverrouillé avec succès"
 
 msgid "This topic is locked"
-msgstr "Ce thème est verrouillé"
+msgstr "Ce sujet est verrouillé"
 
 msgid "This topic type has been changed successfully."
-msgstr "Ce type de thème a été modifié avec succès."
+msgstr "Ce type de sujet a été modifié avec succès."
 
 msgid "Topic"
 msgstr "Sujet"
 
 msgid "Topic forum"
 msgstr "Forum du topic"
 
@@ -940,72 +941,72 @@
 msgid "Topic poll votes"
 msgstr "Votes de sondages"
 
 msgid "Topic polls"
 msgstr "Sondages"
 
 msgid "Topic review"
-msgstr "Revue de thème"
+msgstr "Revue de sujet"
 
 msgid "Topic status"
 msgstr "Statut"
 
 msgid "Topic track"
-msgstr "Trace des thèmes"
+msgstr "Trace des sujets"
 
 msgid "Topic tracks"
-msgstr "Traces des thèmes"
+msgstr "Traces des sujets"
 
 msgid "Topic type"
 msgstr "Type de sujet"
 
 msgid "Topic unlocked"
 msgstr "Sujet déverrouillé"
 
 msgid "Topics"
 msgstr "Sujets"
 
 msgid "Topics have been marked read."
-msgstr "Les thèmes ont été marqués comme prêts."
+msgstr "Les sujets ont été marqués comme lus."
 
 msgid "Topics that you are subscribed to"
-msgstr "Thèmes auxquels vous avez souscrits"
+msgstr "Sujets auxquels vous êtes abonnés"
 
 msgid "Topics:"
-msgstr "Thèmes :"
+msgstr "Sujets :"
 
 msgid "Total posts"
 msgstr "Tous les posts"
 
 msgid "Total posts:"
-msgstr "Nombre total de posts :"
+msgstr "Nombre total de messages :"
 
 msgid "Total redirects:"
 msgstr "Nombre total de redirections :"
 
 msgid "Total topics:"
-msgstr "Nombre total de thèmes :"
+msgstr "Nombre total de sujets :"
 
 msgid "Total votes:"
 msgstr "Total des votes :"
 
 msgid "Track link redirects count"
 msgstr "Comptabiliser les redirections vers le lien du forum"
 
 msgid "Type"
 msgstr "Type"
 
 msgid "Unlock topic"
-msgstr "Déverrouiller le thème"
+msgstr "Déverrouiller le sujet"
 
 msgid "Unsubscribe"
 msgstr "Supprimer la souscription"
 
 msgid "Unsubscribe from topic"
-msgstr "Supprimer la souscription au thème."
+msgstr "Se désabonner de ce sujet."
 
 msgid "Up to <b>%(max_options)s</b> options may be selected"
 msgstr "Jusqu'à <b>%(max_options)s</b> options peuvent être sélectionnées."
 
 msgid "Update date"
 msgstr "Date de mise à jour"
 
@@ -1036,15 +1037,15 @@
 msgid "View my posts"
 msgstr "Voir mes posts"
 
 msgid "View results"
 msgstr "Voir les résultats"
 
 msgid "View unread topics"
-msgstr "Voir les thèmes non lu"
+msgstr "Voir les sujets non lu"
 
 msgid "Views"
 msgstr "Vues"
 
 msgid "Views count"
 msgstr "Nombre de vues"
 
@@ -1054,39 +1055,39 @@
 msgid "Vote's date"
 msgstr "Date du vote"
 
 msgid "Voter"
 msgstr "Votant"
 
 msgid "Would you like to subscribe to this topic?"
-msgstr "Voudriez-vous sourscrire à ce thème ?"
+msgstr "Voudriez-vous vous abonné à ce sujet ?"
 
 msgid "Would you like to unsubscribe from this topic?"
-msgstr "Voudriez-vous supprimer la souscription à ce thème ?"
+msgstr "Voudriez-vous vous désabonner de ce sujet ?"
 
 msgid "Would you want to change this topic to a default topic?"
-msgstr "Voudriez-vous changer ce thème en un thème par défaut ?"
+msgstr "Voudriez-vous changer ce sujet en un sujet par défaut ?"
 
 msgid "Would you want to change this topic to a sticky topic?"
-msgstr "Voudriez-vous mettre ce thème toujours en premier ?"
+msgstr "Voudriez-vous épingler ce sujet ?"
 
 msgid "Would you want to change this topic to an announce?"
-msgstr "Voudriez-vous que ce thème soit une annonce ?"
+msgstr "Voudriez-vous que ce sujet soit une annonce ?"
 
 msgid "Yes, I'm sure"
 msgstr "Oui, je suis sûr"
 
 msgid "You have tried to vote for too many options."
 msgstr "Vous avez choisi trop de choix possibles"
 
 msgid "You may select <b>1</b> option"
-msgstr "Vous pourriez sectionner l'option <b>1</b>"
+msgstr "Vous pourriez sélectionner l'option <b>1</b>"
 
 msgid "You may select up to <b>%(max_options)s</b> options"
-msgstr "Vous pourriez selectionner jusqu'à <b>%(max_options)s</b> options"
+msgstr "Vous pourriez sélectionner jusqu'à <b>%(max_options)s</b> options"
 
 msgid ""
 "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 "Vous devez indiquer le nombre maximum de choix par utilisateur pour le "
 "sondage"
```

### Comparing `django-machina-1.2.0/machina/locale/fr/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/fr/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -9,22 +9,22 @@
 # Morgan Aubert <morgan@aubert.email>, 2017
 # Morgan Aubert <morgan@aubert.email>, 2016
 # Tutur L <arthur.lerou@gmail.com>, 2020
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2021-06-21 20:18+0000\n"
 "Last-Translator: Gaget L <lauri.gaget@opencop.fr>\n"
 "Language-Team: French (http://www.transifex.com/django-machina-team/django-machina/language/fr/)\n"
+"Language: fr\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: fr\n"
 "Plural-Forms: nplurals=2; plural=(n > 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
 msgstr "Parent"
 
 msgid "Name"
@@ -71,16 +71,15 @@
 
 msgid "Last post added on"
 msgstr "Dernier post ajouté"
 
 msgid "Display in parent-forums legend"
 msgstr "Affichage dans la légende des forums-parents"
 
-msgid ""
-"Displays this forum on the legend of its parent-forum (sub forums list)"
+msgid "Displays this forum on the legend of its parent-forum (sub forums list)"
 msgstr " Affiche ce forum dans la légende de son forum-parent (dans la liste des forums)"
 
 msgid "Forum"
 msgstr "Forum"
 
 msgid "Forums"
 msgstr "Forums"
@@ -129,30 +128,24 @@
 
 msgid "Machina: Forum"
 msgstr "Machina: Forum"
 
 msgid "Anonymous"
 msgstr "Anonyme"
 
-msgid ""
-"Please select this option if you want to edit the permissions of the "
-"anonymous user"
+msgid "Please select this option if you want to edit the permissions of the anonymous user"
 msgstr "Veuillez sélectionner cette option si vous souhaitez éditer les permissions de l'utilisateur anonyme"
 
 msgid "Authenticated"
 msgstr "Authentifié"
 
-msgid ""
-"Please select this option if you want to edit the permissions of every (non-"
-"specific) logged in user"
+msgid "Please select this option if you want to edit the permissions of every (non-specific) logged in user"
 msgstr "Sélectionnez cette option si vous voulez modifier les permissions de tous les utilisateurs (non déterminés) authentifiés"
 
-msgid ""
-"Choose either a user ID or check either the anonymous or authenticated user "
-"checkbox"
+msgid "Choose either a user ID or check either the anonymous or authenticated user checkbox"
 msgstr "Choisir un ID d'utilisateur ou cocher soit la case anonyme ou la case utilisateur authentifié"
 
 msgid "Not set"
 msgstr "Non définie"
 
 msgid "Granted"
 msgstr "Accordée"
@@ -204,14 +197,20 @@
 
 msgid "First post"
 msgstr "Premier poste"
 
 msgid "Subscribers"
 msgstr "Abonnés"
 
+msgid "Creation date"
+msgstr "Date de création"
+
+msgid "Update date"
+msgstr "Date de mise à jour"
+
 msgid "Topic"
 msgstr "Sujet"
 
 msgid "Topics"
 msgstr "Sujets"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -243,16 +242,15 @@
 
 msgid "Posts"
 msgstr "Messages"
 
 msgid "A user id or an anonymous key must be associated with a post."
 msgstr "Un utilisateur ou une clé d'utilisateur anonyme doit être associé à un message."
 
-msgid ""
-"A user id or an anonymous key must be associated with a post, but not both."
+msgid "A user id or an anonymous key must be associated with a post, but not both."
 msgstr "Un utilisateur ou une clé d'utilisateur anonyme doit être associé à un message, mais pas les deux."
 
 msgid "A username must be specified if the poster is anonymous"
 msgstr "Un nom d'utilisateur doit être spécifié si l'utilisateur est anonyme."
 
 msgid "Machina: Forum conversations"
 msgstr "Machina: Conversations"
@@ -271,17 +269,15 @@
 
 msgid "Post topic as"
 msgstr "Publier le sujet en tant que"
 
 msgid "Poll question"
 msgstr "Question du sondage"
 
-msgid ""
-"Enter a question to associate a poll with the topic or leave blank to not "
-"create a poll."
+msgid "Enter a question to associate a poll with the topic or leave blank to not create a poll."
 msgstr "Entrez une question pour associer un sondage avec le sujet sinon laissez vide si vous ne voulez pas créer de sondage."
 
 msgid "Maximum number of poll options per user"
 msgstr "Nombre maximum de choix possibles par utilisateur"
 
 msgid "This is the number of options each user may select when voting."
 msgstr "Il s'agit nombre de choix que chaque utilisateur peut sélectionner lorsqu'il participe au sondage."
@@ -294,16 +290,23 @@
 
 msgid "Allow re-voting?"
 msgstr "Autoriser la modification des votes?"
 
 msgid "If enabled users are able to change their vote."
 msgstr "Si activé, les utilisateurs peuvent changer leurs votes."
 
-msgid ""
-"You must set the maximum number of poll options per user when creating polls"
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Voir les résultats"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
+msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "Vous devez indiquer le nombre maximum de choix par utilisateur pour le sondage"
 
 msgid "File"
 msgstr "Fichier"
 
 msgid "Comment"
 msgstr "Commentaire"
@@ -319,14 +322,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Durée du sondage, en jours"
 
 msgid "Allow vote changes"
 msgstr "Permettre les changements de votes"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Voir les résultats"
+
 msgid "Topic poll"
 msgstr "Sondage"
 
 msgid "Topic polls"
 msgstr "Sondages"
 
 msgid "Poll"
@@ -487,17 +495,15 @@
 
 msgid "User forum permission"
 msgstr "Permission de l'utilisateur pour le forum"
 
 msgid "User forum permissions"
 msgstr "Permissions de l'utilisateur du forum"
 
-msgid ""
-"A permission should target either a specific user, an anonymous user or any "
-"authenticated user"
+msgid "A permission should target either a specific user, an anonymous user or any authenticated user"
 msgstr "Une permission devrait cibler soit un utilisateur spécifique, un utilisateur anonyme ou n’importe quel utilisateur authentifié"
 
 msgid "Group"
 msgstr "Groupe"
 
 msgid "Group forum permission"
 msgstr "Permission de groupe pour le forum"
@@ -612,41 +618,45 @@
 
 msgid "Topics have been marked read."
 msgstr "Les sujets ont été marqués comme lus."
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Ni Pillow ou PIL a pu être importé : {}"
 
-msgid "Creation date"
-msgstr "Date de création"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "Impossible d'importer MACHINA_MARKUP_LANGUAGE {}: {}"
 
-msgid "Update date"
-msgstr "Date de mise à jour"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "Les paramètres de MACHINA_MARKUP_LANGUAGE sont requis"
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "Impossible d'importer MACHINA_MARKUP_WIDGET {}: {}"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "Impossible d'importer MACHINA_MARKUP_LANGUAGE {}: {}"
 
 msgid "MACHINA_MARKUP_LANGUAGE setting is required"
 msgstr "Les paramètres de MACHINA_MARKUP_LANGUAGE sont requis"
 
 msgid "Files of size greater than {} are not allowed. Your file is {}"
 msgstr "Les fichiers qui dépasse la taille de {} ne sont pas autorisés. Votre fichier est {}."
 
-msgid ""
-"Images of width lesser than {}px or greater than {}px or are not allowed. "
-"The width of your image is {}px"
-msgstr "Les images de largeur inférieur à {} px ou supérieur à {} px ne sont pas autorisées.\nLa largeur de votre image est de {} px."
+msgid "Images of width lesser than {}px or greater than {}px or are not allowed. The width of your image is {}px"
+msgstr ""
+"Les images de largeur inférieur à {} px ou supérieur à {} px ne sont pas autorisées.\n"
+"La largeur de votre image est de {} px."
 
-msgid ""
-"Images of height lesser than {}px or greater than {}px or are not allowed. "
-"The height of your image is {}px"
-msgstr "Les images de hauteur inférieur à {} px ou supérieur à {} px ne sont pas autorisées.\nLa hauteur de votre image est de {} px."
+msgid "Images of height lesser than {}px or greater than {}px or are not allowed. The height of your image is {}px"
+msgstr ""
+"Les images de hauteur inférieur à {} px ou supérieur à {} px ne sont pas autorisées.\n"
+"La hauteur de votre image est de {} px."
 
 msgid "List of forums"
 msgstr "Liste des forums"
 
 msgid "Quick actions"
 msgstr "Actions rapides"
 
@@ -709,17 +719,15 @@
 
 msgid "Please select a group in order to update its permissions"
 msgstr "Merci de sélectionner un groupe afin de mettre à jour ses permissions"
 
 msgid "Copy permissions from another forum"
 msgstr "Copier les permissions à partir d'un autre forum"
 
-msgid ""
-"Please select a forum in order to copy its permissions configuration to the "
-"current forum"
+msgid "Please select a forum in order to copy its permissions configuration to the current forum"
 msgstr "Merci de sélectionner un forum afin de copier la configuration de ses permissions vers le forum actuel."
 
 msgid "Copy"
 msgstr "Copier"
 
 msgid "Search"
 msgstr "Rechercher"
@@ -738,17 +746,14 @@
 
 msgid "Mark subforums read"
 msgstr "Marquer le sous-forum comme 'lu'"
 
 msgid "New topic"
 msgstr "Nouveau sujet"
 
-msgid "New Topic"
-msgstr "Nouveau Sujet"
-
 msgid "Mark topics read"
 msgstr "Marquer le sujet comme 'lu'"
 
 msgid "Announcements"
 msgstr "Annonces"
 
 msgid "RSS feed"
@@ -813,22 +818,23 @@
 
 msgid "Poll options"
 msgstr "Options de sondage"
 
 msgid "Add a poll option"
 msgstr "Ajouter une option de sondage"
 
-msgid ""
-"<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the "
-"associated votes."
+msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "<b>Note:</b>&nbsp;Supprimer les options de sondage d'un sondage existant supprimera les votes associés."
 
 msgid "Preview:"
 msgstr "Aperçu :"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Total des votes :"
 
 msgid "Submit"
 msgstr "Soumettre"
 
 msgid "View results"
@@ -948,26 +954,34 @@
 #, python-format
 msgid ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Post</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Posts</small></p>"
-msgstr[0] "<h2><strong>%(counter)s</strong></h2>\n<p><small>Post</small></p>"
-msgstr[1] "<h2><strong>%(counter)s</strong></h2>\n<p class=\"mb-1\"><small>Posts</small></p>"
+msgstr[0] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p><small>Post</small></p>"
+msgstr[1] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p class=\"mb-1\"><small>Posts</small></p>"
 
 #, python-format
 msgid ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Topic</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Topics</small></p>"
-msgstr[0] "<h2><strong>%(counter)s</strong></h2>\n<p><small>Sujet</small></p>"
-msgstr[1] "<h2><strong>%(counter)s</strong></h2>\n<p class=\"mb-1\"><small>sujet</small></p>"
+msgstr[0] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p><small>Sujet</small></p>"
+msgstr[1] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p class=\"mb-1\"><small>sujet</small></p>"
 
 msgid "Recent posts"
 msgstr "Messages récents"
 
 msgid "View all"
 msgstr "Voir tout"
 
@@ -1046,16 +1060,15 @@
 
 msgid "Are you sure you want to approve this post?"
 msgstr "Êtes-vous sûr de vouloir approuver ce message ?"
 
 msgid "Disapprove post"
 msgstr "Désapprouver ce message"
 
-msgid ""
-"Are you sure you want to disapprove this post? This post will be deleted."
+msgid "Are you sure you want to disapprove this post? This post will be deleted."
 msgstr "Êtes-vous sûr de vouloir désapprouver ce message ? Celui-ci sera donc supprimé."
 
 msgid "Are you sure you want to delete this topic?"
 msgstr "Êtes-vous sûr de vouloir supprimer ce sujet ?"
 
 msgid "Are you sure you want to lock this topic?"
 msgstr "Êtes-vous sûr de vouloir verrouiller ce sujet ?"
@@ -1097,7 +1110,10 @@
 msgstr[1] ""
 
 msgid "There are no unread topics."
 msgstr "Il n'y a aucun sujet non lu."
 
 msgid "Forum index"
 msgstr "Index du forum"
+
+#~ msgid "New Topic"
+#~ msgstr "Nouveau Sujet"
```

### Comparing `django-machina-1.2.0/machina/locale/fr_CA/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/fr_CA/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/fr_CA/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/fr_CA/LC_MESSAGES/django.po`

 * *Files 6% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Translators:
 # anthony laquerre <anthony.laquerre@ccsr.qc.ca>, 2016
 # Morgan Aubert <morgan@aubert.email>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: French (Canada) (http://www.transifex.com/django-machina-team/django-machina/language/fr_CA/)\n"
 "Language: fr_CA\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -193,14 +193,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr "Abonnés"
 
+msgid "Creation date"
+msgstr "Date de création"
+
+msgid "Update date"
+msgstr "Date de mise à jour"
+
 msgid "Topic"
 msgstr "Sujet"
 
 msgid "Topics"
 msgstr "Sujets"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -280,14 +286,22 @@
 
 msgid "Allow re-voting?"
 msgstr "Autoriser la modification des votes?"
 
 msgid "If enabled users are able to change their vote."
 msgstr "Si activé, les utilisateurs peuvent changer leurs votes."
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Voir les résultats"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "Vous devez indiquer le nombre maximum de choix par utilisateur pour le sondage"
 
 msgid "File"
 msgstr "Fichier"
 
 msgid "Comment"
@@ -304,14 +318,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Durée du sondage, en jours"
 
 msgid "Allow vote changes"
 msgstr "Permettre les changements de votes"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Voir les résultats"
+
 msgid "Topic poll"
 msgstr "Sondage"
 
 msgid "Topic polls"
 msgstr "Sondages"
 
 msgid "Poll"
@@ -595,19 +614,23 @@
 
 msgid "Topics have been marked read."
 msgstr "Les sujets ont été marqués comme lus."
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Neither Pillow nor PIL could be imported: {}"
 
-msgid "Creation date"
-msgstr "Date de création"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 
-msgid "Update date"
-msgstr "Date de mise à jour"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "MACHINA_MARKUP_LANGUAGE setting is required"
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 
@@ -793,14 +816,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "<b>Note :</b>&nbsp;La suppression des options d'un sondage existant entraînera la suppression des votes associés."
 
 msgid "Preview:"
 msgstr "Aperçu :"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Nombre de votes :"
 
 msgid "Submit"
 msgstr "Soumettre"
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/hu/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/hu/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/hu/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/hu/LC_MESSAGES/django.po`

 * *Files 5% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Translators:
 # Peter Torok <peter@bluefridge.com>, 2018
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: Hungarian (http://www.transifex.com/django-machina-team/django-machina/language/hu/)\n"
 "Language: hu\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -192,14 +192,20 @@
 
 msgid "First post"
 msgstr "Első hozzászólás"
 
 msgid "Subscribers"
 msgstr "Feliratkozók"
 
+msgid "Creation date"
+msgstr "Létrehozás dátuma"
+
+msgid "Update date"
+msgstr "Módosítás dátuma"
+
 msgid "Topic"
 msgstr "Téma"
 
 msgid "Topics"
 msgstr "Témák"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -279,14 +285,22 @@
 
 msgid "Allow re-voting?"
 msgstr "Újraszavazás engedélyezése?"
 
 msgid "If enabled users are able to change their vote."
 msgstr "Ha engedélyezett, akkor a felhasználók megváltoztathatják a szavazatukat."
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Találatok megtekintése"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "Szavazás létrehozásakor kötelező megadni a válaszlehetőségek felhasználónként megadható számát."
 
 msgid "File"
 msgstr "File"
 
 msgid "Comment"
@@ -303,14 +317,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Szavazás időtartama napokban"
 
 msgid "Allow vote changes"
 msgstr "Szavazatmódosítás engedélyezése"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Találatok megtekintése"
+
 msgid "Topic poll"
 msgstr "Téma-szavazás"
 
 msgid "Topic polls"
 msgstr "Téma-szavazások"
 
 msgid "Poll"
@@ -594,19 +613,23 @@
 
 msgid "Topics have been marked read."
 msgstr "Témák olvasottnak jelölve."
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Sem a Pillow, sem a PIL beimportálása nem sikerült: {}"
 
-msgid "Creation date"
-msgstr "Létrehozás dátuma"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "Nem lehetett beimportálni: MACHINA_MARKUP_LANGUAGE {}: {}"
 
-msgid "Update date"
-msgstr "Módosítás dátuma"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "MACHINA_MARKUP_LANGUAGE beállítás szükséges"
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "Nem lehetett beimportálni: MACHINA_MARKUP_WIDGET {}: {}"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "Nem lehetett beimportálni: MACHINA_MARKUP_LANGUAGE {}: {}"
 
@@ -792,14 +815,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "<b>Figyelem:</b>&nbsp;Ha meglévő szavazás válaszlehetőségeit törli, akkor a hozzátartozó szavazatok is törlődnek."
 
 msgid "Preview:"
 msgstr "Előnézet:"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Szavazatok összesen:"
 
 msgid "Submit"
 msgstr "Küldés"
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/it/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/cs/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
-"PO-Revision-Date: 2019-10-29 01:36+0000\n"
-"Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
-"Language-Team: Italian (http://www.transifex.com/django-machina-team/django-machina/language/it/)\n"
-"Language: it\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
+"PO-Revision-Date: 2016-02-23 03:25+0000\n"
+"Last-Translator: \n"
+"Language-Team: Czech (http://www.transifex.com/django-machina-team/django-machina/language/cs/)\n"
+"Language: cs\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n != 1);\n"
+"Plural-Forms: nplurals=4; plural=(n == 1 && n % 1 == 0) ? 0 : (n >= 2 && n <= 4 && n % 1 == 0) ? 1: (n % 1 != 0 ) ? 2 : 3;\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
 msgstr ""
 
 msgid "Name"
 msgstr ""
@@ -191,14 +191,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr ""
 
+msgid "Creation date"
+msgstr ""
+
+msgid "Update date"
+msgstr ""
+
 msgid "Topic"
 msgstr ""
 
 msgid "Topics"
 msgstr ""
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -278,14 +284,20 @@
 
 msgid "Allow re-voting?"
 msgstr ""
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
+msgid "Hide results?"
+msgstr ""
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr ""
 
 msgid "Comment"
@@ -302,14 +314,17 @@
 
 msgid "Poll duration, in days"
 msgstr ""
 
 msgid "Allow vote changes"
 msgstr ""
 
+msgid "Hide results"
+msgstr ""
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -593,18 +608,18 @@
 
 msgid "Topics have been marked read."
 msgstr ""
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
 msgstr ""
 
-msgid "Update date"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
@@ -791,14 +806,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr ""
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr ""
 
 msgid "Submit"
 msgstr ""
 
 msgid "View results"
@@ -882,14 +900,16 @@
 msgstr ""
 
 #, python-format
 msgid "edited %(counter)s time in total."
 msgid_plural "edited %(counter)s times in total."
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 msgid "Reason:"
 msgstr ""
 
 msgid "Replies"
 msgstr ""
 
@@ -920,24 +940,28 @@
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Post</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Posts</small></p>"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 #, python-format
 msgid ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Topic</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Topics</small></p>"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 msgid "Recent posts"
 msgstr ""
 
 msgid "View all"
 msgstr ""
 
@@ -952,14 +976,16 @@
 msgstr ""
 
 #, python-format
 msgid "%(counter)s topic found"
 msgid_plural "%(counter)s topics found"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 msgid "Not topics found."
 msgstr ""
 
 msgid "Subscribe to topic"
 msgstr ""
 
@@ -980,14 +1006,16 @@
 msgstr ""
 
 #, python-format
 msgid "%(counter)s post found"
 msgid_plural "%(counter)s posts found"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 msgid "No posts found"
 msgstr ""
 
 msgid "Disapprove"
 msgstr ""
 
@@ -1042,14 +1070,16 @@
 msgstr ""
 
 #, python-format
 msgid "Your search has returned <b>%(number_of_results)s</b> result"
 msgid_plural "Your search has returned <b>%(number_of_results)s</b> results"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 msgid "Results"
 msgstr ""
 
 msgid "No results."
 msgstr ""
 
@@ -1060,13 +1090,15 @@
 msgstr ""
 
 #, python-format
 msgid "%(topic_length)s unread topic found"
 msgid_plural "%(topic_length)s unread topics found"
 msgstr[0] ""
 msgstr[1] ""
+msgstr[2] ""
+msgstr[3] ""
 
 msgid "There are no unread topics."
 msgstr ""
 
 msgid "Forum index"
 msgstr ""
```

### Comparing `django-machina-1.2.0/machina/locale/ja_JP/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/ja_JP/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/ja_JP/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/ja_JP/LC_MESSAGES/django.po`

 * *Files 4% similar despite different names*

```diff
@@ -4,15 +4,15 @@
 #
 # Translators:
 # I K <ki.foobar@gmail.com>, 2019
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: Japanese (Japan) (http://www.transifex.com/django-machina-team/django-machina/language/ja_JP/)\n"
 "Language: ja_JP\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -192,14 +192,20 @@
 
 msgid "First post"
 msgstr "最初の投稿"
 
 msgid "Subscribers"
 msgstr "購読者"
 
+msgid "Creation date"
+msgstr "作成日"
+
+msgid "Update date"
+msgstr "更新日"
+
 msgid "Topic"
 msgstr "トピック"
 
 msgid "Topics"
 msgstr "トピック"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -279,14 +285,22 @@
 
 msgid "Allow re-voting?"
 msgstr "再投票を認めるか"
 
 msgid "If enabled users are able to change their vote."
 msgstr "有効にした場合は、票を後から変更することができます"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "結果を見る"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "投票を設置するときは、一人当たりの最大投票数を設定する必要があります"
 
 msgid "File"
 msgstr "ファイル"
 
 msgid "Comment"
@@ -303,14 +317,19 @@
 
 msgid "Poll duration, in days"
 msgstr "投票受付時間 (単位: 日)"
 
 msgid "Allow vote changes"
 msgstr "票の変更を認める"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "結果を見る"
+
 msgid "Topic poll"
 msgstr "トピックの投票"
 
 msgid "Topic polls"
 msgstr "トピックの投票"
 
 msgid "Poll"
@@ -594,19 +613,23 @@
 
 msgid "Topics have been marked read."
 msgstr "トピックを既読にしました"
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Pillow、PILのどちらもimportできませんでした: {}"
 
-msgid "Creation date"
-msgstr "作成日"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "MACHINA_MARKUP_LANGUAGE {} をimportできません: {}"
 
-msgid "Update date"
-msgstr "更新日"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "MACHINA_MARKUP_LANGUAGEの設定は必須です"
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "MACHINA_MARKUP_WIDGET {} をimportできません: {}"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "MACHINA_MARKUP_LANGUAGE {} をimportできません: {}"
 
@@ -792,14 +815,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "<b>注意:</b>&nbsp;選択肢を削除するとそれに投票した票も失われます"
 
 msgid "Preview:"
 msgstr "プレビュー:"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "合計投票数:"
 
 msgid "Submit"
 msgstr "送信"
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/nb/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/nb/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/nb/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/nb/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -5,15 +5,15 @@
 # Translators:
 # Simen Heggestøyl <simenheg@gmail.com>, 2016
 # Stein Strindhaug <stein.strindhaug@gmail.com>, 2016-2017
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: Norwegian Bokmål (http://www.transifex.com/django-machina-team/django-machina/language/nb/)\n"
 "Language: nb\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -193,14 +193,20 @@
 
 msgid "First post"
 msgstr "Første innlegg"
 
 msgid "Subscribers"
 msgstr "Abonnenter"
 
+msgid "Creation date"
+msgstr "Opprettelsesdato"
+
+msgid "Update date"
+msgstr "Oppdateringsdato"
+
 msgid "Topic"
 msgstr "Tråd"
 
 msgid "Topics"
 msgstr "Tråder"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -280,14 +286,22 @@
 
 msgid "Allow re-voting?"
 msgstr "Tillat omvalg?"
 
 msgid "If enabled users are able to change their vote."
 msgstr "Hvis på, så vil brukere kunne endre sine stemmer."
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Vis resultater"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "Du må angi et maksimalt antall avstemningsvalg per bruker når du lager avstemninger"
 
 msgid "File"
 msgstr "Fil"
 
 msgid "Comment"
@@ -304,14 +318,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Varighet på avstemningen, i dager"
 
 msgid "Allow vote changes"
 msgstr "Tillat endring av stemmer"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Vis resultater"
+
 msgid "Topic poll"
 msgstr "Trådavstemning"
 
 msgid "Topic polls"
 msgstr "Trådavstemninger"
 
 msgid "Poll"
@@ -595,19 +614,23 @@
 
 msgid "Topics have been marked read."
 msgstr "Tråder har blitt markert som lest."
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Hverken Pillow eller PIL kunne importeres: {}"
 
-msgid "Creation date"
-msgstr "Opprettelsesdato"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "Kunne ikke importere MACHINA_MARKUP_LANGUAGE {}: {}"
 
-msgid "Update date"
-msgstr "Oppdateringsdato"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "Innstillingen MACHINA_MARKUP_LANGUAGE er påkrevd"
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "Kunne ikke importere MACHINA_MARKUP_WIDGET {}: {}"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "Kunne ikke importere MACHINA_MARKUP_LANGUAGE {}: {}"
 
@@ -793,14 +816,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "<b>Merk:</b>&nbsp;Sletting av et avstemningsvalg på en eksisterende avstemning vil også slette de tilhørende stemmene."
 
 msgid "Preview:"
 msgstr "Forhåndsvisning:"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Antall stemmer totalt:"
 
 msgid "Submit"
 msgstr "Send inn"
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/nl_NL/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/nl_NL/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-11-27 10:19+0000\n"
 "Last-Translator: Brenda H <brendahellenthal@gmail.com>\n"
 "Language-Team: Dutch (Netherlands) (http://www.transifex.com/django-machina-"
 "team/django-machina/language/nl_NL/)\n"
+"Language: nl_NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: nl_NL\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "%(counter)s post found"
 msgid_plural "%(counter)s posts found"
 msgstr[0] "%(counter)s bericht gevonden"
 msgstr[1] "%(counter)s berichten gevonden"
```

### Comparing `django-machina-1.2.0/machina/locale/nl_NL/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/nl_NL/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -1,27 +1,27 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # Brenda H <brendahellenthal@gmail.com>, 2018-2019
 # S. Jansen <samuel.anton.j@gmail.com>, 2016-2018
 # S. Jansen <samuel.anton.j@gmail.com>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-11-27 10:19+0000\n"
 "Last-Translator: Brenda H <brendahellenthal@gmail.com>\n"
 "Language-Team: Dutch (Netherlands) (http://www.transifex.com/django-machina-team/django-machina/language/nl_NL/)\n"
+"Language: nl_NL\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: nl_NL\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
 msgstr "Onderdeel van"
 
 msgid "Name"
@@ -68,16 +68,15 @@
 
 msgid "Last post added on"
 msgstr "Laatste bericht toegevoegd op"
 
 msgid "Display in parent-forums legend"
 msgstr "Geef weer in hoofdforum legenda"
 
-msgid ""
-"Displays this forum on the legend of its parent-forum (sub forums list)"
+msgid "Displays this forum on the legend of its parent-forum (sub forums list)"
 msgstr "Geeft dit forum weer in de legenda van de bijhorende hoofdforum (deelfora lijst)"
 
 msgid "Forum"
 msgstr "Forum"
 
 msgid "Forums"
 msgstr "Fora"
@@ -126,30 +125,24 @@
 
 msgid "Machina: Forum"
 msgstr "Machina: Forum"
 
 msgid "Anonymous"
 msgstr "Anoniem"
 
-msgid ""
-"Please select this option if you want to edit the permissions of the "
-"anonymous user"
+msgid "Please select this option if you want to edit the permissions of the anonymous user"
 msgstr "Selecteer een optie als je de rechten van de anonieme gebruiker wilt bewerken"
 
 msgid "Authenticated"
 msgstr "Geauthenticeerd"
 
-msgid ""
-"Please select this option if you want to edit the permissions of every (non-"
-"specific) logged in user"
+msgid "Please select this option if you want to edit the permissions of every (non-specific) logged in user"
 msgstr "Kies deze optie als je de permissies wilt bewerken van elke (niet-specifieke) ingelogde gebruiker"
 
-msgid ""
-"Choose either a user ID or check either the anonymous or authenticated user "
-"checkbox"
+msgid "Choose either a user ID or check either the anonymous or authenticated user checkbox"
 msgstr "Kies een gebruikers-ID of vink de checkbox aan van ofwel de anonieme ofwel de geauthenticeerde gebruiker"
 
 msgid "Not set"
 msgstr "Niet ingesteld"
 
 msgid "Granted"
 msgstr "Toegestaan"
@@ -201,14 +194,20 @@
 
 msgid "First post"
 msgstr "Eerste reactie"
 
 msgid "Subscribers"
 msgstr "Abonnees"
 
+msgid "Creation date"
+msgstr "Aanmaakdatum"
+
+msgid "Update date"
+msgstr "Werk datum bij"
+
 msgid "Topic"
 msgstr "Onderwerp"
 
 msgid "Topics"
 msgstr "Onderwerpen"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -240,16 +239,15 @@
 
 msgid "Posts"
 msgstr "Berichten"
 
 msgid "A user id or an anonymous key must be associated with a post."
 msgstr "De reactie moet een gebruikers-ID of een anonieme gebruiker hebben."
 
-msgid ""
-"A user id or an anonymous key must be associated with a post, but not both."
+msgid "A user id or an anonymous key must be associated with a post, but not both."
 msgstr "Enkel een gebruikers-ID of een anonieme gebruiker moet geselecteerd zijn, maar niet beide."
 
 msgid "A username must be specified if the poster is anonymous"
 msgstr "Een gebruikersnaam moet ingevuld zijn als de gebruiker anoniem is"
 
 msgid "Machina: Forum conversations"
 msgstr "Machina: Forum conversaties"
@@ -268,17 +266,15 @@
 
 msgid "Post topic as"
 msgstr "Plaats onderwerp als"
 
 msgid "Poll question"
 msgstr "Poll vraag"
 
-msgid ""
-"Enter a question to associate a poll with the topic or leave blank to not "
-"create a poll."
+msgid "Enter a question to associate a poll with the topic or leave blank to not create a poll."
 msgstr "Vul een vraag in om weer te geven, of niets om deze weg te laten."
 
 msgid "Maximum number of poll options per user"
 msgstr "Maximale keuzes per gebruiker"
 
 msgid "This is the number of options each user may select when voting."
 msgstr "Dit is het aantal opties die de gebruiker mag kiezen om op te stemmen."
@@ -291,16 +287,23 @@
 
 msgid "Allow re-voting?"
 msgstr "Nogmaals stemmen toestaan?"
 
 msgid "If enabled users are able to change their vote."
 msgstr "Of gebruikers hun stem mogen wijzigen."
 
-msgid ""
-"You must set the maximum number of poll options per user when creating polls"
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Bekijk resultaten"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
+msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "Je moet een maximaal aantal kiesopties per gebruiker instellen"
 
 msgid "File"
 msgstr "Bestand"
 
 msgid "Comment"
 msgstr "Commentaar"
@@ -316,14 +319,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Tijdsduur, in dagen"
 
 msgid "Allow vote changes"
 msgstr "Sta keuzeverandering toe"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Bekijk resultaten"
+
 msgid "Topic poll"
 msgstr "Onderwerp vraag"
 
 msgid "Topic polls"
 msgstr "Onderwerp vragen"
 
 msgid "Poll"
@@ -484,17 +492,15 @@
 
 msgid "User forum permission"
 msgstr "Forum rechten gebruiker"
 
 msgid "User forum permissions"
 msgstr "Forum rechten gebruiker"
 
-msgid ""
-"A permission should target either a specific user, an anonymous user or any "
-"authenticated user"
+msgid "A permission should target either a specific user, an anonymous user or any authenticated user"
 msgstr "Een permissie moet van toepassing zijn op ofwel een specifieke gebruiker, een anonieme gebruiker of elke geauthenticeerde gebruiker"
 
 msgid "Group"
 msgstr "Groep"
 
 msgid "Group forum permission"
 msgstr "Forum rechten groep"
@@ -609,40 +615,40 @@
 
 msgid "Topics have been marked read."
 msgstr "Onderwerpen zijn gemarkeerd als gelezen."
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Pillow noch PIL kunnen geïmporteerd worden: {}"
 
-msgid "Creation date"
-msgstr "Aanmaakdatum"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "Kon niet MACHINA_MARKUP_LANGUAGE {}: {} importeren"
 
-msgid "Update date"
-msgstr "Werk datum bij"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "MACHINA_MARKUP_LANGUAGE instelling is verplicht"
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "Kon niet MACHINA_MARKUP_WIDGET {}: {} importeren"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "Kon niet MACHINA_MARKUP_LANGUAGE {}: {} importeren"
 
 msgid "MACHINA_MARKUP_LANGUAGE setting is required"
 msgstr "MACHINA_MARKUP_LANGUAGE instelling is verplicht"
 
 msgid "Files of size greater than {} are not allowed. Your file is {}"
 msgstr "Bestanden groter dan {} zijn niet toegestaan. Jouw bestand is {}"
 
-msgid ""
-"Images of width lesser than {}px or greater than {}px or are not allowed. "
-"The width of your image is {}px"
+msgid "Images of width lesser than {}px or greater than {}px or are not allowed. The width of your image is {}px"
 msgstr "Afbeeldingen met breedte kleinder dan {}px of groter dan {}px zijn niet toegestaan. De breedte van je afbeelding is {}px"
 
-msgid ""
-"Images of height lesser than {}px or greater than {}px or are not allowed. "
-"The height of your image is {}px"
+msgid "Images of height lesser than {}px or greater than {}px or are not allowed. The height of your image is {}px"
 msgstr "Afbeeldingen met hoogte kleinder dan {}px of groter dan {}px zijn niet toegestaan. De hoogte van je afbeelding is {}px"
 
 msgid "List of forums"
 msgstr "Lijst van fora"
 
 msgid "Quick actions"
 msgstr "Snelle acties"
@@ -706,17 +712,15 @@
 
 msgid "Please select a group in order to update its permissions"
 msgstr "Selecteer een groep om zijn rechten bij te werken"
 
 msgid "Copy permissions from another forum"
 msgstr "Kopieer rechten van een ander forum"
 
-msgid ""
-"Please select a forum in order to copy its permissions configuration to the "
-"current forum"
+msgid "Please select a forum in order to copy its permissions configuration to the current forum"
 msgstr "Selecteer een forum om zijn rechten naar het huidige forum te kopiëren"
 
 msgid "Copy"
 msgstr "Kopiëren"
 
 msgid "Search"
 msgstr "Zoeken"
@@ -807,22 +811,23 @@
 
 msgid "Poll options"
 msgstr "Stem opties"
 
 msgid "Add a poll option"
 msgstr "Voeg een optie toe"
 
-msgid ""
-"<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the "
-"associated votes."
+msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "<b>Let op:</b>&nbsp; Het verwijderen van een optie zal de bijhorende stemmen ook verwijderen"
 
 msgid "Preview:"
 msgstr "Voorvertoning"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Totaal aantal stemmen:"
 
 msgid "Submit"
 msgstr "Verzenden"
 
 msgid "View results"
@@ -942,26 +947,34 @@
 #, python-format
 msgid ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Post</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Posts</small></p>"
-msgstr[0] "<h2><strong>%(counter)s</strong></h2>\n                      <p><small>Bericht</small></p>"
-msgstr[1] "<h2><strong>%(counter)s</strong></h2>\n                      <p class=\"mb-1\"><small>Berichten</small></p>"
+msgstr[0] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"                      <p><small>Bericht</small></p>"
+msgstr[1] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"                      <p class=\"mb-1\"><small>Berichten</small></p>"
 
 #, python-format
 msgid ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Topic</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Topics</small></p>"
-msgstr[0] "<h2><strong>%(counter)s</strong></h2>\n                      <p><small>Onderwerp</small></p>"
-msgstr[1] "<h2><strong>%(counter)s</strong></h2>\n                      <p class=\"mb-1\"><small>Onderwerpen</small></p>"
+msgstr[0] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"                      <p><small>Onderwerp</small></p>"
+msgstr[1] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"                      <p class=\"mb-1\"><small>Onderwerpen</small></p>"
 
 msgid "Recent posts"
 msgstr "Recente berichten"
 
 msgid "View all"
 msgstr "Bekijk alles"
 
@@ -1040,16 +1053,15 @@
 
 msgid "Are you sure you want to approve this post?"
 msgstr "Weet je zeker dat je dit bericht wilt goedkeuren?"
 
 msgid "Disapprove post"
 msgstr "Bericht afkeuren"
 
-msgid ""
-"Are you sure you want to disapprove this post? This post will be deleted."
+msgid "Are you sure you want to disapprove this post? This post will be deleted."
 msgstr "Weet je zeker dat je dit bericht wilt afkeuren? Het bericht zal worden verwijderd."
 
 msgid "Are you sure you want to delete this topic?"
 msgstr "Weet je zeker dat je dit onderwerp wilt verwijderen?"
 
 msgid "Are you sure you want to lock this topic?"
 msgstr "Weet je zeker dat je dit onderwerp wilt vergrendelen?"
```

### Comparing `django-machina-1.2.0/machina/locale/pl/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/pl/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/pl/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/pl/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: Polish (http://www.transifex.com/django-machina-team/django-machina/language/pl/)\n"
 "Language: pl\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -191,14 +191,20 @@
 
 msgid "First post"
 msgstr "Pierwszy post"
 
 msgid "Subscribers"
 msgstr "Subskrybenci"
 
+msgid "Creation date"
+msgstr "Data utworzenia"
+
+msgid "Update date"
+msgstr "Data edycji"
+
 msgid "Topic"
 msgstr "Temat"
 
 msgid "Topics"
 msgstr "Tematy"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -278,14 +284,22 @@
 
 msgid "Allow re-voting?"
 msgstr "Pozwalaj na zmianę odpowiedzi?"
 
 msgid "If enabled users are able to change their vote."
 msgstr "Określa czy użytkownik może zmienić odpowiedź."
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Zobacz wyniki"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "Musisz ustalić maksymalną liczbę odpowiedzi na użytkownika w czasie tworzenia ankiety"
 
 msgid "File"
 msgstr "Plik"
 
 msgid "Comment"
@@ -302,14 +316,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Czas trwania ankiety w dniach"
 
 msgid "Allow vote changes"
 msgstr "Pozwól zmieniać odpowiedzi"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Zobacz wyniki"
+
 msgid "Topic poll"
 msgstr "Temat z ankietą"
 
 msgid "Topic polls"
 msgstr "Tematy z ankietą"
 
 msgid "Poll"
@@ -593,19 +612,23 @@
 
 msgid "Topics have been marked read."
 msgstr "Tematy oznaczono jako przeczytane."
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Nie można zaimportować Pillow ani PIL: {}"
 
-msgid "Creation date"
-msgstr "Data utworzenia"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "Nie można zaimportować MACHINA_MARKUP_LANGUAGE {}: {}"
 
-msgid "Update date"
-msgstr "Data edycji"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "Ustawienie MACHINA_MARKUP_LANGUAGE jest wymagane"
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "Nie można zaimportować MACHINA_MARKUP_WIDGET {}: {}"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "Nie można zaimportować MACHINA_MARKUP_LANGUAGE {}: {}"
 
@@ -791,14 +814,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "<b>Ostrzeżenie:</b>&nbsp;Usunięcie opcji w istniejącej ankiecie usunię przypisane głosy"
 
 msgid "Preview:"
 msgstr "Podgląd:"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Łącznie głosów:"
 
 msgid "Submit"
 msgstr "Wyślij"
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/pt_BR/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/ca/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
-"PO-Revision-Date: 2019-10-29 01:36+0000\n"
-"Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
-"Language-Team: Portuguese (Brazil) (http://www.transifex.com/django-machina-team/django-machina/language/pt_BR/)\n"
-"Language: pt_BR\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
+"PO-Revision-Date: 2016-02-23 03:25+0000\n"
+"Last-Translator: \n"
+"Language-Team: Catalan (http://www.transifex.com/django-machina-team/django-machina/language/ca/)\n"
+"Language: ca\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=2; plural=(n > 1);\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
 msgstr ""
 
 msgid "Name"
 msgstr ""
@@ -191,14 +191,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr ""
 
+msgid "Creation date"
+msgstr ""
+
+msgid "Update date"
+msgstr ""
+
 msgid "Topic"
 msgstr ""
 
 msgid "Topics"
 msgstr ""
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -278,14 +284,20 @@
 
 msgid "Allow re-voting?"
 msgstr ""
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
+msgid "Hide results?"
+msgstr ""
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr ""
 
 msgid "Comment"
@@ -302,14 +314,17 @@
 
 msgid "Poll duration, in days"
 msgstr ""
 
 msgid "Allow vote changes"
 msgstr ""
 
+msgid "Hide results"
+msgstr ""
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -593,18 +608,18 @@
 
 msgid "Topics have been marked read."
 msgstr ""
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
 msgstr ""
 
-msgid "Update date"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
@@ -791,14 +806,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr ""
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr ""
 
 msgid "Submit"
 msgstr ""
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/ro/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/ro/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/ro/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/ro/LC_MESSAGES/django.po`

 * *Files 0% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: Romanian (http://www.transifex.com/django-machina-team/django-machina/language/ro/)\n"
 "Language: ro\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -191,14 +191,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr ""
 
+msgid "Creation date"
+msgstr ""
+
+msgid "Update date"
+msgstr ""
+
 msgid "Topic"
 msgstr ""
 
 msgid "Topics"
 msgstr ""
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -278,14 +284,20 @@
 
 msgid "Allow re-voting?"
 msgstr ""
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
+msgid "Hide results?"
+msgstr ""
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr ""
 
 msgid "Comment"
@@ -302,14 +314,17 @@
 
 msgid "Poll duration, in days"
 msgstr ""
 
 msgid "Allow vote changes"
 msgstr ""
 
+msgid "Hide results"
+msgstr ""
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -593,18 +608,18 @@
 
 msgid "Topics have been marked read."
 msgstr ""
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
 msgstr ""
 
-msgid "Update date"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
@@ -791,14 +806,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr ""
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr ""
 
 msgid "Submit"
 msgstr ""
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/ro_RO/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/ro_RO/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/ro_RO/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/ro_RO/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,15 +3,15 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: Romanian (Romania) (http://www.transifex.com/django-machina-team/django-machina/language/ro_RO/)\n"
 "Language: ro_RO\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -191,14 +191,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr ""
 
+msgid "Creation date"
+msgstr ""
+
+msgid "Update date"
+msgstr ""
+
 msgid "Topic"
 msgstr ""
 
 msgid "Topics"
 msgstr ""
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -278,14 +284,20 @@
 
 msgid "Allow re-voting?"
 msgstr ""
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
+msgid "Hide results?"
+msgstr ""
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr ""
 
 msgid "Comment"
@@ -302,14 +314,17 @@
 
 msgid "Poll duration, in days"
 msgstr ""
 
 msgid "Allow vote changes"
 msgstr ""
 
+msgid "Hide results"
+msgstr ""
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -593,18 +608,18 @@
 
 msgid "Topics have been marked read."
 msgstr ""
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
 msgstr ""
 
-msgid "Update date"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
@@ -791,14 +806,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr ""
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr ""
 
 msgid "Submit"
 msgstr ""
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/ru/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/ru/LC_MESSAGES/django.mo`

 * *Files 0% similar despite different names*

#### msgunfmt {}

```diff
@@ -2,18 +2,18 @@
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
 "PO-Revision-Date: 2019-12-16 08:00+0000\n"
 "Last-Translator: Emelyan Marakhovsky <savelmtr@gmail.com>\n"
 "Language-Team: Russian (http://www.transifex.com/django-machina-team/django-"
 "machina/language/ru/)\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && "
 "n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || "
 "(n%100>=11 && n%100<=14)? 2 : 3);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "%(counter)s post found"
 msgid_plural "%(counter)s posts found"
```

### Comparing `django-machina-1.2.0/machina/locale/ru/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/ru/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -1,28 +1,28 @@
 # SOME DESCRIPTIVE TITLE.
 # Copyright (C) YEAR THE PACKAGE'S COPYRIGHT HOLDER
 # This file is distributed under the same license as the PACKAGE package.
-# 
+#
 # Translators:
 # alexander fedorov <elf607@gmail.com>, 2017
 # georgekpg <konstantinpopov@inbox.ru>, 2018
 # Emelyan Marakhovsky <savelmtr@gmail.com>, 2019
 # Za Ars <zaars.progger@gmail.com>, 2018
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-12-16 08:00+0000\n"
 "Last-Translator: Emelyan Marakhovsky <savelmtr@gmail.com>\n"
 "Language-Team: Russian (http://www.transifex.com/django-machina-team/django-machina/language/ru/)\n"
+"Language: ru\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Language: ru\n"
 "Plural-Forms: nplurals=4; plural=(n%10==1 && n%100!=11 ? 0 : n%10>=2 && n%10<=4 && (n%100<12 || n%100>14) ? 1 : n%10==0 || (n%10>=5 && n%10<=9) || (n%100>=11 && n%100<=14)? 2 : 3);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
 msgstr "Родитель"
 
 msgid "Name"
@@ -69,16 +69,15 @@
 
 msgid "Last post added on"
 msgstr "Последний ответ добавлен в"
 
 msgid "Display in parent-forums legend"
 msgstr "Отображать в легенде родительских форумов"
 
-msgid ""
-"Displays this forum on the legend of its parent-forum (sub forums list)"
+msgid "Displays this forum on the legend of its parent-forum (sub forums list)"
 msgstr "Показывать этот форум в легенде родительского форума (списке подфорумов)"
 
 msgid "Forum"
 msgstr "Форум"
 
 msgid "Forums"
 msgstr "Форумы"
@@ -127,30 +126,24 @@
 
 msgid "Machina: Forum"
 msgstr "Machina: Форум"
 
 msgid "Anonymous"
 msgstr "Аноним"
 
-msgid ""
-"Please select this option if you want to edit the permissions of the "
-"anonymous user"
+msgid "Please select this option if you want to edit the permissions of the anonymous user"
 msgstr "Выберите этот вариант, если вы хотите отредактировать разрешения анонимного пользоватея"
 
 msgid "Authenticated"
 msgstr "Зарегистрированный"
 
-msgid ""
-"Please select this option if you want to edit the permissions of every (non-"
-"specific) logged in user"
+msgid "Please select this option if you want to edit the permissions of every (non-specific) logged in user"
 msgstr "Выберите этот вариант, если вы хотите отредактировать разрешения для всех зарегистрированных пользователей "
 
-msgid ""
-"Choose either a user ID or check either the anonymous or authenticated user "
-"checkbox"
+msgid "Choose either a user ID or check either the anonymous or authenticated user checkbox"
 msgstr "Выберите ID конкретного пользователя или поставьте галочку в соответствующем чекбоксе, чтобы настроить разрешения для анонимных или зарегистрированных пользователей"
 
 msgid "Not set"
 msgstr "Не установлено"
 
 msgid "Granted"
 msgstr "Предоставлено"
@@ -202,14 +195,20 @@
 
 msgid "First post"
 msgstr "Первый ответ"
 
 msgid "Subscribers"
 msgstr "Подписчики"
 
+msgid "Creation date"
+msgstr "Дата создания"
+
+msgid "Update date"
+msgstr "Дата обновления"
+
 msgid "Topic"
 msgstr "Тема"
 
 msgid "Topics"
 msgstr "Темы"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -241,16 +240,15 @@
 
 msgid "Posts"
 msgstr "Ответы"
 
 msgid "A user id or an anonymous key must be associated with a post."
 msgstr "Пользовательский ID или ключ анонимного пользователя должен быть связан с ответом"
 
-msgid ""
-"A user id or an anonymous key must be associated with a post, but not both."
+msgid "A user id or an anonymous key must be associated with a post, but not both."
 msgstr "Пользовательский ID или ключ анонимного пользователя должен быть связан с ответом, но не оба одновременно"
 
 msgid "A username must be specified if the poster is anonymous"
 msgstr "Имя пользователя должно быть указано, если автор - анонимный пользователь"
 
 msgid "Machina: Forum conversations"
 msgstr "Machina: Беседы форума"
@@ -269,17 +267,15 @@
 
 msgid "Post topic as"
 msgstr "Создать тему под"
 
 msgid "Poll question"
 msgstr "Добавить вариант опроса"
 
-msgid ""
-"Enter a question to associate a poll with the topic or leave blank to not "
-"create a poll."
+msgid "Enter a question to associate a poll with the topic or leave blank to not create a poll."
 msgstr "Введите вариант, чтобы создать опрос в теме, или оставьте пустым, чтобы не создавать опрос"
 
 msgid "Maximum number of poll options per user"
 msgstr "Максимальное количество вариантов для пользователя."
 
 msgid "This is the number of options each user may select when voting."
 msgstr "Это количество вариантов, которые пользователь сможет выбрать при голосовании."
@@ -292,16 +288,23 @@
 
 msgid "Allow re-voting?"
 msgstr "Позволить голосовать заново?"
 
 msgid "If enabled users are able to change their vote."
 msgstr "Если отмечено, пользователи будут иметь возможность изменить своё выбор."
 
-msgid ""
-"You must set the maximum number of poll options per user when creating polls"
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Посмотреть результаты"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
+msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "Вы должны установить максимальное количество вариантов, которые может выбрать пользователь, когда создаёте опрос"
 
 msgid "File"
 msgstr "Файл"
 
 msgid "Comment"
 msgstr "Комментарий"
@@ -317,14 +320,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Продолжительность опроса в днях"
 
 msgid "Allow vote changes"
 msgstr "Позволить изменение выбора"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Посмотреть результаты"
+
 msgid "Topic poll"
 msgstr "Опрос темы"
 
 msgid "Topic polls"
 msgstr "Опросы темы"
 
 msgid "Poll"
@@ -485,17 +493,15 @@
 
 msgid "User forum permission"
 msgstr "Разрешение пользователя форума"
 
 msgid "User forum permissions"
 msgstr "Разрешения пользователя форума"
 
-msgid ""
-"A permission should target either a specific user, an anonymous user or any "
-"authenticated user"
+msgid "A permission should target either a specific user, an anonymous user or any authenticated user"
 msgstr "Для разрешения следует указать цель - конкретный пользователь, анонимный пользователь или все зарегистрированные пользователи"
 
 msgid "Group"
 msgstr "Группа"
 
 msgid "Group forum permission"
 msgstr "Разрешение группы форума"
@@ -610,40 +616,40 @@
 
 msgid "Topics have been marked read."
 msgstr "Темы были отмечены как прочитанные."
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "Ни Pillow, ни PIL не могут быть импортированы: {}"
 
-msgid "Creation date"
-msgstr "Дата создания"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "Невозможно импортировать MACHINA_MARKUP_LANGUAGE {}: {}"
 
-msgid "Update date"
-msgstr "Дата обновления"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "Настройка MACHINA_MARKUP_LANGUAGE обязательна "
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "Невозможно импортировать MACHINA_MARKUP_WIDGET {}: {}"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "Невозможно импортировать MACHINA_MARKUP_LANGUAGE {}: {}"
 
 msgid "MACHINA_MARKUP_LANGUAGE setting is required"
 msgstr "Настройка MACHINA_MARKUP_LANGUAGE обязательна "
 
 msgid "Files of size greater than {} are not allowed. Your file is {}"
 msgstr "Файлы размера больше чем {} не доступны для загрузки. Ваш файл {}"
 
-msgid ""
-"Images of width lesser than {}px or greater than {}px or are not allowed. "
-"The width of your image is {}px"
+msgid "Images of width lesser than {}px or greater than {}px or are not allowed. The width of your image is {}px"
 msgstr "Изображения имеют ширину меньше {}px, больше {}px или не разрешены. Ширина вашего изображения: {}px"
 
-msgid ""
-"Images of height lesser than {}px or greater than {}px or are not allowed. "
-"The height of your image is {}px"
+msgid "Images of height lesser than {}px or greater than {}px or are not allowed. The height of your image is {}px"
 msgstr "Изображения имеют высоту меньше {}px, больше {}px или не разрешены. Высота вашего изображения: {}px"
 
 msgid "List of forums"
 msgstr "Список форумов"
 
 msgid "Quick actions"
 msgstr "Быстрые действия"
@@ -707,17 +713,15 @@
 
 msgid "Please select a group in order to update its permissions"
 msgstr "Выберите группу, чтобы обновить ее разрешения"
 
 msgid "Copy permissions from another forum"
 msgstr "Скопировать разрешения из другого форума"
 
-msgid ""
-"Please select a forum in order to copy its permissions configuration to the "
-"current forum"
+msgid "Please select a forum in order to copy its permissions configuration to the current forum"
 msgstr "Выберите форум, чтобы скопировать его параметры разрешений в текущий форум "
 
 msgid "Copy"
 msgstr "Скопировать"
 
 msgid "Search"
 msgstr "Поиск"
@@ -808,22 +812,23 @@
 
 msgid "Poll options"
 msgstr "Варианты опроса"
 
 msgid "Add a poll option"
 msgstr "Добавить вариант опроса"
 
-msgid ""
-"<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the "
-"associated votes."
+msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "<b>Внимание:</b>&nbsp;Удаление варианта из существующего опроса удалит и связанные с ним голоса. "
 
 msgid "Preview:"
 msgstr "Предпросмотр:"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Всего голосов:"
 
 msgid "Submit"
 msgstr "Отправить"
 
 msgid "View results"
@@ -945,30 +950,46 @@
 #, python-format
 msgid ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Post</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Posts</small></p>"
-msgstr[0] "<h2><strong>%(counter)s</strong></h2>\n<p><small>Ответ</small></p>"
-msgstr[1] "<h2><strong>%(counter)s</strong></h2>\n<p><small>Ответа</small></p>"
-msgstr[2] "<h2><strong>%(counter)s</strong></h2>\n<p><small>Ответов</small></p>"
-msgstr[3] "<h2><strong>%(counter)s</strong></h2>\n<p class=\"mb-1\"><small>Ответов</small></p>"
+msgstr[0] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p><small>Ответ</small></p>"
+msgstr[1] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p><small>Ответа</small></p>"
+msgstr[2] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p><small>Ответов</small></p>"
+msgstr[3] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p class=\"mb-1\"><small>Ответов</small></p>"
 
 #, python-format
 msgid ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Topic</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Topics</small></p>"
-msgstr[0] "<h2><strong>%(counter)s</strong></h2>\n<p><small>Тема</small></p>"
-msgstr[1] "<h2><strong>%(counter)s</strong></h2>\n<p class=\"mb-1\"><small>Темы</small></p>"
-msgstr[2] "<h2><strong>%(counter)s</strong></h2>\n<p class=\"mb-1\"><small>Тем</small></p>"
-msgstr[3] "<h2><strong>%(counter)s</strong></h2>\n<p class=\"mb-1\"><small>Тем</small></p>"
+msgstr[0] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p><small>Тема</small></p>"
+msgstr[1] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p class=\"mb-1\"><small>Темы</small></p>"
+msgstr[2] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p class=\"mb-1\"><small>Тем</small></p>"
+msgstr[3] ""
+"<h2><strong>%(counter)s</strong></h2>\n"
+"<p class=\"mb-1\"><small>Тем</small></p>"
 
 msgid "Recent posts"
 msgstr "Последние ответы"
 
 msgid "View all"
 msgstr "Просмотреть все"
 
@@ -1051,16 +1072,15 @@
 
 msgid "Are you sure you want to approve this post?"
 msgstr "Вы уверены, что хотите одобрить этот ответ?"
 
 msgid "Disapprove post"
 msgstr "Отклонить ответ"
 
-msgid ""
-"Are you sure you want to disapprove this post? This post will be deleted."
+msgid "Are you sure you want to disapprove this post? This post will be deleted."
 msgstr "Вы уверены. что хотите отклонить этот ответ?"
 
 msgid "Are you sure you want to delete this topic?"
 msgstr "Вы уверены, что хотите удалить эту тему?"
 
 msgid "Are you sure you want to lock this topic?"
 msgstr "Вы уверены, что хотите заблокировать эту тему?"
```

### Comparing `django-machina-1.2.0/machina/locale/sl_SI/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/sl_SI/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/sl_SI/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/sl_SI/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # Miha Frangež <miha.frangez@gmail.com>, 2016-2017
 # Miha Frangež <miha.frangez@gmail.com>, 2016
 # Miha Frangež <miha.frangez@gmail.com>, 2018
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: Slovenian (Slovenia) (http://www.transifex.com/django-machina-team/django-machina/language/sl_SI/)\n"
 "Language: sl_SI\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -194,14 +194,20 @@
 
 msgid "First post"
 msgstr "Prva objava"
 
 msgid "Subscribers"
 msgstr "Naročniki"
 
+msgid "Creation date"
+msgstr "Datum nastanka"
+
+msgid "Update date"
+msgstr "Datum spremembe"
+
 msgid "Topic"
 msgstr "Tema"
 
 msgid "Topics"
 msgstr "Teme"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -281,14 +287,22 @@
 
 msgid "Allow re-voting?"
 msgstr "Dovolote ponovno glasovanje"
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "Poglej rezultate"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr "Datoteka"
 
 msgid "Comment"
@@ -305,14 +319,19 @@
 
 msgid "Poll duration, in days"
 msgstr "Trajanje ankete, v dnevih"
 
 msgid "Allow vote changes"
 msgstr "Dovoli spremembe glasov"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "Poglej rezultate"
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -596,19 +615,19 @@
 
 msgid "Topics have been marked read."
 msgstr "Objave označene kot prebrane"
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
-msgstr "Datum nastanka"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr ""
 
-msgid "Update date"
-msgstr "Datum spremembe"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
 
@@ -794,14 +813,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr "Predogled:"
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "Število glasov:"
 
 msgid "Submit"
 msgstr "Pošlji"
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/zh/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/zh_TW/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,19 +3,19 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
-"Language-Team: Chinese (http://www.transifex.com/django-machina-team/django-machina/language/zh/)\n"
-"Language: zh\n"
+"Language-Team: Chinese (Taiwan) (http://www.transifex.com/django-machina-team/django-machina/language/zh_TW/)\n"
+"Language: zh_TW\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
 "Plural-Forms: nplurals=1; plural=0;\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
@@ -191,14 +191,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr ""
 
+msgid "Creation date"
+msgstr ""
+
+msgid "Update date"
+msgstr ""
+
 msgid "Topic"
 msgstr ""
 
 msgid "Topics"
 msgstr ""
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -278,14 +284,20 @@
 
 msgid "Allow re-voting?"
 msgstr ""
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
+msgid "Hide results?"
+msgstr ""
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr ""
 
 msgid "Comment"
@@ -302,14 +314,17 @@
 
 msgid "Poll duration, in days"
 msgstr ""
 
 msgid "Allow vote changes"
 msgstr ""
 
+msgid "Hide results"
+msgstr ""
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -593,18 +608,18 @@
 
 msgid "Topics have been marked read."
 msgstr ""
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
 msgstr ""
 
-msgid "Update date"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
@@ -791,14 +806,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr ""
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr ""
 
 msgid "Submit"
 msgstr ""
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/zh_CN/LC_MESSAGES/django.mo` & `django_machina-1.3.0/machina/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/locale/zh_CN/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files 2% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 # yanceyy <20135224@stu.neu.edu.cn>, 2016
 # Neo Chang <me@neoto.xin>, 2017
 # yanceyy <20135224@stu.neu.edu.cn>, 2016
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
 "Language-Team: Chinese (China) (http://www.transifex.com/django-machina-team/django-machina/language/zh_CN/)\n"
 "Language: zh_CN\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
@@ -194,14 +194,20 @@
 
 msgid "First post"
 msgstr "首帖"
 
 msgid "Subscribers"
 msgstr "订阅者"
 
+msgid "Creation date"
+msgstr "创建日期"
+
+msgid "Update date"
+msgstr "更新日期"
+
 msgid "Topic"
 msgstr "话题"
 
 msgid "Topics"
 msgstr "话题"
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -281,14 +287,22 @@
 
 msgid "Allow re-voting?"
 msgstr "允许重新投票？"
 
 msgid "If enabled users are able to change their vote."
 msgstr "是否授权给用户更改他们的投票"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results?"
+msgstr "显示结果"
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr "创建投票时，你必须设置每个用户可选择的最大投票选项数"
 
 msgid "File"
 msgstr "文件"
 
 msgid "Comment"
@@ -305,14 +319,19 @@
 
 msgid "Poll duration, in days"
 msgstr "投票持续时间"
 
 msgid "Allow vote changes"
 msgstr "允许更改投票"
 
+#, fuzzy
+#| msgid "View results"
+msgid "Hide results"
+msgstr "显示结果"
+
 msgid "Topic poll"
 msgstr "话题投票"
 
 msgid "Topic polls"
 msgstr "话题投票"
 
 msgid "Poll"
@@ -596,19 +615,23 @@
 
 msgid "Topics have been marked read."
 msgstr "话题已标记已读"
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr "缺乏相关变量"
 
-msgid "Creation date"
-msgstr "创建日期"
+#, fuzzy
+#| msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
+msgstr "不能输入 MACHINA_MARKUP_LANGUAGE"
 
-msgid "Update date"
-msgstr "更新日期"
+#, fuzzy
+#| msgid "MACHINA_MARKUP_LANGUAGE setting is required"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
+msgstr "MACHINA_MARKUP_LANGUAGE符合设定要求"
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr "不能输入 MACHINA_MARKUP_WIDGET"
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr "不能输入 MACHINA_MARKUP_LANGUAGE"
 
@@ -794,14 +817,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr "删除已存在的投票选项将会一并删除相关投票数"
 
 msgid "Preview:"
 msgstr "概要："
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr "总投票数："
 
 msgid "Submit"
 msgstr "提交"
 
 msgid "View results"
```

### Comparing `django-machina-1.2.0/machina/locale/zh_TW/LC_MESSAGES/django.po` & `django_machina-1.3.0/machina/locale/it/LC_MESSAGES/django.po`

 * *Files 1% similar despite different names*

```diff
@@ -3,23 +3,23 @@
 # This file is distributed under the same license as the PACKAGE package.
 #
 # Translators:
 msgid ""
 msgstr ""
 "Project-Id-Version: django-machina\n"
 "Report-Msgid-Bugs-To: \n"
-"POT-Creation-Date: 2019-11-16 17:35-0500\n"
+"POT-Creation-Date: 2023-02-19 16:58-0500\n"
 "PO-Revision-Date: 2019-10-29 01:36+0000\n"
 "Last-Translator: Morgan Aubert <morgan@aubert.email>\n"
-"Language-Team: Chinese (Taiwan) (http://www.transifex.com/django-machina-team/django-machina/language/zh_TW/)\n"
-"Language: zh_TW\n"
+"Language-Team: Italian (http://www.transifex.com/django-machina-team/django-machina/language/it/)\n"
+"Language: it\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=UTF-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Plural-Forms: nplurals=1; plural=0;\n"
+"Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "X-Generator: Poedit 1.8.4\n"
 
 msgid "Parent"
 msgstr ""
 
 msgid "Name"
 msgstr ""
@@ -191,14 +191,20 @@
 
 msgid "First post"
 msgstr ""
 
 msgid "Subscribers"
 msgstr ""
 
+msgid "Creation date"
+msgstr ""
+
+msgid "Update date"
+msgstr ""
+
 msgid "Topic"
 msgstr ""
 
 msgid "Topics"
 msgstr ""
 
 msgid "A topic can not be associated with a category or a link forum"
@@ -278,14 +284,20 @@
 
 msgid "Allow re-voting?"
 msgstr ""
 
 msgid "If enabled users are able to change their vote."
 msgstr ""
 
+msgid "Hide results?"
+msgstr ""
+
+msgid "If enabled results are hidden to everyone except topic creator."
+msgstr ""
+
 msgid "You must set the maximum number of poll options per user when creating polls"
 msgstr ""
 
 msgid "File"
 msgstr ""
 
 msgid "Comment"
@@ -302,14 +314,17 @@
 
 msgid "Poll duration, in days"
 msgstr ""
 
 msgid "Allow vote changes"
 msgstr ""
 
+msgid "Hide results"
+msgstr ""
+
 msgid "Topic poll"
 msgstr ""
 
 msgid "Topic polls"
 msgstr ""
 
 msgid "Poll"
@@ -593,18 +608,18 @@
 
 msgid "Topics have been marked read."
 msgstr ""
 
 msgid "Neither Pillow nor PIL could be imported: {}"
 msgstr ""
 
-msgid "Creation date"
+msgid "Could not import MACHINA MARKUP_MAX_LENGTH_VALIDATOR {}: {}"
 msgstr ""
 
-msgid "Update date"
+msgid "MACHINA_MARKUP_MAX_LENGTH_VALIDATOR setting is required"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_WIDGET {}: {}"
 msgstr ""
 
 msgid "Could not import MACHINA_MARKUP_LANGUAGE {}: {}"
 msgstr ""
@@ -791,14 +806,17 @@
 
 msgid "<b>Note:</b>&nbsp;Deleting poll options of an existing poll will delete the associated votes."
 msgstr ""
 
 msgid "Preview:"
 msgstr ""
 
+msgid "Results are currently hidden."
+msgstr ""
+
 msgid "Total votes:"
 msgstr ""
 
 msgid "Submit"
 msgstr ""
 
 msgid "View results"
@@ -881,14 +899,15 @@
 msgid "on"
 msgstr ""
 
 #, python-format
 msgid "edited %(counter)s time in total."
 msgid_plural "edited %(counter)s times in total."
 msgstr[0] ""
+msgstr[1] ""
 
 msgid "Reason:"
 msgstr ""
 
 msgid "Replies"
 msgstr ""
 
@@ -918,23 +937,25 @@
 msgid ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Post</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Posts</small></p>"
 msgstr[0] ""
+msgstr[1] ""
 
 #, python-format
 msgid ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p><small>Topic</small></p>"
 msgid_plural ""
 "<h2><strong>%(counter)s</strong></h2>\n"
 "                      <p class=\"mb-1\"><small>Topics</small></p>"
 msgstr[0] ""
+msgstr[1] ""
 
 msgid "Recent posts"
 msgstr ""
 
 msgid "View all"
 msgstr ""
 
@@ -948,14 +969,15 @@
 msgid "Topics that you are subscribed to"
 msgstr ""
 
 #, python-format
 msgid "%(counter)s topic found"
 msgid_plural "%(counter)s topics found"
 msgstr[0] ""
+msgstr[1] ""
 
 msgid "Not topics found."
 msgstr ""
 
 msgid "Subscribe to topic"
 msgstr ""
 
@@ -975,14 +997,15 @@
 msgid "%(username)s's posts"
 msgstr ""
 
 #, python-format
 msgid "%(counter)s post found"
 msgid_plural "%(counter)s posts found"
 msgstr[0] ""
+msgstr[1] ""
 
 msgid "No posts found"
 msgstr ""
 
 msgid "Disapprove"
 msgstr ""
 
@@ -1036,14 +1059,15 @@
 msgid "New search"
 msgstr ""
 
 #, python-format
 msgid "Your search has returned <b>%(number_of_results)s</b> result"
 msgid_plural "Your search has returned <b>%(number_of_results)s</b> results"
 msgstr[0] ""
+msgstr[1] ""
 
 msgid "Results"
 msgstr ""
 
 msgid "No results."
 msgstr ""
 
@@ -1053,13 +1077,14 @@
 msgid "Are you sure you want to mark topics read?"
 msgstr ""
 
 #, python-format
 msgid "%(topic_length)s unread topic found"
 msgid_plural "%(topic_length)s unread topics found"
 msgstr[0] ""
+msgstr[1] ""
 
 msgid "There are no unread topics."
 msgstr ""
 
 msgid "Forum index"
 msgstr ""
```

### Comparing `django-machina-1.2.0/machina/models/fields.py` & `django_machina-1.3.0/machina/models/fields.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/css/machina.admin_theme.min.css` & `django_machina-1.3.0/machina/static/machina/build/css/machina.admin_theme.min.css`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/css/machina.board_theme.min.css` & `django_machina-1.3.0/machina/static/machina/build/css/machina.board_theme.min.css`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/css/machina.board_theme.vendor.min.css` & `django_machina-1.3.0/machina/static/machina/build/css/machina.board_theme.vendor.min.css`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/css/vendor/easymde.min.css` & `django_machina-1.3.0/machina/static/machina/build/css/vendor/easymde.min.css`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.eot` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.eot`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.svg` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.svg`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.ttf` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.ttf`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.woff` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.woff`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-brands-400.woff2` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-brands-400.woff2`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.eot` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.eot`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.svg` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.svg`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.ttf` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.ttf`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.woff` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.woff`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-regular-400.woff2` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-regular-400.woff2`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.eot` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.eot`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.svg` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.svg`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.ttf` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.ttf`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.woff` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.woff`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/fonts/fa-solid-900.woff2` & `django_machina-1.3.0/machina/static/machina/build/fonts/fa-solid-900.woff2`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/js/machina.editor.min.js` & `django_machina-1.3.0/machina/static/machina/build/js/machina.editor.min.js`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/js/machina.min.js` & `django_machina-1.3.0/machina/static/machina/build/js/machina.min.js`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/js/machina.packages.min.js` & `django_machina-1.3.0/machina/static/machina/build/js/machina.packages.min.js`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/build/js/vendor/easymde.min.js` & `django_machina-1.3.0/machina/static/machina/build/js/vendor/easymde.min.js`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/js/editor.js` & `django_machina-1.3.0/machina/static/machina/js/editor.js`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/js/ui.js` & `django_machina-1.3.0/machina/static/machina/js/ui.js`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/admin_pages/forum_permissions.scss` & `django_machina-1.3.0/machina/static/machina/sass/admin_pages/forum_permissions.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/admin_theme.scss` & `django_machina-1.3.0/machina/static/machina/sass/admin_theme.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/board_pages/conversation_post_edit.scss` & `django_machina-1.3.0/machina/static/machina/sass/board_pages/conversation_post_edit.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/board_pages/conversation_topic_detail.scss` & `django_machina-1.3.0/machina/static/machina/sass/board_pages/conversation_topic_detail.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/board_pages/forum_detail.scss` & `django_machina-1.3.0/machina/static/machina/sass/board_pages/forum_detail.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/board_pages/forum_lists.scss` & `django_machina-1.3.0/machina/static/machina/sass/board_pages/forum_lists.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/board_pages/member_profile.scss` & `django_machina-1.3.0/machina/static/machina/sass/board_pages/member_profile.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/board_pages/moderation.scss` & `django_machina-1.3.0/machina/static/machina/sass/board_pages/moderation.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/board_pages/search.scss` & `django_machina-1.3.0/machina/static/machina/sass/board_pages/search.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/static/machina/sass/variables.scss` & `django_machina-1.3.0/machina/static/machina/sass/variables.scss`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/admin/forum/forum/change_list.html` & `django_machina-1.3.0/machina/templates/admin/forum/forum/change_list.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/admin/forum/forum/change_list_table.html` & `django_machina-1.3.0/machina/templates/admin/forum/forum/change_list_table.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/admin/forum/forum/editpermissions_form.html` & `django_machina-1.3.0/machina/templates/admin/forum/forum/editpermissions_form.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/admin/forum/forum/editpermissions_index.html` & `django_machina-1.3.0/machina/templates/admin/forum/forum/editpermissions_index.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/_base.html` & `django_machina-1.3.0/machina/templates/machina/_base.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/board_base.html` & `django_machina-1.3.0/machina/templates/machina/board_base.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum/forum_detail.html` & `django_machina-1.3.0/machina/templates/machina/forum/forum_detail.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum/forum_list.html` & `django_machina-1.3.0/machina/templates/machina/forum/forum_list.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum/index.html` & `django_machina-1.3.0/machina/templates/machina/forum/index.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_attachments/attachment_formset.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_attachments/attachment_formset.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_attachments/attachments_detail.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_attachments/attachments_detail.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_attachments/attachments_preview.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_attachments/attachments_preview.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_detail.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_detail.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_option_formset.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_option_formset.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_preview.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_preview.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_results.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_results.html`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,17 @@
 {% load i18n %}
+{% load forum_permission_tags %}
 
+{% get_permission 'can_edit_post' poll.topic.first_post request.user as user_can_edit_first_post %}
+
+{% if poll.hide_results %}
+    {% trans "Results are currently hidden." %}<br><br>
+{% endif %}
+
+{% if not poll.hide_results or user_can_edit_first_post %}
 {% for option in poll.options.all %}
 {% if forloop.first or not forloop.counter|divisibleby:2 %}
 <div class="mb-3 row">
 {% endif %}
 <div class="col-md-6">
   <b>{{ option.text }}</b>
   <div class="progress">
@@ -12,8 +20,10 @@
     </div>
   </div>
 </div>
 {% if forloop.last or forloop.counter|divisibleby:2 %}
 </div>
 {% endif %}
 {% endfor %}
+{% endif %}
+
 {% trans "Total votes:" %}&nbsp;{{ poll.votes|length }}
```

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/forum_polls/poll_vote_form.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/forum_polls/poll_vote_form.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/partials/post_form.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/partials/post_form.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/partials/topic_detail_actions.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/partials/topic_detail_actions.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/partials/topic_form.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/partials/topic_form.html`

 * *Files 6% similar despite different names*

```diff
@@ -69,14 +69,22 @@
               <div class="checkbox">
                 <label for="{{ post_form.poll_user_changes.auto_id }}">
                   {{ post_form.poll_user_changes }}
                   {{ post_form.poll_user_changes.label }}
                 </label>
               </div>
             </div>
+            <div{% if post_form.poll_hide_results.errors %} class="has-error"{% endif %}>
+              <div class="checkbox">
+                <label for="{{ post_form.poll_hide_results.auto_id }}">
+                  {{ post_form.poll_hide_results }}
+                  {{ post_form.poll_hide_results.label }}
+                </label>
+              </div>
+            </div>
           </div>
           <div id="poll_formset" class="col-md-6">
             {% include "forum_conversation/forum_polls/poll_option_formset.html" %}
           </div>
         </div>
       </div>
     </div>
```

#### html2text {}

```diff
@@ -28,14 +28,16 @@
 {{ poll_option_formset.non_form_errors|striptags }}
 {% endif %}
 {% include "partials/form_field.html" with field=post_form.poll_question %} {%
 include "partials/form_field.html" with field=post_form.poll_max_options %} {%
 include "partials/form_field.html" with field=post_form.poll_duration %}
 % if post_form.poll_user_changes.errors %} class="has-error"{% endif %}>
  {{ post_form.poll_user_changes }} {{ post_form.poll_user_changes.label }}
+% if post_form.poll_hide_results.errors %} class="has-error"{% endif %}>
+ {{ post_form.poll_hide_results }} {{ post_form.poll_hide_results.label }}
 {% include "forum_conversation/forum_polls/poll_option_formset.html" %}
 {% endif %} {% if attachment_formset %}
 
 {% include "forum_conversation/forum_attachments/attachment_formset.html" %}
 {% endif %}
  %}" /> 
  %}" />
```

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/post_create.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/post_create.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/post_delete.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/post_delete.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/post_preview.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/post_preview.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/post_update.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/post_update.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_create.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_create.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_detail.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_detail.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_list.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_list.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_pages_inline_list.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_pages_inline_list.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_conversation/topic_update.html` & `django_machina-1.3.0/machina/templates/machina/forum_conversation/topic_update.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_member/forum_profile_detail.html` & `django_machina-1.3.0/machina/templates/machina/forum_member/forum_profile_detail.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_member/forum_profile_update.html` & `django_machina-1.3.0/machina/templates/machina/forum_member/forum_profile_update.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_member/subscription_topic_list.html` & `django_machina-1.3.0/machina/templates/machina/forum_member/subscription_topic_list.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_member/topic_subscribe.html` & `django_machina-1.3.0/machina/templates/machina/forum_member/topic_subscribe.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_member/topic_unsubscribe.html` & `django_machina-1.3.0/machina/templates/machina/forum_member/topic_unsubscribe.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_member/user_posts_list.html` & `django_machina-1.3.0/machina/templates/machina/forum_member/user_posts_list.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_moderation/moderation_queue/detail.html` & `django_machina-1.3.0/machina/templates/machina/forum_moderation/moderation_queue/detail.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_moderation/moderation_queue/list.html` & `django_machina-1.3.0/machina/templates/machina/forum_moderation/moderation_queue/list.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_moderation/moderation_queue/post_approve.html` & `django_machina-1.3.0/machina/templates/machina/forum_moderation/moderation_queue/post_approve.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_moderation/moderation_queue/post_disapprove.html` & `django_machina-1.3.0/machina/templates/machina/forum_moderation/moderation_queue/post_disapprove.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_delete.html` & `django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_delete.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_lock.html` & `django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_lock.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_move.html` & `django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_move.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_unlock.html` & `django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_unlock.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_moderation/topic_update_type.html` & `django_machina-1.3.0/machina/templates/machina/forum_moderation/topic_update_type.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_search/pagination.html` & `django_machina-1.3.0/machina/templates/machina/forum_search/pagination.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_search/search.html` & `django_machina-1.3.0/machina/templates/machina/forum_search/search.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_tracking/mark_forums_read.html` & `django_machina-1.3.0/machina/templates/machina/forum_tracking/mark_forums_read.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_tracking/mark_topics_read.html` & `django_machina-1.3.0/machina/templates/machina/forum_tracking/mark_topics_read.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/forum_tracking/unread_topic_list.html` & `django_machina-1.3.0/machina/templates/machina/forum_tracking/unread_topic_list.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/partials/breadcrumb.html` & `django_machina-1.3.0/machina/templates/machina/partials/breadcrumb.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/partials/form_field.html` & `django_machina-1.3.0/machina/templates/machina/partials/form_field.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templates/machina/partials/pagination.html` & `django_machina-1.3.0/machina/templates/machina/partials/pagination.html`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templatetags/forum_conversation_tags.py` & `django_machina-1.3.0/machina/templatetags/forum_conversation_tags.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templatetags/forum_permission_tags.py` & `django_machina-1.3.0/machina/templatetags/forum_permission_tags.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templatetags/forum_polls_tags.py` & `django_machina-1.3.0/machina/templatetags/forum_polls_tags.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templatetags/forum_tags.py` & `django_machina-1.3.0/machina/templatetags/forum_tags.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/templatetags/forum_tracking_tags.py` & `django_machina-1.3.0/machina/templatetags/forum_tracking_tags.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/test/context_managers.py` & `django_machina-1.3.0/machina/test/context_managers.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/test/factories/auth.py` & `django_machina-1.3.0/machina/test/factories/auth.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/test/factories/conversation.py` & `django_machina-1.3.0/machina/test/factories/conversation.py`

 * *Files 12% similar despite different names*

```diff
@@ -25,15 +25,15 @@
     class Meta:
         model = Topic
 
 
 class PostFactory(factory.django.DjangoModelFactory):
     topic = factory.SubFactory(TopicFactory)
     poster = factory.SubFactory(UserFactory)
-    subject = factory.LazyAttribute(lambda t: faker.text(max_nb_chars=200))
+    subject = factory.LazyAttribute(lambda t: faker.sentence()[:200])
     content = fuzzy.FuzzyText(length=255)
 
     class Meta:
         model = Post
 
 
 def build_topic(**attrs):
```

### Comparing `django-machina-1.2.0/machina/test/factories/forum.py` & `django_machina-1.3.0/machina/test/factories/forum.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/test/factories/permission.py` & `django_machina-1.3.0/machina/test/factories/permission.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/test/factories/polls.py` & `django_machina-1.3.0/machina/test/factories/polls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/test/factories/tracking.py` & `django_machina-1.3.0/machina/test/factories/tracking.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/test/mixins.py` & `django_machina-1.3.0/machina/test/mixins.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/test/testcases.py` & `django_machina-1.3.0/machina/test/testcases.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/machina/urls.py` & `django_machina-1.3.0/machina/urls.py`

 * *Files identical despite different names*

### Comparing `django-machina-1.2.0/pyproject.toml` & `django_machina-1.3.0/pyproject.toml`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "django-machina"
-version = "1.2.0"
+version = "1.3.0"
 description = "A Django forum engine for building powerful community driven websites."
 authors = ["Morgan Aubert <me@morganaubert.name>"]
 license = "BSD-3-Clause"
 readme = "README.rst"
 homepage = "https://github.com/ellmetha/django-machina"
 repository = "https://github.com/ellmetha/django-machina"
 keywords = ["django", "forum", "board", "messages"]
@@ -18,14 +18,15 @@
     'Programming Language :: Python',
     'Programming Language :: Python :: 3',
     'Programming Language :: Python :: 3.6',
     'Programming Language :: Python :: 3.7',
     'Programming Language :: Python :: 3.8',
     'Programming Language :: Python :: 3.9',
     'Programming Language :: Python :: 3.10',
+    'Programming Language :: Python :: 3.11',
     'Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Message Boards',
 ]
 packages = [
     { include = "machina" },
 ]
 include = [
     "AUTHORS",
@@ -45,28 +46,27 @@
 django-haystack = ">=2.1"
 django-mptt = ">=0.10.0"
 django-widget-tweaks = ">=1.4"
 markdown2 = ">=2.3"
 pillow = ">=2.2"
 
 [tool.poetry.dev-dependencies]
-codecov = "*"
 django-debug-toolbar = "*"
 factory-boy = "*"
 faker = "*"
 flake8 = "*"
 ipython = "*"
 isort = "*"
 mock = "*"
 pytest = ">=6.2.5"
 pytest-cov = "*"
 pytest-django = "*"
 pytest-pythonpath = "*"
 pytest-spec = "*"
 pytest-xdist = "*"
-sphinx = "*"
+sphinx = ">= 4.2"
 sphinx-rtd-theme = "*"
 whoosh = "*"
 
 [build-system]
 requires = ["poetry>=0.12"]
 build-backend = "poetry.masonry.api"
```

### Comparing `django-machina-1.2.0/PKG-INFO` & `django_machina-1.3.0/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: django-machina
-Version: 1.2.0
+Version: 1.3.0
 Summary: A Django forum engine for building powerful community driven websites.
 Home-page: https://github.com/ellmetha/django-machina
 License: BSD-3-Clause
 Keywords: django,forum,board,messages
 Author: Morgan Aubert
 Author-email: me@morganaubert.name
 Requires-Python: >=3.6,<4.0
@@ -12,29 +12,38 @@
 Classifier: Environment :: Web Environment
 Classifier: Framework :: Django
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: BSD License
 Classifier: Natural Language :: English
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.6
+Classifier: Programming Language :: Python :: 3.7
+Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
+Classifier: Programming Language :: Python :: 3
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Topic :: Internet :: WWW/HTTP :: Dynamic Content :: Message Boards
 Requires-Dist: django (>=3.2)
 Requires-Dist: django-haystack (>=2.1)
 Requires-Dist: django-mptt (>=0.10.0)
 Requires-Dist: django-widget-tweaks (>=1.4)
 Requires-Dist: markdown2 (>=2.3)
 Requires-Dist: pillow (>=2.2)
 Project-URL: Repository, https://github.com/ellmetha/django-machina
 Description-Content-Type: text/x-rst
 
+##############
 Django-machina
 ##############
 
 Django-machina is a forum framework for Django providing a way to build community-driven websites.
 It offers a full-featured yet very extensible forum solution:
 
 * Topic and post editing
```

