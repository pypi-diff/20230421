# Comparing `tmp/renderlab-0.1.20230421184209.tar.gz` & `tmp/renderlab-0.1.20230421184216-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "renderlab-0.1.20230421184209.tar", last modified: Fri Apr 21 18:42:09 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

