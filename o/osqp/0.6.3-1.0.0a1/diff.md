# Comparing `tmp/osqp-0.6.3.tar.gz` & `tmp/osqp-1.0.0a1-cp39-cp39-manylinux_2_17_aarch64.manylinux2014_aarch64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "osqp-0.6.3.tar", last modified: Fri May 26 00:58:44 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

