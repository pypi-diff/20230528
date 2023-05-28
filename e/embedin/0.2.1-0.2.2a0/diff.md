# Comparing `tmp/embedin-0.2.1.tar.gz` & `tmp/embedin-0.2.2a0-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "embedin-0.2.1.tar", last modified: Wed May 17 03:02:11 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

