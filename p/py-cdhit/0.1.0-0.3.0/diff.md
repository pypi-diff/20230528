# Comparing `tmp/py-cdhit-0.1.0.tar.gz` & `tmp/py_cdhit-0.3.0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "py-cdhit-0.1.0.tar", last modified: Thu May 25 11:42:25 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

