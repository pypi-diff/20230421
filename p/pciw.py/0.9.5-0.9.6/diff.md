# Comparing `tmp/pciw.py-0.9.5.tar.gz` & `tmp/pciw.py-0.9.6-py39-none-win_amd64.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pciw.py-0.9.5.tar", last modified: Sun Apr 16 11:10:21 2023, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

