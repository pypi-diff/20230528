# Comparing `tmp/django_copilot-0.1.0.tar.gz` & `tmp/django_copilot-0.2.0a1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django_copilot-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "django_copilot-0.2.0a1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `django_copilot-0.1.0.tar` & `django_copilot-0.2.0a1.tar`

### file list

```diff
@@ -1,3 +1,3 @@
--rw-r--r--   0        0        0       70 2023-05-28 09:40:01.463590 django_copilot-0.1.0/copilot/__init__.py
--rw-r--r--   0        0        0      282 2023-05-28 09:43:40.018035 django_copilot-0.1.0/pyproject.toml
--rw-r--r--   0        0        0      198 1970-01-01 00:00:00.000000 django_copilot-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0       72 2023-05-28 10:39:24.285253 django_copilot-0.2.0a1/copilot/__init__.py
+-rw-r--r--   0        0        0      282 2023-05-28 09:43:40.018035 django_copilot-0.2.0a1/pyproject.toml
+-rw-r--r--   0        0        0      200 1970-01-01 00:00:00.000000 django_copilot-0.2.0a1/PKG-INFO
```

