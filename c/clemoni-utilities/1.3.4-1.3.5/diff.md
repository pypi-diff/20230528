# Comparing `tmp/clemoni_utilities-1.3.4.tar.gz` & `tmp/clemoni_utilities-1.3.5-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "clemoni_utilities-1.3.4.tar", last modified: Tue Jan 31 16:40:31 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

