# Comparing `tmp/anisha_vehicles-0.2.3.tar.gz` & `tmp/anisha_vehicles-0.2.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anisha_vehicles-0.2.3.tar", max compression
+gzip compressed data, was "anisha_vehicles-0.2.4.tar", max compression
```

## Comparing `anisha_vehicles-0.2.3.tar` & `anisha_vehicles-0.2.4.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       22 2023-05-25 12:07:57.873334 anisha_vehicles-0.2.3/README.md
--rw-r--r--   0        0        0      319 2023-05-28 12:33:09.951346 anisha_vehicles-0.2.3/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-25 12:20:18.757722 anisha_vehicles-0.2.3/src/anisha_vehicles/__init__.py
--rw-r--r--   0        0        0      515 2023-05-25 12:43:57.294272 anisha_vehicles-0.2.3/src/anisha_vehicles/new_car.py
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 anisha_vehicles-0.2.3/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-25 12:07:57.873334 anisha_vehicles-0.2.4/README.md
+-rw-r--r--   0        0        0      319 2023-05-28 20:38:54.242696 anisha_vehicles-0.2.4/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-25 12:20:18.757722 anisha_vehicles-0.2.4/src/anisha_vehicles/__init__.py
+-rw-r--r--   0        0        0      515 2023-05-25 12:43:57.294272 anisha_vehicles-0.2.4/src/anisha_vehicles/new_car.py
+-rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 anisha_vehicles-0.2.4/PKG-INFO
```

### Comparing `anisha_vehicles-0.2.3/src/anisha_vehicles/new_car.py` & `anisha_vehicles-0.2.4/src/anisha_vehicles/new_car.py`

 * *Files identical despite different names*

