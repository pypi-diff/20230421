# Comparing `tmp/django-deno-0.1.2.tar.gz` & `tmp/django_deno-0.1.3-py2.py3-none-any.whl.zip`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "django-deno-0.1.2.tar", last modified: Sat Jun 18 10:33:37 2022, max compression
+Zip archive data, at least v2.0 to extract, compression method=deflate
```

## filetype from diffoscope

```diff
@@ -1 +1 @@
-GzipFile
+ZipFile
```

