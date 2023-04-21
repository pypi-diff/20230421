# Comparing `tmp/mongo_db_operation-1.0.3.tar.gz` & `tmp/mongo_db_operation-1.0.6-py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "mongo_db_operation-1.0.3.tar", last modified: Thu Apr 20 19:47:33 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

