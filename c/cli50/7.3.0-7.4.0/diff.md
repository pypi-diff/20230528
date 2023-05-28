# Comparing `tmp/cli50-7.3.0.tar.gz` & `tmp/cli50-7.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/runner/work/cli50/cli50/dist/tmp5klij7j8/cli50-7.3.0.tar", last modified: Wed Sep 21 03:45:16 2022, max compression
+gzip compressed data, was "cli50-7.4.0.tar", last modified: Sun May 28 14:24:32 2023, max compression
```

## Comparing `cli50-7.3.0.tar` & `cli50-7.4.0.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:45:16.000000 cli50-7.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)      848 2022-09-21 03:44:55.000000 cli50-7.3.0/setup.py
--rw-r--r--   0 runner    (1001) docker     (121)       33 2022-09-21 03:44:55.000000 cli50-7.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)      386 2022-09-21 03:45:16.000000 cli50-7.3.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      334 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        6 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       47 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       25 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50.egg-info/PKG-INFO
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50/locale/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50/locale/es/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-09-21 03:45:16.000000 cli50-7.3.0/cli50/locale/es/LC_MESSAGES/
--rw-r--r--   0 runner    (1001) docker     (121)     1465 2022-09-21 03:44:55.000000 cli50-7.3.0/cli50/locale/es/LC_MESSAGES/cli50.po
--rw-r--r--   0 runner    (1001) docker     (121)     1519 2022-09-21 03:45:06.000000 cli50-7.3.0/cli50/locale/es/LC_MESSAGES/cli50.mo
--rw-r--r--   0 runner    (1001) docker     (121)    12104 2022-09-21 03:44:55.000000 cli50-7.3.0/cli50/__main__.py
--rw-r--r--   0 runner    (1001) docker     (121)      588 2022-09-21 03:44:55.000000 cli50-7.3.0/cli50/__init__.py
--rw-r--r--   0 runner    (1001) docker     (121)    35149 2022-09-21 03:44:55.000000 cli50-7.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      219 2022-09-21 03:44:55.000000 cli50-7.3.0/README.md
--rw-r--r--   0 runner    (1001) docker     (121)      534 2022-09-21 03:45:16.000000 cli50-7.3.0/PKG-INFO
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:24:32.753034 cli50-7.4.0/
+-rw-r--r--   0 runner    (1001) docker     (123)    35149 2023-05-28 14:24:22.000000 cli50-7.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       33 2023-05-28 14:24:22.000000 cli50-7.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-28 14:24:32.753034 cli50-7.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      114 2023-05-28 14:24:22.000000 cli50-7.4.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:24:32.753034 cli50-7.4.0/cli50/
+-rw-r--r--   0 runner    (1001) docker     (123)      588 2023-05-28 14:24:22.000000 cli50-7.4.0/cli50/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12207 2023-05-28 14:24:22.000000 cli50-7.4.0/cli50/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:24:32.749034 cli50-7.4.0/cli50/locale/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:24:32.749034 cli50-7.4.0/cli50/locale/es/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:24:32.753034 cli50-7.4.0/cli50/locale/es/LC_MESSAGES/
+-rw-r--r--   0 runner    (1001) docker     (123)     1519 2023-05-28 14:24:25.000000 cli50-7.4.0/cli50/locale/es/LC_MESSAGES/cli50.mo
+-rw-r--r--   0 runner    (1001) docker     (123)     1465 2023-05-28 14:24:22.000000 cli50-7.4.0/cli50/locale/es/LC_MESSAGES/cli50.po
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-05-28 14:24:32.753034 cli50-7.4.0/cli50.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      621 2023-05-28 14:24:32.000000 cli50-7.4.0/cli50.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      334 2023-05-28 14:24:32.000000 cli50-7.4.0/cli50.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-05-28 14:24:32.000000 cli50-7.4.0/cli50.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       46 2023-05-28 14:24:32.000000 cli50-7.4.0/cli50.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       25 2023-05-28 14:24:32.000000 cli50-7.4.0/cli50.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        6 2023-05-28 14:24:32.000000 cli50-7.4.0/cli50.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      386 2023-05-28 14:24:32.753034 cli50-7.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      895 2023-05-28 14:24:22.000000 cli50-7.4.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `cli50-7.3.0/setup.py` & `cli50-7.4.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,20 +9,21 @@
         "Programming Language :: Python :: 3.6",
         "Topic :: Software Development"
     ],
     message_extractors = {
         'cli50': [('**.py', 'python', None),],
     },
     description="This is CS50 CLI, with which you can mount a directory inside of an Ubuntu container.",
+    long_description=open("README.md").read(),
     license="GPLv3",
     install_requires=["inflect", "requests", "tzlocal"],
     keywords="cli50",
     name="cli50",
-    python_requires=">=3.6",
+    python_requires=">=3.8",
     packages=["cli50"],
     entry_points={
         "console_scripts": ["cli50=cli50.__main__:main"]
     },
     url="https://github.com/cs50/cli50",
-    version="7.3.0",
+    version="7.4.0",
     include_package_data=True
 )
```

### Comparing `cli50-7.3.0/cli50/locale/es/LC_MESSAGES/cli50.po` & `cli50-7.4.0/cli50/locale/es/LC_MESSAGES/cli50.po`

 * *Files identical despite different names*

### Comparing `cli50-7.3.0/cli50/locale/es/LC_MESSAGES/cli50.mo` & `cli50-7.4.0/cli50/locale/es/LC_MESSAGES/cli50.mo`

 * *Files 7% similar despite different names*

#### msgunfmt {}

```diff
@@ -1,21 +1,21 @@
 msgid ""
 msgstr ""
 "Project-Id-Version: PROJECT VERSION\n"
 "Report-Msgid-Bugs-To: EMAIL@ADDRESS\n"
-"POT-Creation-Date: 2022-09-21 03:45+0000\n"
+"POT-Creation-Date: 2023-05-28 14:24+0000\n"
 "PO-Revision-Date: YEAR-MO-DA HO:MI+ZONE\n"
 "Last-Translator: FULL NAME <EMAIL@ADDRESS>\n"
 "Language: es\n"
 "Language-Team: es <LL@li.org>\n"
 "Plural-Forms: nplurals=2; plural=(n != 1);\n"
 "MIME-Version: 1.0\n"
 "Content-Type: text/plain; charset=utf-8\n"
 "Content-Transfer-Encoding: 8bit\n"
-"Generated-By: Babel 2.10.3\n"
+"Generated-By: Babel 2.12.1\n"
 
 msgid " with {} mounted"
 msgstr " con {} montado"
 
 msgid "CS50 CLI requires Python 3.6 or higher"
 msgstr "Necesitas Python 3.6 o una versión más reciente para usar CS50 CLI"
```

### Comparing `cli50-7.3.0/cli50/__main__.py` & `cli50-7.4.0/cli50/__main__.py`

 * *Files 1% similar despite different names*

```diff
@@ -211,14 +211,18 @@
                "--label", LABEL,
                "--rm",
                "--security-opt", "seccomp=unconfined",  # https://stackoverflow.com/q/35860527#comment62818827_35860527, https://github.com/apple/swift-docker/issues/9#issuecomment-328218803
                "--tty",
                "--volume", directory + ":" + workdir,
                "--workdir", workdir]
 
+    # Check for locale
+    if lang := os.getenv("LANG"):
+        options += ["--env", f"LANG={lang}"]
+
     # Validate ports
     if not args["port"]:
         args["port"] = PORTS
     for port in args["port"]:
         if port < 1024 or port > 65535:
             sys.exit(f"Invalid port: {port}")
         options += ["--expose", f"{port}"]
```

### Comparing `cli50-7.3.0/cli50/__init__.py` & `cli50-7.4.0/cli50/__init__.py`

 * *Files identical despite different names*

### Comparing `cli50-7.3.0/LICENSE` & `cli50-7.4.0/LICENSE`

 * *Files identical despite different names*

