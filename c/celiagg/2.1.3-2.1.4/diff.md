# Comparing `tmp/celiagg-2.1.3.tar.gz` & `tmp/celiagg-2.1.4-cp39-cp39-macosx_10_9_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "celiagg-2.1.3.tar", last modified: Sun Jan 22 14:59:35 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

