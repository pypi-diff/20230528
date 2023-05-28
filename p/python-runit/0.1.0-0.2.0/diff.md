# Comparing `tmp/python-runit-0.1.0.tar.gz` & `tmp/python-runit-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "python-runit-0.1.0.tar", last modified: Sun Apr 30 20:37:12 2023, max compression
+gzip compressed data, was "python-runit-0.2.0.tar", last modified: Sun May 28 17:04:09 2023, max compression
```

## Comparing `python-runit-0.1.0.tar` & `python-runit-0.2.0.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.655633 python-runit-0.1.0/
--rw-rw-rw-   0        0        0     1090 2023-04-30 20:35:32.000000 python-runit-0.1.0/LICENSE
--rw-rw-rw-   0        0        0       89 2022-12-02 15:17:26.000000 python-runit-0.1.0/MANIFEST.in
--rw-rw-rw-   0        0        0     4662 2023-04-30 20:37:12.653631 python-runit-0.1.0/PKG-INFO
--rw-rw-rw-   0        0        0     3779 2022-11-18 15:19:03.000000 python-runit-0.1.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.091405 python-runit-0.1.0/python_runit.egg-info/
--rw-rw-rw-   0        0        0     4662 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1561 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       41 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       62 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/requires.txt
--rw-rw-rw-   0        0        0        6 2023-04-30 20:37:11.000000 python-runit-0.1.0/python_runit.egg-info/top_level.txt
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.159412 python-runit-0.1.0/runit/
--rw-rw-rw-   0        0        0      767 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/Request.py
--rw-rw-rw-   0        0        0      376 2022-12-10 20:04:06.000000 python-runit-0.1.0/runit/__init__.py
--rw-rw-rw-   0        0        0    12358 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/cli.py
--rw-rw-rw-   0        0        0     2064 2023-04-30 20:35:32.000000 python-runit-0.1.0/runit/constants.py
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.251402 python-runit-0.1.0/runit/languages/
--rw-rw-rw-   0        0        0     1004 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/languages/__init__.py
--rw-rw-rw-   0        0        0      503 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/languages/javascript.py
--rw-rw-rw-   0        0        0     3704 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/languages/multi.py
--rw-rw-rw-   0        0        0      487 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/languages/php.py
--rw-rw-rw-   0        0        0      485 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/languages/python.py
--rw-rw-rw-   0        0        0     2425 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/languages/runtime.py
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.285884 python-runit-0.1.0/runit/modules/
--rw-rw-rw-   0        0        0       30 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/modules/__init__.py
--rw-rw-rw-   0        0        0     8941 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/modules/account.py
--rw-rw-rw-   0        0        0    13182 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/runit.py
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.323636 python-runit-0.1.0/runit/templates/
--rw-rw-rw-   0        0        0       67 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/.runitignore
--rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/404.html
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.342624 python-runit-0.1.0/runit/templates/javascript/
--rw-rw-rw-   0        0        0       13 2022-09-03 23:35:52.000000 python-runit-0.1.0/runit/templates/javascript/.env
--rw-rw-rw-   0        0        0      259 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/javascript/main.js
--rw-rw-rw-   0        0        0      299 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/javascript/package.json
--rw-rw-rw-   0        0        0      270 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/javascript/runit.json
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.550056 python-runit-0.1.0/runit/templates/multi/
--rw-rw-rw-   0        0        0     1182 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/application.py
--rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/composer.json
--rw-rw-rw-   0        0        0      227 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/index.php
--rw-rw-rw-   0        0        0      259 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/main.js
--rw-rw-rw-   0        0        0      299 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/package.json
--rw-rw-rw-   0        0        0      392 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/request.php
--rw-rw-rw-   0        0        0        0 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/requirements.txt
--rw-rw-rw-   0        0        0       27 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/multi/test.php
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.579630 python-runit-0.1.0/runit/templates/php/
--rw-rw-rw-   0        0        0       12 2022-09-03 23:35:52.000000 python-runit-0.1.0/runit/templates/php/.env
--rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/php/composer.json
--rw-rw-rw-   0        0        0      227 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/php/index.php
--rw-rw-rw-   0        0        0      392 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/php/request.php
--rw-rw-rw-   0        0        0      262 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/php/runit.json
--rw-rw-rw-   0        0        0       27 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/php/test.php
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.622630 python-runit-0.1.0/runit/templates/python/
--rw-rw-rw-   0        0        0       18 2022-09-03 23:35:52.000000 python-runit-0.1.0/runit/templates/python/.env
--rw-rw-rw-   0        0        0     1182 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/templates/python/application.py
--rw-rw-rw-   0        0        0      363 2023-04-30 20:35:32.000000 python-runit-0.1.0/runit/templates/python/requirements.txt
--rw-rw-rw-   0        0        0      275 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/python/runit.json
--rw-rw-rw-   0        0        0      266 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/templates/runit.json
--rw-rw-rw-   0        0        0      404 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/test.py
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.020402 python-runit-0.1.0/runit/tools/
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.630628 python-runit-0.1.0/runit/tools/javascript/
--rw-rw-rw-   0        0        0      250 2023-04-30 18:54:45.000000 python-runit-0.1.0/runit/tools/javascript/loader.js
--rw-rw-rw-   0        0        0      490 2023-04-30 20:06:25.000000 python-runit-0.1.0/runit/tools/javascript/runner.js
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.640631 python-runit-0.1.0/runit/tools/php/
--rw-rw-rw-   0        0        0      362 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/tools/php/loader.php
--rw-rw-rw-   0        0        0      630 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/tools/php/runner.php
-drwxrwxrwx   0        0        0        0 2023-04-30 20:37:12.648627 python-runit-0.1.0/runit/tools/python/
--rw-rw-rw-   0        0        0      380 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/tools/python/loader.py
--rw-rw-rw-   0        0        0      639 2022-11-16 16:12:51.000000 python-runit-0.1.0/runit/tools/python/runner.py
--rw-rw-rw-   0        0        0       42 2023-04-30 20:37:12.656627 python-runit-0.1.0/setup.cfg
--rw-rw-rw-   0        0        0     1433 2023-04-30 20:35:32.000000 python-runit-0.1.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:09.293608 python-runit-0.2.0/
+-rw-rw-rw-   0        0        0     1090 2023-04-30 20:35:32.000000 python-runit-0.2.0/LICENSE
+-rw-rw-rw-   0        0        0       89 2022-12-02 15:17:26.000000 python-runit-0.2.0/MANIFEST.in
+-rw-rw-rw-   0        0        0     4703 2023-05-28 17:04:09.290605 python-runit-0.2.0/PKG-INFO
+-rw-rw-rw-   0        0        0     3779 2022-11-18 15:19:03.000000 python-runit-0.2.0/README.md
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:07.136947 python-runit-0.2.0/python_runit.egg-info/
+-rw-rw-rw-   0        0        0     4703 2023-05-28 17:04:06.000000 python-runit-0.2.0/python_runit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1561 2023-05-28 17:04:06.000000 python-runit-0.2.0/python_runit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 17:04:06.000000 python-runit-0.2.0/python_runit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       41 2023-05-28 17:04:06.000000 python-runit-0.2.0/python_runit.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       39 2023-05-28 17:04:06.000000 python-runit-0.2.0/python_runit.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        6 2023-05-28 17:04:06.000000 python-runit-0.2.0/python_runit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:07.434947 python-runit-0.2.0/runit/
+-rw-rw-rw-   0        0        0      767 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/Request.py
+-rw-rw-rw-   0        0        0      376 2022-12-10 20:04:06.000000 python-runit-0.2.0/runit/__init__.py
+-rw-rw-rw-   0        0        0    12750 2023-05-28 16:56:26.000000 python-runit-0.2.0/runit/cli.py
+-rw-rw-rw-   0        0        0     2064 2023-05-28 16:56:26.000000 python-runit-0.2.0/runit/constants.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:07.770947 python-runit-0.2.0/runit/languages/
+-rw-rw-rw-   0        0        0     1004 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/languages/__init__.py
+-rw-rw-rw-   0        0        0      503 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/languages/javascript.py
+-rw-rw-rw-   0        0        0     3704 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/languages/multi.py
+-rw-rw-rw-   0        0        0      487 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/languages/php.py
+-rw-rw-rw-   0        0        0      485 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/languages/python.py
+-rw-rw-rw-   0        0        0     2425 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/languages/runtime.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:07.872947 python-runit-0.2.0/runit/modules/
+-rw-rw-rw-   0        0        0       30 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/modules/__init__.py
+-rw-rw-rw-   0        0        0     8941 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/modules/account.py
+-rw-rw-rw-   0        0        0    13030 2023-05-28 16:56:26.000000 python-runit-0.2.0/runit/runit.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:07.999945 python-runit-0.2.0/runit/templates/
+-rw-rw-rw-   0        0        0       67 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/.runitignore
+-rw-rw-rw-   0        0        0     1157 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/templates/404.html
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:08.152947 python-runit-0.2.0/runit/templates/javascript/
+-rw-rw-rw-   0        0        0       13 2022-09-03 23:35:52.000000 python-runit-0.2.0/runit/templates/javascript/.env
+-rw-rw-rw-   0        0        0      259 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/templates/javascript/main.js
+-rw-rw-rw-   0        0        0      299 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/templates/javascript/package.json
+-rw-rw-rw-   0        0        0      270 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/javascript/runit.json
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:08.481603 python-runit-0.2.0/runit/templates/multi/
+-rw-rw-rw-   0        0        0     1182 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/multi/application.py
+-rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/multi/composer.json
+-rw-rw-rw-   0        0        0      227 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/multi/index.php
+-rw-rw-rw-   0        0        0      259 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/multi/main.js
+-rw-rw-rw-   0        0        0      299 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/multi/package.json
+-rw-rw-rw-   0        0        0      392 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/multi/request.php
+-rw-rw-rw-   0        0        0        0 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/multi/requirements.txt
+-rw-rw-rw-   0        0        0       27 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/multi/test.php
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:08.569603 python-runit-0.2.0/runit/templates/php/
+-rw-rw-rw-   0        0        0       12 2022-09-03 23:35:52.000000 python-runit-0.2.0/runit/templates/php/.env
+-rw-rw-rw-   0        0        0      277 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/php/composer.json
+-rw-rw-rw-   0        0        0      227 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/templates/php/index.php
+-rw-rw-rw-   0        0        0      392 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/templates/php/request.php
+-rw-rw-rw-   0        0        0      262 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/php/runit.json
+-rw-rw-rw-   0        0        0       27 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/templates/php/test.php
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:08.809605 python-runit-0.2.0/runit/templates/python/
+-rw-rw-rw-   0        0        0       18 2022-09-03 23:35:52.000000 python-runit-0.2.0/runit/templates/python/.env
+-rw-rw-rw-   0        0        0     1182 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/templates/python/application.py
+-rw-rw-rw-   0        0        0      363 2023-05-28 11:17:41.000000 python-runit-0.2.0/runit/templates/python/requirements.txt
+-rw-rw-rw-   0        0        0      275 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/python/runit.json
+-rw-rw-rw-   0        0        0      266 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/templates/runit.json
+-rw-rw-rw-   0        0        0      404 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/test.py
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:07.033948 python-runit-0.2.0/runit/tools/
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:09.055606 python-runit-0.2.0/runit/tools/javascript/
+-rw-rw-rw-   0        0        0      250 2023-04-30 18:54:45.000000 python-runit-0.2.0/runit/tools/javascript/loader.js
+-rw-rw-rw-   0        0        0      490 2023-04-30 20:06:25.000000 python-runit-0.2.0/runit/tools/javascript/runner.js
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:09.213602 python-runit-0.2.0/runit/tools/php/
+-rw-rw-rw-   0        0        0      362 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/tools/php/loader.php
+-rw-rw-rw-   0        0        0      630 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/tools/php/runner.php
+drwxrwxrwx   0        0        0        0 2023-05-28 17:04:09.280607 python-runit-0.2.0/runit/tools/python/
+-rw-rw-rw-   0        0        0      380 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/tools/python/loader.py
+-rw-rw-rw-   0        0        0      639 2022-11-16 16:12:51.000000 python-runit-0.2.0/runit/tools/python/runner.py
+-rw-rw-rw-   0        0        0       42 2023-05-28 17:04:09.295609 python-runit-0.2.0/setup.cfg
+-rw-rw-rw-   0        0        0     1456 2023-05-28 16:59:31.000000 python-runit-0.2.0/setup.py
```

### Comparing `python-runit-0.1.0/LICENSE` & `python-runit-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/PKG-INFO` & `python-runit-0.2.0/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-runit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit/
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Runit CLI ![Python](https://img.shields.io/badge/builthwith-python-brightgreen) 
 The Runit Command Line Interface (CLI) Tools can be used to test, manage, and deploy your Runit project from the command line.
 - Create new runit project
 - Run a local web server for your runit project
 - publish code and assets to your runit-server domain
```

### Comparing `python-runit-0.1.0/README.md` & `python-runit-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/python_runit.egg-info/PKG-INFO` & `python-runit-0.2.0/python_runit.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: python-runit
-Version: 0.1.0
+Version: 0.2.0
 Summary: Develop serverless applications
 Author: Amos Amissah
 Author-email: theonlyamos@gmail.com
 Project-URL: Source, https://github.com/theonlyamos/runit/
 Project-URL: Tracker, https://github.com/theonlyamos/runit/issues
 Keywords: python3 runit developer serverless architecture docker
 Classifier: Development Status :: 3 - Alpha
@@ -13,14 +13,15 @@
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # Runit CLI ![Python](https://img.shields.io/badge/builthwith-python-brightgreen) 
 The Runit Command Line Interface (CLI) Tools can be used to test, manage, and deploy your Runit project from the command line.
 - Create new runit project
 - Run a local web server for your runit project
 - publish code and assets to your runit-server domain
```

### Comparing `python-runit-0.1.0/python_runit.egg-info/SOURCES.txt` & `python-runit-0.2.0/python_runit.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/Request.py` & `python-runit-0.2.0/runit/Request.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/cli.py` & `python-runit-0.2.0/runit/cli.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,38 +1,52 @@
 import os
 import sys
 import shelve
 import getpass
 import argparse
-from typing import Type
+from typing import Type, Optional
 
-from flask import Flask, request
+from fastapi import FastAPI, Request
 from dotenv import load_dotenv, set_key, find_dotenv, dotenv_values
 
 from .languages import LanguageParser
 from .modules import Account
 from .runit import RunIt
 
 from .constants import VERSION, CURRENT_PROJECT, CURRENT_PROJECT_DIR, EXT_TO_RUNTIME, \
                         LANGUAGE_TO_RUNTIME
 
 load_dotenv()
 
 def StartWebserver(project: Type[RunIt], host: str = '127.0.0.1', port: int = 5000):
-    app = Flask(__name__)
-    app.secret = "fdakfjlfdsaflfkjbasdoiefanckdareafasdfkowadbfakidfadfkj"
+    app = FastAPI()
+    app.secret_key = "fdakfjlfdsaflfkjbasdoiefanckdareafasdfkowadbfakidfadfkj"
+    
+    @app.api_route('/')
+    @app.api_route('/{func}')
+    @app.api_route('/{func}/')
+    async def serve(func: Optional[str], request: Request):
+        if request.method.lower() in ['get', 'post']:
+            func = func if func else 'index'
+            params = list(request.query_params.values())
+            return project.serve(func, params) \
+                if len(params) else project.serve(func)
+        return 'MethodNodAllowed'
+
+    
     try:
-        app.add_url_rule('/', view_func=project.serve)
-        app.add_url_rule('/<func>', view_func=project.serve)
-        app.add_url_rule('/<func>/', view_func=project.serve)
-        app.run(host, port, False)
+        import uvicorn
+        uvicorn.run(app, host=host, port=port)
     except KeyboardInterrupt:
+        import sys
         sys.exit(1)
     except Exception as e:
         print(e)
+        import sys
+        sys.exit(1)
 
 def create_new_project(args):
     global CONFIG_FILE
     global CURRENT_PROJECT
     '''
     Method for creating new project or
     function from command line arguments
```

### Comparing `python-runit-0.1.0/runit/constants.py` & `python-runit-0.2.0/runit/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 import os
 from dotenv import load_dotenv
 
 load_dotenv()
 
-VERSION = "0.1.0"
+VERSION = "0.2.0"
 CURRENT_PROJECT = ""
 NOT_FOUND_FILE = '404.html'
 DOT_RUNIT_IGNORE = '.runitignore'
 CONFIG_FILE = 'runit.json'
 STARTER_CONFIG_FILE = 'runit.json'
 IS_RUNNING = False
 CURRENT_PROJECT_DIR = os.path.realpath(os.curdir)
```

### Comparing `python-runit-0.1.0/runit/languages/__init__.py` & `python-runit-0.2.0/runit/languages/__init__.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/languages/multi.py` & `python-runit-0.2.0/runit/languages/multi.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/languages/runtime.py` & `python-runit-0.2.0/runit/languages/runtime.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/modules/account.py` & `python-runit-0.2.0/runit/modules/account.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/runit.py` & `python-runit-0.2.0/runit/runit.py`

 * *Files 2% similar despite different names*

```diff
@@ -158,27 +158,22 @@
     
     def get_functions(self)->list:
         lang_parser = LanguageParser.detect_language(self.start_file, self.runtime)
         return lang_parser.list_functions()
     
     def serve(self, func: str = 'index', args: Optional[Union[dict,list]]=None, filename: str = ''):
         global NOT_FOUND_FILE
-        global request
         
         lang_parser = LanguageParser.detect_language(self.start_file, self.runtime)
         setattr(lang_parser, 'current_func', func)
 
-        if not args and request:
-            args = dict(request.args)
-
-        args_list = args if type(args) == list else []
-        
         if type(args) == dict:
-            for key, value in args.items():
-                args_list.append(value)
+            args = list(args.values())
+
+        args_list = args if type(args) == list  else []
         
         try:
             return getattr(lang_parser, func)(*args_list)
         except AttributeError as e:
             return RunIt.notfound()
             # return f"Function with name '{func}' not defined!"
         except TypeError as e:
```

### Comparing `python-runit-0.1.0/runit/templates/404.html` & `python-runit-0.2.0/runit/templates/404.html`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/templates/multi/application.py` & `python-runit-0.2.0/runit/templates/multi/application.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/templates/python/application.py` & `python-runit-0.2.0/runit/templates/python/application.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/tools/php/runner.php` & `python-runit-0.2.0/runit/tools/php/runner.php`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/runit/tools/python/runner.py` & `python-runit-0.2.0/runit/tools/python/runner.py`

 * *Files identical despite different names*

### Comparing `python-runit-0.1.0/setup.py` & `python-runit-0.2.0/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,26 +1,26 @@
 from importlib.metadata import entry_points
 from setuptools import setup, find_packages
 
-VERSION = '0.1.0'
+VERSION = '0.2.0'
 
 with open('README.md', 'rt') as file:
     LONG_DESCRIPTION = file.read()
 
 setup(
     name='python-runit',
     version=VERSION,
     author='Amos Amissah',
     author_email='theonlyamos@gmail.com',
     description='Develop serverless applications',
     long_description=LONG_DESCRIPTION,
+    long_description_content_type = "text/markdown",
     packages=find_packages(),
     include_package_data=True,
-    install_requires=['requests','python-dotenv','flask','flask-jwt-extended',
-    'flask-restful'],
+    install_requires=['requests','python-dotenv','fastapi','passlib'],
     keywords='python3 runit developer serverless architecture docker',
     project_urls={
         'Source': 'https://github.com/theonlyamos/runit/',
         'Tracker': 'https://github.com/theonlyamos/runit/issues',
     },
     classifiers=[
         'Development Status :: 3 - Alpha',
```

