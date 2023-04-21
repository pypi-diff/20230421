# Comparing `tmp/cirque_pinnacle-0.0.0.tar.gz` & `tmp/cirque_pinnacle-1.0.0-cp39-cp39-manylinux_2_17_x86_64.manylinux2014_x86_64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cirque_pinnacle-0.0.0.tar", last modified: Fri Apr 21 02:32:28 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=store
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

