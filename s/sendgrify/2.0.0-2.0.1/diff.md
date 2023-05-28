# Comparing `tmp/sendgrify-2.0.0.macosx-11.6-arm64.tar.gz` & `tmp/sendgrify-2.0.1-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sendgrify-2.0.0.macosx-11.6-arm64.tar", last modified: Sat May 27 23:26:27 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

