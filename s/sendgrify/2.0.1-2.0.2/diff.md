# Comparing `tmp/sendgrify-2.0.1-py3-none-any.whl.zip` & `tmp/sendgrify-2.0.2-py3-none-any.whl.zip`

## zipinfo {}

```diff
@@ -1,9 +1,9 @@
-Zip file size: 3677 bytes, number of entries: 7
+Zip file size: 3675 bytes, number of entries: 7
 -rw-r--r--  2.0 unx       27 b- defN 23-May-27 23:11 sendgrify/__init__.py
 -rw-r--r--  2.0 unx     2795 b- defN 23-May-27 23:11 sendgrify/core.py
--rw-r--r--  2.0 unx     1080 b- defN 23-May-27 23:33 sendgrify-2.0.1.dist-info/LICENSE
--rw-r--r--  2.0 unx     1500 b- defN 23-May-27 23:33 sendgrify-2.0.1.dist-info/METADATA
--rw-r--r--  2.0 unx       92 b- defN 23-May-27 23:33 sendgrify-2.0.1.dist-info/WHEEL
--rw-r--r--  2.0 unx       10 b- defN 23-May-27 23:33 sendgrify-2.0.1.dist-info/top_level.txt
--rw-rw-r--  2.0 unx      546 b- defN 23-May-27 23:33 sendgrify-2.0.1.dist-info/RECORD
-7 files, 6050 bytes uncompressed, 2709 bytes compressed:  55.2%
+-rw-r--r--  2.0 unx     1080 b- defN 23-May-28 12:23 sendgrify-2.0.2.dist-info/LICENSE
+-rw-r--r--  2.0 unx     1490 b- defN 23-May-28 12:23 sendgrify-2.0.2.dist-info/METADATA
+-rw-r--r--  2.0 unx       92 b- defN 23-May-28 12:23 sendgrify-2.0.2.dist-info/WHEEL
+-rw-r--r--  2.0 unx       10 b- defN 23-May-28 12:23 sendgrify-2.0.2.dist-info/top_level.txt
+-rw-rw-r--  2.0 unx      546 b- defN 23-May-28 12:23 sendgrify-2.0.2.dist-info/RECORD
+7 files, 6040 bytes uncompressed, 2707 bytes compressed:  55.2%
```

## zipnote {}

```diff
@@ -1,22 +1,22 @@
 Filename: sendgrify/__init__.py
 Comment: 
 
 Filename: sendgrify/core.py
 Comment: 
 
-Filename: sendgrify-2.0.1.dist-info/LICENSE
+Filename: sendgrify-2.0.2.dist-info/LICENSE
 Comment: 
 
-Filename: sendgrify-2.0.1.dist-info/METADATA
+Filename: sendgrify-2.0.2.dist-info/METADATA
 Comment: 
 
-Filename: sendgrify-2.0.1.dist-info/WHEEL
+Filename: sendgrify-2.0.2.dist-info/WHEEL
 Comment: 
 
-Filename: sendgrify-2.0.1.dist-info/top_level.txt
+Filename: sendgrify-2.0.2.dist-info/top_level.txt
 Comment: 
 
-Filename: sendgrify-2.0.1.dist-info/RECORD
+Filename: sendgrify-2.0.2.dist-info/RECORD
 Comment: 
 
 Zip file comment:
```

## Comparing `sendgrify-2.0.1.dist-info/LICENSE` & `sendgrify-2.0.2.dist-info/LICENSE`

 * *Files identical despite different names*

## Comparing `sendgrify-2.0.1.dist-info/METADATA` & `sendgrify-2.0.2.dist-info/METADATA`

 * *Files 5% similar despite different names*

```diff
@@ -1,19 +1,19 @@
 Metadata-Version: 2.1
 Name: sendgrify
-Version: 2.0.1
+Version: 2.0.2
 Summary: SendGrid for Humans
 Home-page: https://github.com/sdelquin/sendgrify.git
 Author: Sergio Delgado Quintero
 Author-email: sdelquin@gmail.com
 License: MIT
 Description-Content-Type: text/markdown
 License-File: LICENSE
 Requires-Dist: sendgrid (==5.3.0)
-Requires-Dist: markdown (==3.4.3)
+Requires-Dist: markdown
 
 # sendgrify
 
 SendGrid for Humans.
 
 **Sendgrify** is a Python package serving as a wrapper over the email delivery service [SendGrid](https://sendgrid.com/).
```

