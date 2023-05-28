# Comparing `tmp/anisha_vehicles-0.2.1.tar.gz` & `tmp/anisha_vehicles-0.2.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "anisha_vehicles-0.2.1.tar", max compression
+gzip compressed data, was "anisha_vehicles-0.2.2.tar", max compression
```

## Comparing `anisha_vehicles-0.2.1.tar` & `anisha_vehicles-0.2.2.tar`

### file list

```diff
@@ -1,5 +1,5 @@
--rw-r--r--   0        0        0       22 2023-05-25 12:07:57.873334 anisha_vehicles-0.2.1/README.md
--rw-r--r--   0        0        0      319 2023-05-25 12:20:18.762293 anisha_vehicles-0.2.1/pyproject.toml
--rw-r--r--   0        0        0       28 2023-05-25 12:20:18.757722 anisha_vehicles-0.2.1/src/anisha_vehicles/__init__.py
--rw-r--r--   0        0        0      471 2023-05-25 12:07:57.880923 anisha_vehicles-0.2.1/src/anisha_vehicles/new_car.py
--rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 anisha_vehicles-0.2.1/PKG-INFO
+-rw-r--r--   0        0        0       22 2023-05-25 12:07:57.873334 anisha_vehicles-0.2.2/README.md
+-rw-r--r--   0        0        0      319 2023-05-28 10:06:36.900433 anisha_vehicles-0.2.2/pyproject.toml
+-rw-r--r--   0        0        0       28 2023-05-25 12:20:18.757722 anisha_vehicles-0.2.2/src/anisha_vehicles/__init__.py
+-rw-r--r--   0        0        0      515 2023-05-25 12:43:57.294272 anisha_vehicles-0.2.2/src/anisha_vehicles/new_car.py
+-rw-r--r--   0        0        0      416 1970-01-01 00:00:00.000000 anisha_vehicles-0.2.2/PKG-INFO
```

