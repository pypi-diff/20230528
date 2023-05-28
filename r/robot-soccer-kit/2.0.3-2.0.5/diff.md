# Comparing `tmp/robot-soccer-kit-2.0.3.tar.gz` & `tmp/robot-soccer-kit-2.0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "robot-soccer-kit-2.0.3.tar", last modified: Sat Apr 29 10:42:48 2023, max compression
+gzip compressed data, was "robot-soccer-kit-2.0.5.tar", last modified: Sun May 28 13:09:42 2023, max compression
```

## Comparing `robot-soccer-kit-2.0.3.tar` & `robot-soccer-kit-2.0.5.tar`

### file list

```diff
@@ -1,162 +1,164 @@
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/LICENSE
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/README.md
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.008063 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/PKG-INFO
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4847 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/SOURCES.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/dependency_links.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       82 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/requires.txt
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2023-04-29 10:42:47.000000 robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/top_level.txt
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.008063 robot-soccer-kit-2.0.3/rsk/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/__init__.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/api.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5422 2023-04-29 10:15:19.000000 robot-soccer-kit-2.0.3/rsk/backend.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10937 2023-04-29 10:28:28.000000 robot-soccer-kit-2.0.3/rsk/client.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/config.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3225 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/constants.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13513 2023-04-29 10:23:15.000000 robot-soccer-kit-2.0.3/rsk/control.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       35 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/debug.sh
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.0.3/rsk/detection.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/dumb_ia.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/dump_referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       73 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/em.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/field.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2379 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/game_controller.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/kinematics.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/logger.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/place.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    23541 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/referee.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2362 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/robot.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11752 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/robot_serial.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/robots.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10231 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/simulator.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/state.py
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.008063 robot-soccer-kit-2.0.3/rsk/static/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.008063 robot-soccer-kit-2.0.3/rsk/static/bootstrap/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.016063 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.min.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.css.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.min.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.020063 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.min.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.min.js.map
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/camera-setting.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.020063 robot-soccer-kit-2.0.3/rsk/static/css/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2566 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/css/app.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/favicon.ico
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.020063 robot-soccer-kit-2.0.3/rsk/static/icons/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.browserslistrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.editorconfig
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.eslintignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.eslintrc.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.fantasticonrc.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.gitattributes
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/.github/
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/.github/ISSUE_TEMPLATE/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/dependabot.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/preview.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/release-drafter.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/codeql.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/deploy.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/release-notes.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/test.yml
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.gitignore
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/.stylelintrc
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/LICENSE.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/README.md
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/bootstrap-icons.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/composer.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/config.yml
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/font/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/bootstrap-icons.css
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/bootstrap-icons.json
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/bootstrap-icons.woff
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/bootstrap-icons.woff2
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/font/index.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/package-lock.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/package.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/svg-sprite.json
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/icons/svgo.config.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.024063 robot-soccer-kit-2.0.3/rsk/static/imgs/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_16x16.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_24x24.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_256x256.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_32x32.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/ball_48x48.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/field.png
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/field.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robot.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robotblue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robotblue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robotgreen1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/imgs/robotgreen2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    26782 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/index.html
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/rsk/static/jquery/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/jquery/jquery.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/rsk/static/js/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1614 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/js/app.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1567 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/js/control.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    24647 2023-04-29 10:29:12.000000 robot-soccer-kit-2.0.3/rsk/static/js/referee.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/js/robots.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/js/tabs.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/js/utils.js
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5996 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/js/video.js
-drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/rsk/static/markers/
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/markers/blue1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/markers/blue2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/markers/green1.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/markers/green2.svg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/referee_event_neutral.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/referee_event_team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/static/robot.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.3/rsk/static/team.html
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3865 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/tasks.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/utils.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.3/rsk/video.py
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-04-29 10:42:48.028063 robot-soccer-kit-2.0.3/setup.cfg
--rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1391 2023-04-29 10:42:22.000000 robot-soccer-kit-2.0.3/setup.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.740067 robot-soccer-kit-2.0.5/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      262 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/LICENSE
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-05-28 13:09:42.740067 robot-soccer-kit-2.0.5/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      588 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/README.md
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.724067 robot-soccer-kit-2.0.5/robot_soccer_kit.egg-info/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1157 2023-05-28 13:09:42.000000 robot-soccer-kit-2.0.5/robot_soccer_kit.egg-info/PKG-INFO
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4903 2023-05-28 13:09:42.000000 robot-soccer-kit-2.0.5/robot_soccer_kit.egg-info/SOURCES.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        1 2023-05-28 13:09:42.000000 robot-soccer-kit-2.0.5/robot_soccer_kit.egg-info/dependency_links.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       82 2023-05-28 13:09:42.000000 robot-soccer-kit-2.0.5/robot_soccer_kit.egg-info/requires.txt
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)        4 2023-05-28 13:09:42.000000 robot-soccer-kit-2.0.5/robot_soccer_kit.egg-info/top_level.txt
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.724067 robot-soccer-kit-2.0.5/rsk/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      102 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/__init__.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/api.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5422 2023-04-29 10:15:19.000000 robot-soccer-kit-2.0.5/rsk/backend.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10981 2023-05-28 13:09:30.000000 robot-soccer-kit-2.0.5/rsk/client.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      277 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/config.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3224 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.5/rsk/constants.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13616 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.5/rsk/control.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       35 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/debug.sh
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    18552 2023-04-29 10:39:09.000000 robot-soccer-kit-2.0.5/rsk/detection.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1058 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/dumb_ia.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      571 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/dump_referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       73 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/em.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10173 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/field.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2379 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/game_controller.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2462 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/kinematics.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      445 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/logger.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      602 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/place.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    23624 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.5/rsk/referee.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2362 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/robot.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11752 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/robot_serial.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6030 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/robots.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    10231 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/simulator.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2321 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/state.py
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.724067 robot-soccer-kit-2.0.5/rsk/static/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.720067 robot-soccer-kit-2.0.5/rsk/static/bootstrap/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.732067 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75616 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226018 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56464 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142342 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    75690 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   226022 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    56539 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   142419 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11735 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126626 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9817 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    51406 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    11728 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   126641 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9889 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    63643 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96254 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250681 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163881 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    96121 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   250622 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   163716 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267476 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658460 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220780 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   568408 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.min.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   267055 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.rtl.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   658305 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.rtl.css.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   220887 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.rtl.min.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   567947 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.732067 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   208288 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.bundle.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   448884 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.bundle.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80599 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.bundle.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   333974 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   136243 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.esm.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   305274 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.esm.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    74135 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.esm.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   222070 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.esm.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   145819 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   306458 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    60554 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.min.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   217885 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.min.js.map
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      215 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/camera-setting.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.732067 robot-soccer-kit-2.0.5/rsk/static/css/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2566 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/css/app.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1150 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/favicon.ico
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.736067 robot-soccer-kit-2.0.5/rsk/static/icons/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      376 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.browserslistrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      167 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.editorconfig
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       40 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.eslintignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      375 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.eslintrc.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      922 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.fantasticonrc.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       43 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.gitattributes
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.736067 robot-soccer-kit-2.0.5/rsk/static/icons/.github/
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.736067 robot-soccer-kit-2.0.5/rsk/static/icons/.github/ISSUE_TEMPLATE/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      583 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      122 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.github/ISSUE_TEMPLATE/icon-request.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      433 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.github/dependabot.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   248086 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.github/preview.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      572 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.github/release-drafter.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.736067 robot-soccer-kit-2.0.5/rsk/static/icons/.github/workflows/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      662 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.github/workflows/codeql.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1190 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.github/workflows/deploy.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      243 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.github/workflows/release-notes.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      575 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.github/workflows/test.yml
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       63 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.gitignore
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      125 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/.stylelintrc
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1093 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/LICENSE.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3312 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/README.md
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   881772 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/bootstrap-icons.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      425 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/composer.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2052 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/config.yml
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.736067 robot-soccer-kit-2.0.5/rsk/static/icons/font/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    80510 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/font/bootstrap-icons.css
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    42897 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/font/bootstrap-icons.json
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.736067 robot-soccer-kit-2.0.5/rsk/static/icons/font/fonts/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   137124 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/font/fonts/bootstrap-icons.woff
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   102536 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/font/fonts/bootstrap-icons.woff2
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   200995 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/font/index.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   643115 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/package-lock.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3152 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/package.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3085 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/svg-sprite.json
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/icons/svgo.config.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.740067 robot-soccer-kit-2.0.5/rsk/static/imgs/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3287 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/ball.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1251 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/ball_16x16.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1856 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/ball_24x24.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    43069 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/ball_256x256.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     2654 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/ball_32x32.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4470 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/ball_48x48.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    19402 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/field.png
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    17815 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/field.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   249649 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/robot.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   507520 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/robotblue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   524385 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/robotblue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   498488 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/robotgreen1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   522425 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/imgs/robotgreen2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    34869 2023-05-13 07:41:39.000000 robot-soccer-kit-2.0.5/rsk/static/index.html
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.740067 robot-soccer-kit-2.0.5/rsk/static/jquery/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)   288580 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/jquery/jquery.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.740067 robot-soccer-kit-2.0.5/rsk/static/js/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1714 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.5/rsk/static/js/app.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1713 2023-05-12 17:27:02.000000 robot-soccer-kit-2.0.5/rsk/static/js/competition.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1567 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/js/control.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13460 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.5/rsk/static/js/referee.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6005 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/js/robots.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)    13772 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.5/rsk/static/js/simulator.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      426 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/js/tabs.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      329 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/js/utils.js
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5997 2023-05-13 07:36:16.000000 robot-soccer-kit-2.0.5/rsk/static/js/video.js
+drwxrwxr-x   0 gregwar   (1000) gregwar   (1000)        0 2023-05-28 13:09:42.740067 robot-soccer-kit-2.0.5/rsk/static/markers/
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6021 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/markers/blue1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6023 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/markers/blue2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     6009 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/markers/green1.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     5098 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/markers/green2.svg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      337 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/referee_event_neutral.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      632 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/referee_event_team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1029 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/static/robot.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)      569 2022-09-27 10:59:02.000000 robot-soccer-kit-2.0.5/rsk/static/team.html
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     3865 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/tasks.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     4154 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/utils.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     9469 2023-04-29 10:06:21.000000 robot-soccer-kit-2.0.5/rsk/video.py
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)       38 2023-05-28 13:09:42.740067 robot-soccer-kit-2.0.5/setup.cfg
+-rw-rw-r--   0 gregwar   (1000) gregwar   (1000)     1391 2023-05-28 13:09:34.000000 robot-soccer-kit-2.0.5/setup.py
```

### Comparing `robot-soccer-kit-2.0.3/PKG-INFO` & `robot-soccer-kit-2.0.5/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.0.3
+Version: 2.0.5
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.0.3/README.md` & `robot-soccer-kit-2.0.5/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/PKG-INFO` & `robot-soccer-kit-2.0.5/robot_soccer_kit.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: robot-soccer-kit
-Version: 2.0.3
+Version: 2.0.5
 Summary: Robot Soccer Kit
 Home-page: https://github.com/rhoban/robot-soccer-kit/
 Author: Rhoban team
 Author-email: team@rhoban.com
 License: UNKNOWN
 Keywords: robot holonomic omniwheel ssl robocup junior soccer standard localized tracking
 Platform: UNKNOWN
```

### Comparing `robot-soccer-kit-2.0.3/robot_soccer_kit.egg-info/SOURCES.txt` & `robot-soccer-kit-2.0.5/robot_soccer_kit.egg-info/SOURCES.txt`

 * *Files 1% similar despite different names*

```diff
@@ -126,17 +126,19 @@
 rsk/static/imgs/robot.svg
 rsk/static/imgs/robotblue1.svg
 rsk/static/imgs/robotblue2.svg
 rsk/static/imgs/robotgreen1.svg
 rsk/static/imgs/robotgreen2.svg
 rsk/static/jquery/jquery.js
 rsk/static/js/app.js
+rsk/static/js/competition.js
 rsk/static/js/control.js
 rsk/static/js/referee.js
 rsk/static/js/robots.js
+rsk/static/js/simulator.js
 rsk/static/js/tabs.js
 rsk/static/js/utils.js
 rsk/static/js/video.js
 rsk/static/markers/blue1.svg
 rsk/static/markers/blue2.svg
 rsk/static/markers/green1.svg
 rsk/static/markers/green2.svg
```

### Comparing `robot-soccer-kit-2.0.3/rsk/api.py` & `robot-soccer-kit-2.0.5/rsk/api.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/backend.py` & `robot-soccer-kit-2.0.5/rsk/backend.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/client.py` & `robot-soccer-kit-2.0.5/rsk/client.py`

 * *Files 3% similar despite different names*

```diff
@@ -164,15 +164,14 @@
         self.robots = {}
 
         # Declaring stubs for auto completion
         self.green1: ClientRobot
         self.green2: ClientRobot
         self.blue1: ClientRobot
         self.blue2: ClientRobot
-        self.ballObject: ClientRobot = ClientRobot("ball", 0, self)
 
         # Creating self.green1, self.green2 etc.
         for color, number in utils.all_robots():
             robot_id = utils.robot_list2str(color, number)
             robot = ClientRobot(color, number, self)
             self.__dict__[robot_id] = robot
 
@@ -282,14 +281,17 @@
     def em(self):
         self.stop_motion()
 
     def stop(self):
         self.stop_motion()
         self.running = False
 
+    def teleport_ball(self, x: float, y: float):
+        return self.command("ball", 0, "teleport", [x, y, 0])
+
     def command(self, color, number, name, parameters):
         if threading.current_thread() is threading.main_thread():
             sigint_handler = signal.getsignal(signal.SIGINT)
             signal.signal(signal.SIGINT, signal.SIG_IGN)
         self.lock.acquire()
         self.req.send_json([self.key, color, number, [name, *parameters]])
         success, message = self.req.recv_json()
```

### Comparing `robot-soccer-kit-2.0.3/rsk/constants.py` & `robot-soccer-kit-2.0.5/rsk/constants.py`

 * *Files 1% similar despite different names*

```diff
@@ -25,16 +25,16 @@
 dots_y: float = 0.305  # [m]
 
 # Defense area
 defense_area_width = 0.9  # [m]
 defense_area_length = 0.3  # [m]
 
 # Timed circle radius and maximum time before being penalized
-timed_circle_radius: float = 0.25  # [s]
-timed_circle_time: float = 5  # [s]
+timed_circle_radius: float = 0.25  # [m]
+timed_circle_time: float = 3 # [s]
 
 # Margin for ball re-placement (on the center or on dots)
 place_ball_margin: float = 0.05  # [m]
 
 # Margins for being in and out the field
 field_in_margin: float = -0.08  # [m]
 field_out_margin: float = 0.02  # [m]
```

### Comparing `robot-soccer-kit-2.0.3/rsk/control.py` & `robot-soccer-kit-2.0.5/rsk/control.py`

 * *Files 1% similar despite different names*

```diff
@@ -118,14 +118,17 @@
             elif marker == "ball":
                 self.robots.ball.teleport(float(command[1]), float(command[2]), float(command[3]))
                 response = [True, "ok"]
             else:
                 response[1] = f"Unknown robot: {marker}"
         except RobotError as e:
             response = [False, str(e)]
+        except (TypeError, ValueError) as e:
+            response = [False, "ArgumentError: "+str(e)]
+
 
         return response
 
     def thread(self):
         """
         Main control loop, process commands received from the API
         """
```

### Comparing `robot-soccer-kit-2.0.3/rsk/detection.py` & `robot-soccer-kit-2.0.5/rsk/detection.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/dumb_ia.py` & `robot-soccer-kit-2.0.5/rsk/dumb_ia.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/dump_referee.py` & `robot-soccer-kit-2.0.5/rsk/dump_referee.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/field.py` & `robot-soccer-kit-2.0.5/rsk/field.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/game_controller.py` & `robot-soccer-kit-2.0.5/rsk/game_controller.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/kinematics.py` & `robot-soccer-kit-2.0.5/rsk/kinematics.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/place.py` & `robot-soccer-kit-2.0.5/rsk/place.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/referee.py` & `robot-soccer-kit-2.0.5/rsk/referee.py`

 * *Files 1% similar despite different names*

```diff
@@ -185,14 +185,15 @@
         """
         Stop the game (end)
         """
         self.logger.info("Game stopped")
         self.game_state["game_paused"] = True
         self.game_state["game_is_running"] = False
         self.chrono_is_running = False
+        self.wait_ball_position = None
         self.start_timer = 0.0
 
         self.reset_penalties()
         self.control.remove_task("manually-paused")
         self.control.remove_task("sideline-crossed")
         self.control.remove_task("goal")
         self.control.remove_task("game-start")
@@ -382,15 +383,19 @@
         * It has no other tasks to do (it is not preempted)
 
         :param str robot: robot
         :return bool: True if the robot can be penalized
         """
         tasks = self.control.robot_tasks(*utils.robot_str2list(robot))
 
-        return len(tasks) == 0 and (self.penalties[robot]["remaining"] is None) and (self.penalties[robot]["grace"] is None)
+        return (
+            len(tasks) == 0
+            and (self.penalties[robot]["remaining"] is None)
+            and (self.penalties[robot]["grace"] is None)
+        )
 
     def set_team_name(self, team: str, name: str):
         self.game_state["teams"][team]["name"] = name
 
     def swap_team_sides(self):
         """
         Swap team sides (x positive referring to the team defending goals on the
@@ -518,16 +523,16 @@
 
                 # Penalizing extra robots that are entering the defense area
                 if self.can_be_penalized(marker):
                     my_defense_area = constants.defense_area(self.positive_team == team)
                     opponent_defense_area = constants.defense_area(self.positive_team != team)
 
                     # This is penalizing robots for abusive attack (suspended)
-                    # if utils.in_rectangle(robot_position, *opponent_defense_area):
-                    #     self.add_penalty(constants.default_penalty, marker, "abusive_attack")
+                    if utils.in_rectangle(robot_position, *opponent_defense_area):
+                        self.add_penalty(constants.default_penalty, marker, "abusive_attack")
 
                     if utils.in_rectangle(robot_position, *my_defense_area):
                         if team in defender:
                             other_robot, other_robot_position = defender[team]
                             robot_to_penalize = marker
 
                             if abs(other_robot_position[0]) < abs(robot_position[0]):
```

### Comparing `robot-soccer-kit-2.0.3/rsk/robot.py` & `robot-soccer-kit-2.0.5/rsk/robot.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/robot_serial.py` & `robot-soccer-kit-2.0.5/rsk/robot_serial.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/robots.py` & `robot-soccer-kit-2.0.5/rsk/robots.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/simulator.py` & `robot-soccer-kit-2.0.5/rsk/simulator.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/state.py` & `robot-soccer-kit-2.0.5/rsk/state.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.min.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.min.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-grid.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.min.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-reboot.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.min.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap-utilities.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.min.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.min.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.rtl.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.rtl.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.min.css` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.rtl.min.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/css/bootstrap.rtl.min.css.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.js` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.bundle.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.js.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.bundle.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.min.js` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.bundle.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.bundle.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.js` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.esm.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.js.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.esm.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.min.js` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.esm.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.esm.min.js.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.esm.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.js` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.js.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.min.js` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.min.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/bootstrap/js/bootstrap.min.js.map` & `robot-soccer-kit-2.0.5/rsk/static/bootstrap/js/bootstrap.min.js.map`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/css/app.css` & `robot-soccer-kit-2.0.5/rsk/static/css/app.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/favicon.ico` & `robot-soccer-kit-2.0.5/rsk/static/favicon.ico`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/.fantasticonrc.js` & `robot-soccer-kit-2.0.5/rsk/static/icons/.fantasticonrc.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md` & `robot-soccer-kit-2.0.5/rsk/static/icons/.github/ISSUE_TEMPLATE/bug_report.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/.github/preview.png` & `robot-soccer-kit-2.0.5/rsk/static/icons/.github/preview.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/.github/release-drafter.yml` & `robot-soccer-kit-2.0.5/rsk/static/icons/.github/release-drafter.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/codeql.yml` & `robot-soccer-kit-2.0.5/rsk/static/icons/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/deploy.yml` & `robot-soccer-kit-2.0.5/rsk/static/icons/.github/workflows/deploy.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/.github/workflows/test.yml` & `robot-soccer-kit-2.0.5/rsk/static/icons/.github/workflows/test.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/LICENSE.md` & `robot-soccer-kit-2.0.5/rsk/static/icons/LICENSE.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/README.md` & `robot-soccer-kit-2.0.5/rsk/static/icons/README.md`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/bootstrap-icons.svg` & `robot-soccer-kit-2.0.5/rsk/static/icons/bootstrap-icons.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/config.yml` & `robot-soccer-kit-2.0.5/rsk/static/icons/config.yml`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/font/bootstrap-icons.css` & `robot-soccer-kit-2.0.5/rsk/static/icons/font/bootstrap-icons.css`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/font/bootstrap-icons.json` & `robot-soccer-kit-2.0.5/rsk/static/icons/font/bootstrap-icons.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/bootstrap-icons.woff` & `robot-soccer-kit-2.0.5/rsk/static/icons/font/fonts/bootstrap-icons.woff`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/font/fonts/bootstrap-icons.woff2` & `robot-soccer-kit-2.0.5/rsk/static/icons/font/fonts/bootstrap-icons.woff2`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/font/index.html` & `robot-soccer-kit-2.0.5/rsk/static/icons/font/index.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/package-lock.json` & `robot-soccer-kit-2.0.5/rsk/static/icons/package-lock.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/package.json` & `robot-soccer-kit-2.0.5/rsk/static/icons/package.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/svg-sprite.json` & `robot-soccer-kit-2.0.5/rsk/static/icons/svg-sprite.json`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/icons/svgo.config.js` & `robot-soccer-kit-2.0.5/rsk/static/icons/svgo.config.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/ball.png` & `robot-soccer-kit-2.0.5/rsk/static/imgs/ball.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_16x16.png` & `robot-soccer-kit-2.0.5/rsk/static/imgs/ball_16x16.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_24x24.png` & `robot-soccer-kit-2.0.5/rsk/static/imgs/ball_24x24.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_256x256.png` & `robot-soccer-kit-2.0.5/rsk/static/imgs/ball_256x256.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_32x32.png` & `robot-soccer-kit-2.0.5/rsk/static/imgs/ball_32x32.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/ball_48x48.png` & `robot-soccer-kit-2.0.5/rsk/static/imgs/ball_48x48.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/field.png` & `robot-soccer-kit-2.0.5/rsk/static/imgs/field.png`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/field.svg` & `robot-soccer-kit-2.0.5/rsk/static/imgs/field.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/robot.svg` & `robot-soccer-kit-2.0.5/rsk/static/imgs/robot.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/robotblue1.svg` & `robot-soccer-kit-2.0.5/rsk/static/imgs/robotblue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/robotblue2.svg` & `robot-soccer-kit-2.0.5/rsk/static/imgs/robotblue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/robotgreen1.svg` & `robot-soccer-kit-2.0.5/rsk/static/imgs/robotgreen1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/imgs/robotgreen2.svg` & `robot-soccer-kit-2.0.5/rsk/static/imgs/robotgreen2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/jquery/jquery.js` & `robot-soccer-kit-2.0.5/rsk/static/jquery/jquery.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/js/app.js` & `robot-soccer-kit-2.0.5/rsk/static/js/app.js`

 * *Files 26% similar despite different names*

#### js-beautify {}

```diff
@@ -33,18 +33,20 @@
 $(document).ready(function() {
     // Backend initialization
     var backend = new APIBackend('http://127.0.0.1:7070/api');
     backend.is_simulated(function(simulated) {
         if (simulated) {
             console.log("SIMULATION")
             $('.not_show_simulated').css("display", 'none')
+            simulator_initialize(backend, true)
         } else {
             console.log("REEL")
             $('.show_simulated').css("display", 'none')
             video_initialize(backend);
+            simulator_initialize(backend, false)
         }
     })
 
     robots_initialize(backend);
     control_initialize(backend);
     referee_initialize(backend);
```

### Comparing `robot-soccer-kit-2.0.3/rsk/static/js/control.js` & `robot-soccer-kit-2.0.5/rsk/static/js/control.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/js/robots.js` & `robot-soccer-kit-2.0.5/rsk/static/js/robots.js`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/js/video.js` & `robot-soccer-kit-2.0.5/rsk/static/js/video.js`

 * *Format-specific differences are supported for JavaScript files but no file-specific differences were detected; falling back to a binary diff. file(1) reports: JavaScript source, ASCII text*

 * *Files 0% similar despite different names*

```diff
@@ -368,8 +368,8 @@
 000016f0: 2729 3b0a 2020 2020 2020 2020 2020 2020  ');.            
 00001700: 7d20 656c 7365 207b 0a20 2020 2020 2020  } else {.       
 00001710: 2020 2020 2020 2020 2024 2827 626f 6479           $('body
 00001720: 2729 2e72 656d 6f76 6543 6c61 7373 2827  ').removeClass('
 00001730: 7669 7369 6f6e 2d6e 6f2d 6572 726f 7227  vision-no-error'
 00001740: 293b 0a20 2020 2020 2020 2020 2020 207d  );.            }
 00001750: 0a0a 0a20 2020 2020 2020 207d 293b 0a20  ...        });. 
-00001760: 2020 207d 2c20 3530 293b 0a7d               }, 50);.}
+00001760: 2020 207d 2c20 3530 293b 0a7d 0a            }, 50);.}.
```

### Comparing `robot-soccer-kit-2.0.3/rsk/static/markers/blue1.svg` & `robot-soccer-kit-2.0.5/rsk/static/markers/blue1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/markers/blue2.svg` & `robot-soccer-kit-2.0.5/rsk/static/markers/blue2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/markers/green1.svg` & `robot-soccer-kit-2.0.5/rsk/static/markers/green1.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/markers/green2.svg` & `robot-soccer-kit-2.0.5/rsk/static/markers/green2.svg`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/referee_event_team.html` & `robot-soccer-kit-2.0.5/rsk/static/referee_event_team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/robot.html` & `robot-soccer-kit-2.0.5/rsk/static/robot.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/static/team.html` & `robot-soccer-kit-2.0.5/rsk/static/team.html`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/tasks.py` & `robot-soccer-kit-2.0.5/rsk/tasks.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/utils.py` & `robot-soccer-kit-2.0.5/rsk/utils.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/rsk/video.py` & `robot-soccer-kit-2.0.5/rsk/video.py`

 * *Files identical despite different names*

### Comparing `robot-soccer-kit-2.0.3/setup.py` & `robot-soccer-kit-2.0.5/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -10,15 +10,15 @@
         for filename in filenames:
             if '__pycache__' not in path:
                 paths.append(os.path.join('..', path, filename))
     return paths
 
 setuptools.setup(
     name="robot-soccer-kit",
-    version="2.0.3",
+    version="2.0.5",
     author="Rhoban team",
     author_email="team@rhoban.com",
     description="Robot Soccer Kit",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/rhoban/robot-soccer-kit/",
     packages=setuptools.find_packages(),
```

