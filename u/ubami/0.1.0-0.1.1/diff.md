# Comparing `tmp/ubami-0.1.0.tar.gz` & `tmp/ubami-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ubami-0.1.0.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
+gzip compressed data, was "ubami-0.1.1.tar", last modified: Fri Jan  1 00:00:00 2016, max compression
```

## Comparing `ubami-0.1.0.tar` & `ubami-0.1.1.tar`

### file list

```diff
@@ -1,4 +1,5 @@
--rw-r--r--   0        0        0     1080 2023-05-26 19:47:46.229134 ubami-0.1.0/LICENSE
--rw-r--r--   0        0        0      379 2023-05-27 15:07:05.985383 ubami-0.1.0/pyproject.toml
--rw-r--r--   0        0        0     1963 2023-05-27 15:27:17.140021 ubami-0.1.0/src/ubami.py
--rw-r--r--   0        0        0      262 1970-01-01 00:00:00.000000 ubami-0.1.0/PKG-INFO
+-rw-r--r--   0        0        0     1080 2023-05-26 19:47:46.229134 ubami-0.1.1/LICENSE
+-rw-r--r--   0        0        0      692 2023-05-28 18:58:10.839789 ubami-0.1.1/README.md
+-rw-r--r--   0        0        0      400 2023-05-28 19:02:13.787625 ubami-0.1.1/pyproject.toml
+-rw-r--r--   0        0        0     1978 2023-05-28 19:02:27.577502 ubami-0.1.1/src/ubami.py
+-rw-r--r--   0        0        0     1004 1970-01-01 00:00:00.000000 ubami-0.1.1/PKG-INFO
```

### Comparing `ubami-0.1.0/LICENSE` & `ubami-0.1.1/LICENSE`

 * *Files identical despite different names*

### Comparing `ubami-0.1.0/src/ubami.py` & `ubami-0.1.1/src/ubami.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python3
 
-'''Query the latest Ubuntu AMIs from cloud-images.ubuntu.com.
+'''List and find the latest Ubuntu AMIs from cloud-images.ubuntu.com.
 
-For when you'd rather not hard-code an AMI ID.
+For when you'd rather not hard-code an Ubuntu AMI ID.
 
 # find the latest Jammy Jellyfish AMI for amd64 and hvm:ebs-ssd in London
 ami_id = ubami.find(region='eu-west-2',
                     version='22.04 LTS',
                     arch='amd64',
                     instance_type='hvm:ebs-ssd')[0]['ami_id']
 
 # fetch a list of all the latest official Ubuntu AMIs
 ami_list = ubami.list()
 '''
 
-__version__ = '0.1.0'
+__version__ = '0.1.1'
 
 import json
 import re
 
 import click
 import httpx
```

