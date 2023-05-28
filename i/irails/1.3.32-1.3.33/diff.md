# Comparing `tmp/irails-1.3.32.tar.gz` & `tmp/irails-1.3.33.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "irails-1.3.32.tar", last modified: Sat May 27 12:10:09 2023, max compression
+gzip compressed data, was "irails-1.3.33.tar", last modified: Sun May 28 15:30:25 2023, max compression
```

## Comparing `irails-1.3.32.tar` & `irails-1.3.33.tar`

### file list

```diff
@@ -1,105 +1,105 @@
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.050382 irails-1.3.32/
--rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.32/MANIFEST.in
--rw-rw-rw-   0        0        0     4878 2023-05-27 12:10:09.050382 irails-1.3.32/PKG-INFO
--rw-rw-rw-   0        0        0     4096 2023-05-22 07:06:26.000000 irails-1.3.32/README.md
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.947497 irails-1.3.32/irails/
--rw-rw-rw-   0        0        0      307 2023-05-27 12:09:57.000000 irails-1.3.32/irails/__init__.py
--rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.32/irails/_i18n.py
--rw-rw-rw-   0        0        0     3959 2023-05-27 11:52:24.000000 irails-1.3.32/irails/_loader.py
--rw-rw-rw-   0        0        0     5595 2023-05-27 08:18:04.000000 irails-1.3.32/irails/_utils.py
--rw-rw-rw-   0        0        0    14149 2023-05-27 08:28:58.000000 irails-1.3.32/irails/auth.py
--rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.32/irails/base_controller.py
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.958473 irails-1.3.32/irails/casbin_adapters/
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.962458 irails-1.3.32/irails/casbin_adapters/__pycache__/
--rw-rw-rw-   0        0        0     9284 2023-05-25 05:11:53.000000 irails-1.3.32/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
--rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.32/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
--rw-rw-rw-   0        0        0    10591 2023-05-25 05:11:49.000000 irails-1.3.32/irails/casbin_adapters/sqlalchemy_adapter.py
--rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.32/irails/cbv.py
--rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.32/irails/config.py
--rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.32/irails/controller_utils.py
--rw-rw-rw-   0        0        0    26026 2023-05-27 10:48:38.000000 irails-1.3.32/irails/core.py
--rw-rw-rw-   0        0        0    20988 2023-05-27 08:36:14.000000 irails-1.3.32/irails/database.py
--rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.32/irails/log.py
--rw-rw-rw-   0        0        0     8876 2023-05-27 05:49:02.000000 irails-1.3.32/irails/midware.py
--rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.32/irails/midware_casbin.py
--rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.32/irails/midware_session.py
--rw-rw-rw-   0        0        0     4219 2023-05-27 10:24:12.000000 irails-1.3.32/irails/mvc_router.py
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.975468 irails-1.3.32/irails/scripts/
--rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.32/irails/scripts/__init__.py
--rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.32/irails/scripts/_app.py
--rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.32/irails/scripts/_controller.py
--rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.32/irails/scripts/_i18n.py
--rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.32/irails/scripts/_migrate.py
--rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.32/irails/scripts/_model.py
--rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.32/irails/scripts/_project.py
--rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.32/irails/scripts/_run.py
--rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.32/irails/scripts/_shell.py
--rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.32/irails/scripts/_test.py
--rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.32/irails/scripts/main.py
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.912676 irails-1.3.32/irails/scripts/tpls/
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.989292 irails-1.3.32/irails/scripts/tpls/app/
--rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.32/irails/scripts/tpls/app/controller.tpl
--rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.32/irails/scripts/tpls/app/css.tpl
--rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.32/irails/scripts/tpls/app/home.css.tpl
--rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.32/irails/scripts/tpls/app/home.tpl
--rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.32/irails/scripts/tpls/app/model.jinja
--rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.32/irails/scripts/tpls/app/service.jinja
--rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.32/irails/scripts/tpls/app/test_controller.jinja
--rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.32/irails/scripts/tpls/app/test_service.jinja
--rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.32/irails/scripts/tpls/app/view.tpl
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.992277 irails-1.3.32/irails/scripts/tpls/project/
--rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.32/irails/scripts/tpls/project/.gitignore
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.993275 irails-1.3.32/irails/scripts/tpls/project/apps/
--rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.32/irails/scripts/tpls/project/apps/__init__.py
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.005241 irails-1.3.32/irails/scripts/tpls/project/configs/
--rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.32/irails/scripts/tpls/project/configs/alembic.ini
--rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.32/irails/scripts/tpls/project/configs/authencation.yaml
--rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.32/irails/scripts/tpls/project/configs/cache.yaml
--rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin-adapter.csv
--rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin-model.conf
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.019209 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/
--rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
--rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
--rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
--rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
--rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
--rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
--rw-rw-rw-   0        0        0      274 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
--rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
--rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
--rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.32/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
--rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.32/irails/scripts/tpls/project/configs/database.yaml
--rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.32/irails/scripts/tpls/project/configs/general.yaml
--rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.32/irails/scripts/tpls/project/configs/session.yaml
--rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.32/irails/scripts/tpls/project/configs/upload.yaml
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.917102 irails-1.3.32/irails/scripts/tpls/project/data/
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.023194 irails-1.3.32/irails/scripts/tpls/project/data/alembic/
--rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.32/irails/scripts/tpls/project/data/alembic/README
--rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.32/irails/scripts/tpls/project/data/alembic/env.py
--rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.32/irails/scripts/tpls/project/data/alembic/script.py.mako
--rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.32/irails/scripts/tpls/project/main.py
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.026193 irails-1.3.32/irails/scripts/tpls/project/public/
--rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.32/irails/scripts/tpls/project/public/error_404.html
--rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.32/irails/scripts/tpls/project/public/error_500.html
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.030174 irails-1.3.32/irails/scripts/tpls/project/public/libs/
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.920096 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.036191 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
--rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.043179 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
--rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
--rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.32/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
--rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.32/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.922094 irails-1.3.32/irails/scripts/tpls/project/public/vue@3.2.36/
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:09.045907 irails-1.3.32/irails/scripts/tpls/project/public/vue@3.2.36/dist/
--rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.32/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
--rw-rw-rw-   0        0        0     1737 2023-05-27 08:50:04.000000 irails-1.3.32/irails/unit_test.py
--rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.32/irails/view.py
-drwxrwxrwx   0        0        0        0 2023-05-27 12:10:08.956476 irails-1.3.32/irails.egg-info/
--rw-rw-rw-   0        0        0     4878 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     3185 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       52 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0      367 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2023-05-27 12:10:08.000000 irails-1.3.32/irails.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-05-27 12:10:09.050382 irails-1.3.32/setup.cfg
--rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.32/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.659110 irails-1.3.33/
+-rw-rw-rw-   0        0        0       83 2023-05-04 04:10:30.000000 irails-1.3.33/MANIFEST.in
+-rw-rw-rw-   0        0        0     4956 2023-05-28 15:30:25.659110 irails-1.3.33/PKG-INFO
+-rw-rw-rw-   0        0        0     4174 2023-05-27 12:12:58.000000 irails-1.3.33/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.560706 irails-1.3.33/irails/
+-rw-rw-rw-   0        0        0      307 2023-05-28 15:29:45.000000 irails-1.3.33/irails/__init__.py
+-rw-rw-rw-   0        0        0     4887 2023-05-21 14:33:24.000000 irails-1.3.33/irails/_i18n.py
+-rw-rw-rw-   0        0        0     4199 2023-05-27 15:17:05.000000 irails-1.3.33/irails/_loader.py
+-rw-rw-rw-   0        0        0     5595 2023-05-27 08:18:04.000000 irails-1.3.33/irails/_utils.py
+-rw-rw-rw-   0        0        0    15330 2023-05-28 15:25:34.000000 irails-1.3.33/irails/auth.py
+-rw-rw-rw-   0        0        0    12705 2023-05-18 07:46:03.000000 irails-1.3.33/irails/base_controller.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.570680 irails-1.3.33/irails/casbin_adapters/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.572675 irails-1.3.33/irails/casbin_adapters/__pycache__/
+-rw-rw-rw-   0        0        0     9284 2023-05-25 05:11:53.000000 irails-1.3.33/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc
+-rw-rw-rw-   0        0        0    17834 2023-04-30 14:29:09.000000 irails-1.3.33/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc
+-rw-rw-rw-   0        0        0    10591 2023-05-25 05:11:49.000000 irails-1.3.33/irails/casbin_adapters/sqlalchemy_adapter.py
+-rw-rw-rw-   0        0        0     4381 2023-02-25 09:43:32.000000 irails-1.3.33/irails/cbv.py
+-rw-rw-rw-   0        0        0     6357 2023-05-25 10:46:48.000000 irails-1.3.33/irails/config.py
+-rw-rw-rw-   0        0        0    13203 2023-05-26 14:20:32.000000 irails-1.3.33/irails/controller_utils.py
+-rw-rw-rw-   0        0        0    26026 2023-05-27 10:48:38.000000 irails-1.3.33/irails/core.py
+-rw-rw-rw-   0        0        0    20962 2023-05-28 14:25:03.000000 irails-1.3.33/irails/database.py
+-rw-rw-rw-   0        0        0     1592 2023-05-25 14:19:01.000000 irails-1.3.33/irails/log.py
+-rw-rw-rw-   0        0        0     8876 2023-05-27 05:49:02.000000 irails-1.3.33/irails/midware.py
+-rw-rw-rw-   0        0        0     2141 2023-04-03 14:30:15.000000 irails-1.3.33/irails/midware_casbin.py
+-rw-rw-rw-   0        0        0     9103 2023-05-16 08:16:43.000000 irails-1.3.33/irails/midware_session.py
+-rw-rw-rw-   0        0        0     4219 2023-05-27 10:24:12.000000 irails-1.3.33/irails/mvc_router.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.585144 irails-1.3.33/irails/scripts/
+-rw-rw-rw-   0        0        0        0 2023-04-26 07:44:41.000000 irails-1.3.33/irails/scripts/__init__.py
+-rw-rw-rw-   0        0        0     7862 2023-05-13 15:04:27.000000 irails-1.3.33/irails/scripts/_app.py
+-rw-rw-rw-   0        0        0     6892 2023-05-19 07:21:20.000000 irails-1.3.33/irails/scripts/_controller.py
+-rw-rw-rw-   0        0        0     7763 2023-05-21 13:57:03.000000 irails-1.3.33/irails/scripts/_i18n.py
+-rw-rw-rw-   0        0        0     1332 2023-05-21 08:39:33.000000 irails-1.3.33/irails/scripts/_migrate.py
+-rw-rw-rw-   0        0        0     3774 2023-05-14 13:34:33.000000 irails-1.3.33/irails/scripts/_model.py
+-rw-rw-rw-   0        0        0     2301 2023-05-03 14:35:33.000000 irails-1.3.33/irails/scripts/_project.py
+-rw-rw-rw-   0        0        0     1399 2023-05-26 14:27:13.000000 irails-1.3.33/irails/scripts/_run.py
+-rw-rw-rw-   0        0        0     2288 2023-05-11 14:15:32.000000 irails-1.3.33/irails/scripts/_shell.py
+-rw-rw-rw-   0        0        0     4930 2023-05-21 14:27:15.000000 irails-1.3.33/irails/scripts/_test.py
+-rw-rw-rw-   0        0        0     2900 2023-05-21 08:16:21.000000 irails-1.3.33/irails/scripts/main.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.524657 irails-1.3.33/irails/scripts/tpls/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.596794 irails-1.3.33/irails/scripts/tpls/app/
+-rw-rw-rw-   0        0        0      223 2023-05-09 15:18:47.000000 irails-1.3.33/irails/scripts/tpls/app/controller.tpl
+-rw-rw-rw-   0        0        0        0 2023-04-28 06:03:05.000000 irails-1.3.33/irails/scripts/tpls/app/css.tpl
+-rw-rw-rw-   0        0        0      791 2023-04-25 10:42:10.000000 irails-1.3.33/irails/scripts/tpls/app/home.css.tpl
+-rw-rw-rw-   0        0        0     1293 2023-05-05 10:16:42.000000 irails-1.3.33/irails/scripts/tpls/app/home.tpl
+-rw-rw-rw-   0        0        0     1023 2023-05-19 12:27:03.000000 irails-1.3.33/irails/scripts/tpls/app/model.jinja
+-rw-rw-rw-   0        0        0      197 2023-05-24 11:06:24.000000 irails-1.3.33/irails/scripts/tpls/app/service.jinja
+-rw-rw-rw-   0        0        0      237 2023-05-13 13:54:20.000000 irails-1.3.33/irails/scripts/tpls/app/test_controller.jinja
+-rw-rw-rw-   0        0        0      908 2023-05-24 14:14:47.000000 irails-1.3.33/irails/scripts/tpls/app/test_service.jinja
+-rw-rw-rw-   0        0        0       18 2023-05-02 08:56:04.000000 irails-1.3.33/irails/scripts/tpls/app/view.tpl
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.599795 irails-1.3.33/irails/scripts/tpls/project/
+-rw-rw-rw-   0        0        0      139 2023-04-23 09:46:24.000000 irails-1.3.33/irails/scripts/tpls/project/.gitignore
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.601780 irails-1.3.33/irails/scripts/tpls/project/apps/
+-rw-rw-rw-   0        0        0        0 2023-04-26 09:58:51.000000 irails-1.3.33/irails/scripts/tpls/project/apps/__init__.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.611680 irails-1.3.33/irails/scripts/tpls/project/configs/
+-rw-rw-rw-   0        0        0      746 2023-05-09 06:45:34.000000 irails-1.3.33/irails/scripts/tpls/project/configs/alembic.ini
+-rw-rw-rw-   0        0        0      179 2023-05-13 09:22:15.000000 irails-1.3.33/irails/scripts/tpls/project/configs/authencation.yaml
+-rw-rw-rw-   0        0        0        0 2023-03-06 08:27:07.000000 irails-1.3.33/irails/scripts/tpls/project/configs/cache.yaml
+-rw-rw-rw-   0        0        0      104 2023-05-04 05:06:32.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin-adapter.csv
+-rw-rw-rw-   0        0        0      302 2023-05-04 05:24:51.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin-model.conf
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.626640 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/
+-rw-rw-rw-   0        0        0      204 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/ALC.conf
+-rw-rw-rw-   0        0        0       37 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/ALC.csv
+-rw-rw-rw-   0        0        0      236 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBAC.conf
+-rw-rw-rw-   0        0        0      125 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBAC.csv
+-rw-rw-rw-   0        0        0      249 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBACR.conf
+-rw-rw-rw-   0        0        0      159 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBACR.csv
+-rw-rw-rw-   0        0        0      319 2023-05-28 15:30:10.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBACT.conf
+-rw-rw-rw-   0        0        0      178 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RBACT.csv
+-rw-rw-rw-   0        0        0      222 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.conf
+-rw-rw-rw-   0        0        0      152 2023-05-18 07:46:03.000000 irails-1.3.33/irails/scripts/tpls/project/configs/casbin_templates/RESTFUL.csv
+-rw-rw-rw-   0        0        0      817 2023-05-10 10:45:36.000000 irails-1.3.33/irails/scripts/tpls/project/configs/database.yaml
+-rw-rw-rw-   0        0        0      748 2023-05-11 05:35:06.000000 irails-1.3.33/irails/scripts/tpls/project/configs/general.yaml
+-rw-rw-rw-   0        0        0      337 2023-04-22 10:54:12.000000 irails-1.3.33/irails/scripts/tpls/project/configs/session.yaml
+-rw-rw-rw-   0        0        0      272 2023-05-09 06:44:59.000000 irails-1.3.33/irails/scripts/tpls/project/configs/upload.yaml
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.528485 irails-1.3.33/irails/scripts/tpls/project/data/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.630629 irails-1.3.33/irails/scripts/tpls/project/data/alembic/
+-rw-rw-rw-   0        0        0       38 2023-04-09 12:01:20.000000 irails-1.3.33/irails/scripts/tpls/project/data/alembic/README
+-rw-rw-rw-   0        0        0     2144 2023-04-30 09:03:04.000000 irails-1.3.33/irails/scripts/tpls/project/data/alembic/env.py
+-rw-rw-rw-   0        0        0      510 2023-04-09 12:01:20.000000 irails-1.3.33/irails/scripts/tpls/project/data/alembic/script.py.mako
+-rw-rw-rw-   0        0        0      231 2023-05-11 15:42:13.000000 irails-1.3.33/irails/scripts/tpls/project/main.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.635451 irails-1.3.33/irails/scripts/tpls/project/public/
+-rw-rw-rw-   0        0        0     1233 2023-05-02 08:46:22.000000 irails-1.3.33/irails/scripts/tpls/project/public/error_404.html
+-rw-rw-rw-   0        0        0     1083 2023-05-02 08:46:46.000000 irails-1.3.33/irails/scripts/tpls/project/public/error_500.html
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.638449 irails-1.3.33/irails/scripts/tpls/project/public/libs/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.533215 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.644964 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/
+-rw-rw-rw-   0        0        0  1970121 2023-04-23 08:02:36.000000 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.652555 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/
+-rw-rw-rw-   0        0        0   323666 2023-04-23 08:04:13.000000 irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css
+-rw-rw-rw-   0        0        0      725 2023-04-21 12:39:53.000000 irails-1.3.33/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js
+-rw-rw-rw-   0        0        0  1441055 2023-04-21 07:36:37.000000 irails-1.3.33/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.534212 irails-1.3.33/irails/scripts/tpls/project/public/vue@3.2.36/
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.654854 irails-1.3.33/irails/scripts/tpls/project/public/vue@3.2.36/dist/
+-rw-rw-rw-   0        0        0   640610 2023-04-21 07:36:07.000000 irails-1.3.33/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js
+-rw-rw-rw-   0        0        0     1737 2023-05-27 08:50:04.000000 irails-1.3.33/irails/unit_test.py
+-rw-rw-rw-   0        0        0     3034 2023-05-16 08:15:25.000000 irails-1.3.33/irails/view.py
+drwxrwxrwx   0        0        0        0 2023-05-28 15:30:25.568685 irails-1.3.33/irails.egg-info/
+-rw-rw-rw-   0        0        0     4956 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     3185 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       52 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0      367 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 15:30:25.000000 irails-1.3.33/irails.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-05-28 15:30:25.660121 irails-1.3.33/setup.cfg
+-rw-rw-rw-   0        0        0     2551 2023-05-09 11:27:27.000000 irails-1.3.33/setup.py
```

### Comparing `irails-1.3.32/PKG-INFO` & `irails-1.3.33/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.32
+Version: 1.3.33
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -58,14 +58,15 @@
     |   |   +---tests                       ## Unit testting
     |   |   +---views                       ## Static view files (use `Jinja2` Template)
     |   |   |   |   layout.html
     |   |   |   |
     |   |   |   +---home                    ## The controller action's static file(name is same to the controller's class name)
     |   |   |   |       home.css            
     |   |   |   |       home.html           ## Static file corresponding to action(name is same to the controller's method name)
+    |   |   |---manifest.yaml               ## The app manifest for each app
     +---configs                             ## Project configure dir
     |       alembic.ini                     ## Alembic configure file (Generally, there is no need to change, used the database migration)
     |       casbin-adapter.csv              ## Casbin auth module config adapter file()
     |       casbin-model.conf               ## Casbin auth config model
     |       database.yaml                   ## Configure for database support
     |       general.yaml                    ## General configures
     |       session.yaml                    ## Session configures
```

### Comparing `irails-1.3.32/README.md` & `irails-1.3.33/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -38,14 +38,15 @@
     |   |   +---tests                       ## Unit testting
     |   |   +---views                       ## Static view files (use `Jinja2` Template)
     |   |   |   |   layout.html
     |   |   |   |
     |   |   |   +---home                    ## The controller action's static file(name is same to the controller's class name)
     |   |   |   |       home.css            
     |   |   |   |       home.html           ## Static file corresponding to action(name is same to the controller's method name)
+    |   |   |---manifest.yaml               ## The app manifest for each app
     +---configs                             ## Project configure dir
     |       alembic.ini                     ## Alembic configure file (Generally, there is no need to change, used the database migration)
     |       casbin-adapter.csv              ## Casbin auth module config adapter file()
     |       casbin-model.conf               ## Casbin auth config model
     |       database.yaml                   ## Configure for database support
     |       general.yaml                    ## General configures
     |       session.yaml                    ## Session configures
```

### Comparing `irails-1.3.32/irails/_i18n.py` & `irails-1.3.33/irails/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/_loader.py` & `irails-1.3.33/irails/_loader.py`

 * *Files 15% similar despite different names*

```diff
@@ -98,14 +98,17 @@
                             sys.path.insert(0,_abs_app_path)
                         debug and print('load app:'+app)
                         n = _load_app(app,manifest)
                         if n:
                             if application:
                                 if not app in application.apps:
                                     application.apps[app] = {}
+                                elif application.apps[app]['manifest']:
+                                    raise RuntimeError(_('The app:%s already loaded,Duplicate name in (%s) ') % (app,abs_app_dir))
+                                 
                                 application.apps[app]['manifest'] = manifest
                             loaded = loaded + 1
                         else:
                             unloaded = unloaded + 1
                 else:
                     #just return the app list
                     apps.append( f"{app_dir}.{app}" )
```

### Comparing `irails-1.3.32/irails/_utils.py` & `irails-1.3.33/irails/_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/auth.py` & `irails-1.3.33/irails/auth.py`

 * *Files 12% similar despite different names*

```diff
@@ -13,38 +13,45 @@
 from casbin.persist.adapter import Adapter
 # from .midware_casbin import CasbinMiddleware
 
 from .config import config, ROOT_PATH
 from .log import _log
 import jwt
 from datetime import datetime, timedelta
-from typing import Optional, Tuple, Type, Union, Dict
+from typing import List, Optional, Tuple, Type, Union, Dict
 from ._utils import iJSONEncoder, is_datetime_format
 from ._i18n import _
 AUTH_EXPIRED = '[EXPIRED]!'
 _session_name: str = ""
 default_domain = "system"
 
 
 class DomainUser(BaseUser):
-    def __init__(self, username: str = 'anonymous', group: str = "", domain: str = "") -> None:
+    def __init__(self, username: str = 'anonymous', roles = [], domain: str = "") -> None:
+        '''
+        :group Roles 
+        :domain Tenant
+        '''
         self.username = username
-        self._group = group
+        self._roles = roles
         self._domain = domain or default_domain
         self._lang = "zh"
         self._timezone = 'Asia/Shanghai'
         super().__init__()
 
     @property
-    def group(self):
-        return self._group
+    def roles(self):
+        return self._roles
 
-    @group.setter
-    def group(self, value):
-        self._group = value
+    @roles.setter
+    def roles(self, value:List):
+        names=[]
+        for row in value:
+            names.append(row.name)
+        self._roles = names
 
     @property
     def domain(self):
         return self._domain
 
     @domain.setter
     def domain(self, value):
@@ -59,16 +66,16 @@
     @property
     def display_name(self) -> str:
         return self.username
 
     @property
     def identity(self) -> str:
         identity = self.username
-        if self._group:
-            group = self._group
+        if self._roles:
+            group = self._roles
             if self._domain:
                 group = self._domain+"."+group
             identity += '@'+group
         return identity
 
     def __repr__(self):
         return self.identity
@@ -126,16 +133,17 @@
             return self.enforcer.has_grouping_policy(*args)
         raise RuntimeError("Casbin Enforcer is None")
 
     def _auth(self, request: Request, user: DomainUser):
         '''
         do verity,return True means `Success` and others `Failed`
         '''
-
-        sub = user.identity
+        if not user.roles:
+            raise RuntimeError(_("User must have a role %s") % user)
+        sub = ','.join(user.roles)
         path = request.url.path
         method = request.method
         param: Tuple = (sub, user.domain, path, method,)
 
         return self.enforcer.enforce(*param)
 
     def __get_token_from_header(self, authorization: str, prefix: str) -> str:
@@ -223,17 +231,22 @@
             return False, None
         if isinstance(userobj, BasicUser):
             user = userobj
         elif isinstance(userobj, str):
             user = BasicUser(userobj)
         request.scope['user'] = user
         auth_type: str = kwargs.get("auth_type")
-        if not auth_type or auth_type.lower() == 'public':
+        if not auth_type or auth_type.lower() == 'none':
             return True,  user
-        result = _casbin_auth._auth(request=request, user=user)
+        elif auth_type.lower() == 'public':
+            return user.is_authenticated, user
+        elif not user.is_authenticated:
+            return False.user
+        else:
+            result = _casbin_auth._auth(request=request, user=user)
 
         return result, user
 
     def clear_userinfo(self, request: Request):
         global _session_name
         del request.session[_session_name]
 
@@ -285,18 +298,18 @@
                 jwtuser = from_payload(payload)
                 request.scope['user'] = jwtuser
 
         if auth_type.lower() == 'public':
             return jwtuser.is_authenticated, jwtuser
         elif auth_type.lower() == 'none':
             return True, jwtuser
-        elif payload and not jwtuser.is_authenticated:
-            jwtuser = from_payload(payload)
-            request.scope['user'] = jwtuser
-        result = _casbin_auth._auth(request=request, user=jwtuser)
+        elif   not jwtuser.is_authenticated: 
+            return False,jwtuser
+        else:
+            result = _casbin_auth._auth(request=request, user=jwtuser)
         return result, jwtuser
 
     def clear_userinfo(self, request: Request):
         global _session_name
         if _session_name in request.session:
             del request.session[_session_name]
 
@@ -313,15 +326,15 @@
             expire = datetime.utcnow() + timedelta(
                 minutes=expires_delta
             )
 
         auth_user_obj = {
             "exp": expire,
             "username": user.username,
-            "group": user.group,
+            "group": user.roles,
             "domain": user.domain
         }
 
         request: Request = kwargs['request']
 
         access_token = jwt.encode(
             auth_user_obj, self.secret_key, self.algorithm)
@@ -336,24 +349,42 @@
 def init(app: FastAPI, backend: AuthenticationBackend, adapter_class: Type = None, **kwagrs) -> AuthenticationBackend:
     """
         kwargs:secret_key=KEY
     """
     __session_name = config.get("auth").get("session_name", 'user')
     global _casbin_auth
     cfg = config.get("auth")
+    super_domain = cfg.get('super_domain','system')
+    super_group = cfg.get('super_group','admin')
+
     adapter_uri = kwagrs.get('adapter_uri', None)
 
     del kwagrs['adapter_uri']
     model_file = cfg.get("auth_model", './configs/casbin-model.conf')
-    model_file = os.path.abspath(os.path.join(ROOT_PATH, model_file))
+    if not os.path.isabs(model_file):
+        model_file = os.path.abspath(os.path.join(ROOT_PATH, model_file))
+    if not os.path.exists(model_file):
+        raise RuntimeError(_("Casbin model file %s does not exists!")%model_file)
+    
     if adapter_class is FileAdapter and not os.path.isabs(adapter_uri):
         adapter_uri = os.path.abspath(os.path.join(ROOT_PATH, adapter_uri))
     adapter = adapter_class(adapter_uri)
-    enforcer = casbin.Enforcer(model_file, adapter)
-
+    from casbin.model import Model
+    model = Model()
+    with open(model_file,'r',encoding='utf-8') as f: 
+        model_content = f.read()
+        # if super_user and super_group:
+        #     model_content = model_content.replace("${super_user}",super_user).replace("${super_group}",super_group)
+        model.load_model_from_text(model_content)
+    enforcer = casbin.Enforcer(model, adapter)
+
+    def is_super(roles,domain): 
+        return super_group in roles and domain == super_domain
+    
+    enforcer.add_function('is_super',is_super)
     _casbin_auth = CasbinAuth(enforcer=enforcer, session_name=__session_name)
 
     return backend(**kwagrs)
 
 
 def reload_adapter(app: FastAPI, adapter: Adapter = None):
     cfg = config.get("auth")
```

### Comparing `irails-1.3.32/irails/base_controller.py` & `irails-1.3.33/irails/base_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc` & `irails-1.3.33/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-310.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc` & `irails-1.3.33/irails/casbin_adapters/__pycache__/sqlalchemy_adapter.cpython-311.pyc`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/casbin_adapters/sqlalchemy_adapter.py` & `irails-1.3.33/irails/casbin_adapters/sqlalchemy_adapter.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/cbv.py` & `irails-1.3.33/irails/cbv.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/config.py` & `irails-1.3.33/irails/config.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/controller_utils.py` & `irails-1.3.33/irails/controller_utils.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/core.py` & `irails-1.3.33/irails/core.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/database.py` & `irails-1.3.33/irails/database.py`

 * *Files 1% similar despite different names*

```diff
@@ -324,15 +324,15 @@
         else:
             if  kwargs  :
                 m=model(**kwargs)
         if m:
             session = self.session()
             session.add(m)
             session.commit()
-            session.merge(m,load=False)
+             
             return m
         return None
     @classmethod
     def add_all(self,values:List['Base']):
         with self.get_session() as session: 
             session.add_all(values)
```

### Comparing `irails-1.3.32/irails/log.py` & `irails-1.3.33/irails/log.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/midware.py` & `irails-1.3.33/irails/midware.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/midware_casbin.py` & `irails-1.3.33/irails/midware_casbin.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/midware_session.py` & `irails-1.3.33/irails/midware_session.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/mvc_router.py` & `irails-1.3.33/irails/mvc_router.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/_app.py` & `irails-1.3.33/irails/scripts/_app.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/_controller.py` & `irails-1.3.33/irails/scripts/_controller.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/_i18n.py` & `irails-1.3.33/irails/scripts/_i18n.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/_migrate.py` & `irails-1.3.33/irails/scripts/_migrate.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/_model.py` & `irails-1.3.33/irails/scripts/_model.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/_project.py` & `irails-1.3.33/irails/scripts/_project.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/_run.py` & `irails-1.3.33/irails/scripts/_run.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/_shell.py` & `irails-1.3.33/irails/scripts/_shell.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/_test.py` & `irails-1.3.33/irails/scripts/_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/main.py` & `irails-1.3.33/irails/scripts/main.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/app/home.css.tpl` & `irails-1.3.33/irails/scripts/tpls/app/home.css.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/app/home.tpl` & `irails-1.3.33/irails/scripts/tpls/app/home.tpl`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/app/model.jinja` & `irails-1.3.33/irails/scripts/tpls/app/model.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/app/test_service.jinja` & `irails-1.3.33/irails/scripts/tpls/app/test_service.jinja`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/configs/alembic.ini` & `irails-1.3.33/irails/scripts/tpls/project/configs/alembic.ini`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/configs/database.yaml` & `irails-1.3.33/irails/scripts/tpls/project/configs/database.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/configs/general.yaml` & `irails-1.3.33/irails/scripts/tpls/project/configs/general.yaml`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/data/alembic/env.py` & `irails-1.3.33/irails/scripts/tpls/project/data/alembic/env.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/public/error_404.html` & `irails-1.3.33/irails/scripts/tpls/project/public/error_404.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/public/error_500.html` & `irails-1.3.33/irails/scripts/tpls/project/public/error_500.html`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js` & `irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/dist/index.full.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css` & `irails-1.3.33/irails/scripts/tpls/project/public/libs/element-plus@2.3.3/theme-chalk/index.css`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js` & `irails-1.3.33/irails/scripts/tpls/project/public/libs/vue3-sfc-loader-config.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js` & `irails-1.3.33/irails/scripts/tpls/project/public/libs/vue3-sfc-loader.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js` & `irails-1.3.33/irails/scripts/tpls/project/public/vue@3.2.36/dist/vue.global.js`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/unit_test.py` & `irails-1.3.33/irails/unit_test.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails/view.py` & `irails-1.3.33/irails/view.py`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/irails.egg-info/PKG-INFO` & `irails-1.3.33/irails.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: irails
-Version: 1.3.32
+Version: 1.3.33
 Summary: Simple and elegant use of FastApi in MVC mode
 Home-page: https://github.com/smjkzsl/irails
 Author: Bruce chou
 Author-email: smjkzsl@gmail.com
 License: Apache License 2.0
 Keywords: web framework,mvc framework,fastapi framework
 Classifier: License :: OSI Approved :: Apache Software License
@@ -58,14 +58,15 @@
     |   |   +---tests                       ## Unit testting
     |   |   +---views                       ## Static view files (use `Jinja2` Template)
     |   |   |   |   layout.html
     |   |   |   |
     |   |   |   +---home                    ## The controller action's static file(name is same to the controller's class name)
     |   |   |   |       home.css            
     |   |   |   |       home.html           ## Static file corresponding to action(name is same to the controller's method name)
+    |   |   |---manifest.yaml               ## The app manifest for each app
     +---configs                             ## Project configure dir
     |       alembic.ini                     ## Alembic configure file (Generally, there is no need to change, used the database migration)
     |       casbin-adapter.csv              ## Casbin auth module config adapter file()
     |       casbin-model.conf               ## Casbin auth config model
     |       database.yaml                   ## Configure for database support
     |       general.yaml                    ## General configures
     |       session.yaml                    ## Session configures
```

### Comparing `irails-1.3.32/irails.egg-info/SOURCES.txt` & `irails-1.3.33/irails.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `irails-1.3.32/setup.py` & `irails-1.3.33/setup.py`

 * *Files identical despite different names*

