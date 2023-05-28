# Comparing `tmp/flixit-0.2.tar.gz` & `tmp/flixit-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "flixit-0.2.tar", last modified: Wed Nov 16 11:51:24 2022, max compression
+gzip compressed data, was "flixit-0.3.tar", last modified: Sun May 28 08:22:52 2023, max compression
```

## Comparing `flixit-0.2.tar` & `flixit-0.3.tar`

### file list

```diff
@@ -1,30 +1,14 @@
-drwxrwxrwx   0        0        0        0 2022-11-16 11:51:24.531680 flixit-0.2/
--rw-rw-rw-   0        0        0      265 2022-11-16 11:51:24.532176 flixit-0.2/PKG-INFO
--rw-rw-rw-   0        0        0       27 2022-11-16 09:47:31.000000 flixit-0.2/README.rst
--rw-rw-rw-   0        0        0      115 2022-11-16 11:51:24.538253 flixit-0.2/setup.cfg
--rw-rw-rw-   0        0        0      393 2022-11-16 11:50:42.000000 flixit-0.2/setup.py
-drwxrwxrwx   0        0        0        0 2022-11-16 11:51:24.455750 flixit-0.2/src/
-drwxrwxrwx   0        0        0        0 2022-11-16 11:51:24.525139 flixit-0.2/src/flixit/
--rw-rw-rw-   0        0        0     1313 2022-11-16 11:17:01.000000 flixit-0.2/src/flixit/BCT1_bank.py
--rw-rw-rw-   0        0        0      628 2022-11-16 11:17:15.000000 flixit-0.2/src/flixit/BCT2_student.py
--rw-rw-rw-   0        0        0      623 2022-11-16 07:03:35.000000 flixit-0.2/src/flixit/Fib_EXP1.py
--rw-rw-rw-   0        0        0      445 2022-11-16 07:03:35.000000 flixit-0.2/src/flixit/Fib_EXP1R.py
--rw-rw-rw-   0        0        0     1742 2022-11-16 07:03:35.000000 flixit-0.2/src/flixit/Huf_EXP2.py
--rw-rw-rw-   0        0        0     1063 2022-11-16 07:03:35.000000 flixit-0.2/src/flixit/Knap01_EXP4.py
--rw-rw-rw-   0        0        0     1669 2022-11-16 07:03:35.000000 flixit-0.2/src/flixit/Knap_EXP3.py
--rw-rw-rw-   0        0        0     6590 2022-11-16 11:09:28.000000 flixit-0.2/src/flixit/ML1_uber.py
--rw-rw-rw-   0        0        0     1852 2022-11-16 11:09:55.000000 flixit-0.2/src/flixit/ML2_emails.py
--rw-rw-rw-   0        0        0     4888 2022-11-16 11:13:17.000000 flixit-0.2/src/flixit/ML3_churn.py
--rw-rw-rw-   0        0        0     3269 2022-11-16 07:03:37.000000 flixit-0.2/src/flixit/ML4.py
--rw-rw-rw-   0        0        0     1999 2022-11-16 11:13:44.000000 flixit-0.2/src/flixit/ML5_diabetes.py
--rw-rw-rw-   0        0        0     4845 2022-11-16 11:14:25.000000 flixit-0.2/src/flixit/ML6_kmeans_sales.py
--rw-rw-rw-   0        0        0     2215 2022-11-16 11:42:04.000000 flixit-0.2/src/flixit/NQueens.py
--rw-rw-rw-   0        0        0     1454 2022-11-16 07:03:35.000000 flixit-0.2/src/flixit/Quic_EXP5.py
--rw-rw-rw-   0        0        0     2298 2022-11-16 07:03:35.000000 flixit-0.2/src/flixit/Quic_EXP5R.py
--rw-rw-rw-   0        0        0        0 2022-11-16 09:50:03.000000 flixit-0.2/src/flixit/__init__.py
--rw-rw-rw-   0        0        0        0 2022-11-16 10:10:02.000000 flixit-0.2/src/flixit/testing.py
-drwxrwxrwx   0        0        0        0 2022-11-16 11:51:24.530341 flixit-0.2/src/flixit.egg-info/
--rw-rw-rw-   0        0        0      265 2022-11-16 11:51:24.000000 flixit-0.2/src/flixit.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      600 2022-11-16 11:51:24.000000 flixit-0.2/src/flixit.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-11-16 11:51:24.000000 flixit-0.2/src/flixit.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        7 2022-11-16 11:51:24.000000 flixit-0.2/src/flixit.egg-info/top_level.txt
+drwxrwxrwx   0        0        0        0 2023-05-28 08:22:52.397107 flixit-0.3/
+-rw-rw-rw-   0        0        0      256 2023-05-28 08:22:52.397107 flixit-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       27 2023-05-28 08:18:42.000000 flixit-0.3/README.rst
+-rw-rw-rw-   0        0        0      115 2023-05-28 08:22:52.399061 flixit-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      393 2023-05-28 08:20:20.000000 flixit-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:22:52.367494 flixit-0.3/src/
+drwxrwxrwx   0        0        0        0 2023-05-28 08:22:52.373362 flixit-0.3/src/flixit/
+-rw-rw-rw-   0        0        0        0 2023-05-28 08:18:42.000000 flixit-0.3/src/flixit/__init__.py
+-rw-rw-rw-   0        0        0        0 2023-05-28 08:18:42.000000 flixit-0.3/src/flixit/testing.py
+drwxrwxrwx   0        0        0        0 2023-05-28 08:22:52.396106 flixit-0.3/src/flixit.egg-info/
+-rw-rw-rw-   0        0        0      256 2023-05-28 08:22:52.000000 flixit-0.3/src/flixit.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      210 2023-05-28 08:22:52.000000 flixit-0.3/src/flixit.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-05-28 08:22:52.000000 flixit-0.3/src/flixit.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        7 2023-05-28 08:22:52.000000 flixit-0.3/src/flixit.egg-info/top_level.txt
```

