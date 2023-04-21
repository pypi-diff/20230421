# Comparing `tmp/s3pathlib-1.4.1.tar.gz` & `tmp/s3pathlib-2.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "s3pathlib-1.4.1.tar", last modified: Thu Feb 16 16:09:36 2023, max compression
+gzip compressed data, was "s3pathlib-2.0.1.tar", last modified: Fri Apr 21 19:57:18 2023, max compression
```

## Comparing `s3pathlib-1.4.1.tar` & `s3pathlib-2.0.1.tar`

### file list

```diff
@@ -1,66 +1,86 @@
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-16 16:09:36.557965 s3pathlib-1.4.1/
--rw-r--r--   0 sanhehu    (505) staff       (20)      594 2023-02-16 16:05:55.000000 s3pathlib-1.4.1/AUTHORS.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      388 2022-04-26 14:04:57.000000 s3pathlib-1.4.1/CODE_OF_CONDUCT.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     3735 2022-04-26 13:58:02.000000 s3pathlib-1.4.1/CONTRIBUTING.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)    11386 2022-04-26 13:02:50.000000 s3pathlib-1.4.1/LICENSE
--rw-r--r--   0 sanhehu    (505) staff       (20)      306 2022-09-10 16:16:41.000000 s3pathlib-1.4.1/MANIFEST.in
--rw-r--r--   0 sanhehu    (505) staff       (20)       77 2022-04-26 13:02:50.000000 s3pathlib-1.4.1/NOTICE
--rw-r--r--   0 sanhehu    (505) staff       (20)     8371 2023-02-16 16:09:36.557782 s3pathlib-1.4.1/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     7108 2023-02-16 15:08:01.000000 s3pathlib-1.4.1/README.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)     9063 2023-02-16 16:02:27.000000 s3pathlib-1.4.1/release-history.rst
--rw-r--r--   0 sanhehu    (505) staff       (20)      296 2022-11-21 02:30:58.000000 s3pathlib-1.4.1/requirements-dev.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      621 2022-04-26 13:02:50.000000 s3pathlib-1.4.1/requirements-doc.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      193 2022-09-10 16:16:41.000000 s3pathlib-1.4.1/requirements-test.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       92 2023-02-16 14:37:14.000000 s3pathlib-1.4.1/requirements.txt
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-16 16:09:36.543562 s3pathlib-1.4.1/s3pathlib/
--rw-r--r--   0 sanhehu    (505) staff       (20)      641 2022-12-30 16:35:19.000000 s3pathlib-1.4.1/s3pathlib/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-02-16 16:04:29.000000 s3pathlib-1.4.1/s3pathlib/_version.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2177 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/aws.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    11555 2023-02-16 15:14:51.000000 s3pathlib-1.4.1/s3pathlib/client.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1005 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/compat.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-16 16:09:36.554032 s3pathlib-1.4.1/s3pathlib/core/
--rw-r--r--   0 sanhehu    (505) staff       (20)      223 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    10184 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/attribute.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5660 2022-11-21 02:30:58.000000 s3pathlib-1.4.1/s3pathlib/core/base.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      300 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/bucket.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1884 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/comparison.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    20151 2023-02-16 15:17:00.000000 s3pathlib-1.4.1/s3pathlib/core/copy.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2371 2023-02-16 15:06:00.000000 s3pathlib-1.4.1/s3pathlib/core/delete.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2204 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/exists.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5089 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/filterable_property.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3418 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/is_test.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     7449 2022-12-30 16:33:16.000000 s3pathlib-1.4.1/s3pathlib/core/iter_objects.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     4805 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/joinpath.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     6431 2022-11-21 02:30:58.000000 s3pathlib-1.4.1/s3pathlib/core/metadata.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     4090 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/mutate.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     3496 2022-12-30 16:03:51.000000 s3pathlib-1.4.1/s3pathlib/core/opener.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5464 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/relative.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      482 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/resolve_s3_client.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    14703 2023-02-16 15:10:04.000000 s3pathlib-1.4.1/s3pathlib/core/rw.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1361 2023-02-16 15:28:43.000000 s3pathlib-1.4.1/s3pathlib/core/s3path.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      855 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/serde.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     5132 2023-02-16 16:01:48.000000 s3pathlib-1.4.1/s3pathlib/core/sync.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2083 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/tagging.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2997 2023-02-16 15:29:46.000000 s3pathlib-1.4.1/s3pathlib/core/upload.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     6106 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/core/uri.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-16 16:09:36.554243 s3pathlib-1.4.1/s3pathlib/docs/
--rw-r--r--   0 sanhehu    (505) staff       (20)       43 2022-01-17 08:01:19.000000 s3pathlib-1.4.1/s3pathlib/docs/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      933 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/exc.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      748 2022-09-10 16:16:41.000000 s3pathlib-1.4.1/s3pathlib/marker.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      924 2022-11-13 21:00:00.000000 s3pathlib-1.4.1/s3pathlib/tag.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-16 16:09:36.556839 s3pathlib-1.4.1/s3pathlib/tests/
--rw-r--r--   0 sanhehu    (505) staff       (20)      126 2022-11-13 20:36:02.000000 s3pathlib-1.4.1/s3pathlib/tests/__init__.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     1008 2022-11-16 09:14:57.000000 s3pathlib-1.4.1/s3pathlib/tests/aws.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     2041 2022-11-13 20:34:30.000000 s3pathlib-1.4.1/s3pathlib/tests/helpers.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      345 2022-11-13 20:27:49.000000 s3pathlib-1.4.1/s3pathlib/tests/paths.py
--rw-r--r--   0 sanhehu    (505) staff       (20)      329 2023-02-16 15:27:59.000000 s3pathlib-1.4.1/s3pathlib/type.py
--rw-r--r--   0 sanhehu    (505) staff       (20)    21958 2023-02-16 15:34:16.000000 s3pathlib-1.4.1/s3pathlib/utils.py
--rw-r--r--   0 sanhehu    (505) staff       (20)     4118 2022-02-06 15:53:43.000000 s3pathlib-1.4.1/s3pathlib/validate.py
-drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-02-16 16:09:36.544389 s3pathlib-1.4.1/s3pathlib.egg-info/
--rw-r--r--   0 sanhehu    (505) staff       (20)     8371 2023-02-16 16:09:36.000000 s3pathlib-1.4.1/s3pathlib.egg-info/PKG-INFO
--rw-r--r--   0 sanhehu    (505) staff       (20)     1337 2023-02-16 16:09:36.000000 s3pathlib-1.4.1/s3pathlib.egg-info/SOURCES.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-02-16 16:09:36.000000 s3pathlib-1.4.1/s3pathlib.egg-info/dependency_links.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)      273 2023-02-16 16:09:36.000000 s3pathlib-1.4.1/s3pathlib.egg-info/requires.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       10 2023-02-16 16:09:36.000000 s3pathlib-1.4.1/s3pathlib.egg-info/top_level.txt
--rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-02-16 16:09:36.558655 s3pathlib-1.4.1/setup.cfg
--rw-r--r--   0 sanhehu    (505) staff       (20)     8395 2022-09-10 16:16:41.000000 s3pathlib-1.4.1/setup.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-21 19:57:18.306587 s3pathlib-2.0.1/
+-rw-r--r--   0 sanhehu    (505) staff       (20)      594 2023-04-15 15:30:55.000000 s3pathlib-2.0.1/AUTHORS.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)      388 2022-04-26 14:04:57.000000 s3pathlib-2.0.1/CODE_OF_CONDUCT.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)     3735 2022-04-26 13:58:02.000000 s3pathlib-2.0.1/CONTRIBUTING.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)    11386 2022-04-26 13:02:50.000000 s3pathlib-2.0.1/LICENSE
+-rw-r--r--   0 sanhehu    (505) staff       (20)      306 2022-09-10 16:16:41.000000 s3pathlib-2.0.1/MANIFEST.in
+-rw-r--r--   0 sanhehu    (505) staff       (20)       77 2022-04-26 13:02:50.000000 s3pathlib-2.0.1/NOTICE
+-rw-r--r--   0 sanhehu    (505) staff       (20)     9193 2023-04-21 19:57:18.306308 s3pathlib-2.0.1/PKG-INFO
+-rw-r--r--   0 sanhehu    (505) staff       (20)     7982 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/README.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)       32 2023-04-21 19:49:06.000000 s3pathlib-2.0.1/chore.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)    10915 2023-04-21 19:50:57.000000 s3pathlib-2.0.1/release-history.rst
+-rw-r--r--   0 sanhehu    (505) staff       (20)      316 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/requirements-dev.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      824 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/requirements-doc.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      203 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/requirements-test.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      160 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/requirements.txt
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-21 19:57:18.281034 s3pathlib-2.0.1/s3pathlib/
+-rw-r--r--   0 sanhehu    (505) staff       (20)      676 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/__init__.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)       93 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/_version.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     2519 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/aws.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-21 19:57:18.285900 s3pathlib-2.0.1/s3pathlib/better_client/
+-rw-r--r--   0 sanhehu    (505) staff       (20)       66 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/better_client/__init__.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      775 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/better_client/api.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     7809 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/better_client/delete_object.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      902 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/better_client/head_bucket.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     4010 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/better_client/head_object.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     6882 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/better_client/list_object_versions.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     8178 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/better_client/list_objects.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     3448 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/better_client/tagging.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     2509 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/better_client/upload.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     1231 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/compat.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)       61 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/constants.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-21 19:57:18.299120 s3pathlib-2.0.1/s3pathlib/core/
+-rw-r--r--   0 sanhehu    (505) staff       (20)      223 2022-11-16 09:14:57.000000 s3pathlib-2.0.1/s3pathlib/core/__init__.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)    10343 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/attribute.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     6478 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/base.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      300 2022-11-16 09:14:57.000000 s3pathlib-2.0.1/s3pathlib/core/bucket.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     1884 2022-11-16 09:14:57.000000 s3pathlib-2.0.1/s3pathlib/core/comparison.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)    22226 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/core/copy.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     9025 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/core/delete.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     3271 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/core/exists.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     5241 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/filterable_property.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     3948 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/is_test.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     2997 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/iter_object_versions.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)    11570 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/iter_objects.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     3227 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/core/joinpath.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     7663 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/core/metadata.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     5230 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/mutate.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     5007 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/core/opener.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     5609 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/core/relative.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      598 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/core/resolve_s3_client.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)    27959 2023-04-21 19:46:28.000000 s3pathlib-2.0.1/s3pathlib/core/rw.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     1454 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/s3path.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      855 2022-11-16 09:14:57.000000 s3pathlib-2.0.1/s3pathlib/core/serde.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     5556 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/sync.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     4431 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/tagging.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     3068 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/upload.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     6695 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/core/uri.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-21 19:57:18.299346 s3pathlib-2.0.1/s3pathlib/docs/
+-rw-r--r--   0 sanhehu    (505) staff       (20)       43 2022-01-17 08:01:19.000000 s3pathlib-2.0.1/s3pathlib/docs/__init__.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     2529 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/exc.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      748 2022-09-10 16:16:41.000000 s3pathlib-2.0.1/s3pathlib/marker.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      877 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/metadata.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     2359 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/tag.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-21 19:57:18.300985 s3pathlib-2.0.1/s3pathlib/tests/
+-rw-r--r--   0 sanhehu    (505) staff       (20)       59 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/tests/__init__.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     1502 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/tests/helpers.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     6767 2023-04-21 19:40:24.000000 s3pathlib-2.0.1/s3pathlib/tests/mock.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      594 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/tests/paths.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      392 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/type.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)    10351 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/s3pathlib/utils.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     4118 2022-02-06 15:53:43.000000 s3pathlib-2.0.1/s3pathlib/validate.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-21 19:57:18.283236 s3pathlib-2.0.1/s3pathlib.egg-info/
+-rw-r--r--   0 sanhehu    (505) staff       (20)     9193 2023-04-21 19:57:18.000000 s3pathlib-2.0.1/s3pathlib.egg-info/PKG-INFO
+-rw-r--r--   0 sanhehu    (505) staff       (20)     1878 2023-04-21 19:57:18.000000 s3pathlib-2.0.1/s3pathlib.egg-info/SOURCES.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)        1 2023-04-21 19:57:18.000000 s3pathlib-2.0.1/s3pathlib.egg-info/dependency_links.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)      365 2023-04-21 19:57:18.000000 s3pathlib-2.0.1/s3pathlib.egg-info/requires.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)       10 2023-04-21 19:57:18.000000 s3pathlib-2.0.1/s3pathlib.egg-info/top_level.txt
+-rw-r--r--   0 sanhehu    (505) staff       (20)       38 2023-04-21 19:57:18.306643 s3pathlib-2.0.1/setup.cfg
+-rw-r--r--   0 sanhehu    (505) staff       (20)     8346 2023-04-21 19:48:35.000000 s3pathlib-2.0.1/setup.py
+drwxr-xr-x   0 sanhehu    (505) staff       (20)        0 2023-04-21 19:57:18.305808 s3pathlib-2.0.1/tests/
+-rw-r--r--   0 sanhehu    (505) staff       (20)     1104 2022-01-21 00:32:37.000000 s3pathlib-2.0.1/tests/test_exc.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     1349 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/tests/test_marker.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      399 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/tests/test_metadata.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)      989 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/tests/test_tag.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     3233 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/tests/test_utils.py
+-rw-r--r--   0 sanhehu    (505) staff       (20)     2563 2023-04-21 16:54:44.000000 s3pathlib-2.0.1/tests/test_validate.py
```

### Comparing `s3pathlib-1.4.1/AUTHORS.rst` & `s3pathlib-2.0.1/AUTHORS.rst`

 * *Files identical despite different names*

### Comparing `s3pathlib-1.4.1/CONTRIBUTING.rst` & `s3pathlib-2.0.1/CONTRIBUTING.rst`

 * *Files identical despite different names*

### Comparing `s3pathlib-1.4.1/LICENSE` & `s3pathlib-2.0.1/LICENSE`

 * *Files identical despite different names*

### Comparing `s3pathlib-1.4.1/PKG-INFO` & `s3pathlib-2.0.1/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: s3pathlib
-Version: 1.4.1
+Version: 2.0.1
 Summary: Objective Oriented Interface for AWS S3, similar to pathlib.
 Home-page: https://github.com/aws-samples/s3pathlib-project
-Download-URL: https://pypi.python.org/pypi/s3pathlib/1.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/s3pathlib/2.0.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: sanhehu@amazon.com
 License: Apache License 2.0
 Platform: Windows
 Platform: MacOS
@@ -18,15 +18,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
@@ -36,26 +35,32 @@
 .. image:: https://readthedocs.org/projects/s3pathlib/badge/?version=latest
     :target: https://s3pathlib.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 .. image:: https://github.com/aws-samples/s3pathlib-project/workflows/CI/badge.svg
     :target: https://github.com/aws-samples/s3pathlib-project/actions?query=workflow:CI
 
+.. image:: https://img.shields.io/badge/codecov-100%25-brightgreen
+    :target: https://github.com/aws-samples/s3pathlib-project/actions?query=workflow:CI
+
 .. image:: https://img.shields.io/pypi/v/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
 
 .. image:: https://img.shields.io/pypi/l/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
 
 .. image:: https://img.shields.io/pypi/pyversions/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
     
 .. image:: https://img.shields.io/pypi/dm/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
 
+.. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
+    :target: https://github.com/aws-samples/s3pathlib-project
+
 ------
 
 .. image:: https://img.shields.io/badge/Link-Document-orange.svg
     :target: https://s3pathlib.readthedocs.io/en/latest/
 
 .. image:: https://img.shields.io/badge/Link-API-blue.svg
     :target: https://s3pathlib.readthedocs.io/en/latest/py-modindex.html
@@ -71,38 +76,40 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/s3pathlib#files
 
 
 Welcome to ``s3pathlib`` Documentation
 ==============================================================================
-
-``s3pathlib`` is the python package provides the Pythonic objective oriented programming (OOP) interface to manipulate AWS S3 object / directory. The api is similar to the ``pathlib`` `standard library <https://docs.python.org/3/library/pathlib.html>`_ and very intuitive for human.
+`s3pathlib <https://s3pathlib.readthedocs.io/en/latest/>`_ is a Python package that offers an object-oriented programming (OOP) interface to work with AWS S3 objects and directories. Its API is designed to be similar to the standard library `pathlib <https://docs.python.org/3/library/pathlib.html>`_ and is user-friendly. The package also `supports versioning <https://docs.aws.amazon.com/AmazonS3/latest/userguide/Versioning.html>`_ in AWS S3.
 
 .. note::
 
-    You may not viewing the full document, `FULL DOCUMENT IS HERE <https://s3pathlib.readthedocs.io/en/latest/>`_
+    You may not be viewing the full document, `FULL DOCUMENT IS HERE <https://s3pathlib.readthedocs.io/en/latest/>`_
 
 
 Quick Start
 ------------------------------------------------------------------------------
 .. note::
 
-    `COMPREHENSIVE DOCUMENT guide / features / best practice can be found at HERE <https://s3pathlib.readthedocs.io/en/latest/#full-table-of-content>`_
-
+    `COMPREHENSIVE DOCUMENT guide / features / best practice can be found at HERE <https://s3pathlib.readthedocs.io/en/latest/#comprehensive-guide>`_
 
-**Import the library, declare a S3 object**
+**Import the library, declare an S3Path object**
 
 .. code-block:: python
 
     # import
     >>> from s3pathlib import S3Path
 
     # construct from string, auto join parts
     >>> p = S3Path("bucket", "folder", "file.txt")
+    # construct from S3 URI works too
+    >>> p = S3Path("s3://bucket/folder/file.txt")
+    # construct from S3 ARN works too
+    >>> p = S3Path("arn:aws:s3:::bucket/folder/file.txt")
     >>> p.bucket
     'bucket'
     >>> p.key
     'folder/file.txt'
     >>> p.uri
     's3://bucket/folder/file.txt'
     >>> p.console_url # click to preview it in AWS console
@@ -122,14 +129,15 @@
     ...     boto3.session.Session(
     ...         region_name="us-east-1",
     ...         profile_name="my_aws_profile",
     ...     )
     ... )
 
     >>> p = S3Path("bucket", "folder", "file.txt")
+    >>> p.write_text("a lot of data ...")
     >>> p.etag
     '3e20b77868d1a39a587e280b99cec4a8'
     >>> p.size
     56789000
     >>> p.size_for_human
     '51.16 MB'
 
@@ -155,25 +163,25 @@
     >>> p.upload_dir("/my-repo", pattern="**/*.py", overwrite=False)
 
     # copy entire s3 folder to another s3 folder
     >>> p2 = S3Path("bucket", "github", "repos", "another-repo/")
     >>> p1.copy_to(p2, overwrite=True)
 
     # delete all objects in the folder, recursively, to clean up your test bucket
-    >>> p.delete_if_exists()
-    >>> p2.delete_if_exists()
+    >>> p.delete()
+    >>> p2.delete()
 
 **S3 Path Filter**
 
 Ever think of filter S3 object by it's attributes like: dirname, basename, file extension, etag, size, modified time? It is supposed to be simple in Python:
 
 .. code-block:: python
 
-    >>> root = S3Path("bucket") # assume you have a lots of files in this bucket
-    >>> iterproxy = root.iter_objects().filter(
+    >>> s3bkt = S3Path("bucket") # assume you have a lots of files in this bucket
+    >>> iterproxy = s3bkt.iter_objects().filter(
     ...     S3Path.size >= 10_000_000, S3Path.ext == ".csv" # add filter
     ... )
 
     >>> iterproxy.one() # fetch one
     S3Path('s3://bucket/larger-than-10MB-1.csv')
 
     >>> iterproxy.many(3) # fetch three
@@ -208,26 +216,25 @@
     # pandas IO
     >>> import pandas as pd
     >>> p = S3Path("bucket", "dataset.csv")
     >>> df = pd.DataFrame(...)
     >>> with p.open("w") as f:
     ...     df.to_csv(f)
 
+Now that you have a basic understanding of s3pathlib, let's read the `full document <https://s3pathlib.readthedocs.io/en/latest/#comprehensive-guide>`_ to explore its capabilities in greater depth.
+
 
 Getting Help
 ------------------------------------------------------------------------------
 Please use the ``python-s3pathlib`` tag on Stack Overflow to get help.
 
 Submit a ``I want help`` issue tickets on `GitHub Issues <https://github.com/aws-samples/s3pathlib-project/issues/new/choose>`_
 
 
-
 Contributing
 ------------------------------------------------------------------------------
 Please see the `Contribution Guidelines <https://github.com/aws-samples/s3pathlib-project/blob/main/CONTRIBUTING.rst>`_.
 
 
 Copyright
 ------------------------------------------------------------------------------
 s3pathlib is an open source project. See the `LICENSE <https://github.com/aws-samples/s3pathlib-project/blob/main/LICENSE>`_ file for more information.
-
-
```

### Comparing `s3pathlib-1.4.1/README.rst` & `s3pathlib-2.0.1/README.rst`

 * *Files 8% similar despite different names*

```diff
@@ -1,26 +1,32 @@
 .. image:: https://readthedocs.org/projects/s3pathlib/badge/?version=latest
     :target: https://s3pathlib.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 .. image:: https://github.com/aws-samples/s3pathlib-project/workflows/CI/badge.svg
     :target: https://github.com/aws-samples/s3pathlib-project/actions?query=workflow:CI
 
+.. image:: https://img.shields.io/badge/codecov-100%25-brightgreen
+    :target: https://github.com/aws-samples/s3pathlib-project/actions?query=workflow:CI
+
 .. image:: https://img.shields.io/pypi/v/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
 
 .. image:: https://img.shields.io/pypi/l/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
 
 .. image:: https://img.shields.io/pypi/pyversions/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
     
 .. image:: https://img.shields.io/pypi/dm/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
 
+.. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
+    :target: https://github.com/aws-samples/s3pathlib-project
+
 ------
 
 .. image:: https://img.shields.io/badge/Link-Document-orange.svg
     :target: https://s3pathlib.readthedocs.io/en/latest/
 
 .. image:: https://img.shields.io/badge/Link-API-blue.svg
     :target: https://s3pathlib.readthedocs.io/en/latest/py-modindex.html
@@ -36,38 +42,40 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/s3pathlib#files
 
 
 Welcome to ``s3pathlib`` Documentation
 ==============================================================================
-
-``s3pathlib`` is the python package provides the Pythonic objective oriented programming (OOP) interface to manipulate AWS S3 object / directory. The api is similar to the ``pathlib`` `standard library <https://docs.python.org/3/library/pathlib.html>`_ and very intuitive for human.
+`s3pathlib <https://s3pathlib.readthedocs.io/en/latest/>`_ is a Python package that offers an object-oriented programming (OOP) interface to work with AWS S3 objects and directories. Its API is designed to be similar to the standard library `pathlib <https://docs.python.org/3/library/pathlib.html>`_ and is user-friendly. The package also `supports versioning <https://docs.aws.amazon.com/AmazonS3/latest/userguide/Versioning.html>`_ in AWS S3.
 
 .. note::
 
-    You may not viewing the full document, `FULL DOCUMENT IS HERE <https://s3pathlib.readthedocs.io/en/latest/>`_
+    You may not be viewing the full document, `FULL DOCUMENT IS HERE <https://s3pathlib.readthedocs.io/en/latest/>`_
 
 
 Quick Start
 ------------------------------------------------------------------------------
 .. note::
 
-    `COMPREHENSIVE DOCUMENT guide / features / best practice can be found at HERE <https://s3pathlib.readthedocs.io/en/latest/#full-table-of-content>`_
+    `COMPREHENSIVE DOCUMENT guide / features / best practice can be found at HERE <https://s3pathlib.readthedocs.io/en/latest/#comprehensive-guide>`_
 
-
-**Import the library, declare a S3 object**
+**Import the library, declare an S3Path object**
 
 .. code-block:: python
 
     # import
     >>> from s3pathlib import S3Path
 
     # construct from string, auto join parts
     >>> p = S3Path("bucket", "folder", "file.txt")
+    # construct from S3 URI works too
+    >>> p = S3Path("s3://bucket/folder/file.txt")
+    # construct from S3 ARN works too
+    >>> p = S3Path("arn:aws:s3:::bucket/folder/file.txt")
     >>> p.bucket
     'bucket'
     >>> p.key
     'folder/file.txt'
     >>> p.uri
     's3://bucket/folder/file.txt'
     >>> p.console_url # click to preview it in AWS console
@@ -87,14 +95,15 @@
     ...     boto3.session.Session(
     ...         region_name="us-east-1",
     ...         profile_name="my_aws_profile",
     ...     )
     ... )
 
     >>> p = S3Path("bucket", "folder", "file.txt")
+    >>> p.write_text("a lot of data ...")
     >>> p.etag
     '3e20b77868d1a39a587e280b99cec4a8'
     >>> p.size
     56789000
     >>> p.size_for_human
     '51.16 MB'
 
@@ -120,25 +129,25 @@
     >>> p.upload_dir("/my-repo", pattern="**/*.py", overwrite=False)
 
     # copy entire s3 folder to another s3 folder
     >>> p2 = S3Path("bucket", "github", "repos", "another-repo/")
     >>> p1.copy_to(p2, overwrite=True)
 
     # delete all objects in the folder, recursively, to clean up your test bucket
-    >>> p.delete_if_exists()
-    >>> p2.delete_if_exists()
+    >>> p.delete()
+    >>> p2.delete()
 
 **S3 Path Filter**
 
 Ever think of filter S3 object by it's attributes like: dirname, basename, file extension, etag, size, modified time? It is supposed to be simple in Python:
 
 .. code-block:: python
 
-    >>> root = S3Path("bucket") # assume you have a lots of files in this bucket
-    >>> iterproxy = root.iter_objects().filter(
+    >>> s3bkt = S3Path("bucket") # assume you have a lots of files in this bucket
+    >>> iterproxy = s3bkt.iter_objects().filter(
     ...     S3Path.size >= 10_000_000, S3Path.ext == ".csv" # add filter
     ... )
 
     >>> iterproxy.one() # fetch one
     S3Path('s3://bucket/larger-than-10MB-1.csv')
 
     >>> iterproxy.many(3) # fetch three
@@ -173,23 +182,24 @@
     # pandas IO
     >>> import pandas as pd
     >>> p = S3Path("bucket", "dataset.csv")
     >>> df = pd.DataFrame(...)
     >>> with p.open("w") as f:
     ...     df.to_csv(f)
 
+Now that you have a basic understanding of s3pathlib, let's read the `full document <https://s3pathlib.readthedocs.io/en/latest/#comprehensive-guide>`_ to explore its capabilities in greater depth.
+
 
 Getting Help
 ------------------------------------------------------------------------------
 Please use the ``python-s3pathlib`` tag on Stack Overflow to get help.
 
 Submit a ``I want help`` issue tickets on `GitHub Issues <https://github.com/aws-samples/s3pathlib-project/issues/new/choose>`_
 
 
-
 Contributing
 ------------------------------------------------------------------------------
 Please see the `Contribution Guidelines <https://github.com/aws-samples/s3pathlib-project/blob/main/CONTRIBUTING.rst>`_.
 
 
 Copyright
 ------------------------------------------------------------------------------
```

### Comparing `s3pathlib-1.4.1/release-history.rst` & `s3pathlib-2.0.1/release-history.rst`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,58 @@
 .. _release_history:
 
 Release and Version History
 ==============================================================================
 
+:orphan:
+
 
 Backlog (TODO)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - make :class:`s3pathlib.aws.Context` multi-thread safe.
-- add ``acl`` management feature
-- add ``legal_hold`` management feature
+
+
+2.0.1 (TODO)
+~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
+**Features and Improvements**
+
+Changes:
+
+- most of methods now supports ``version_id`` argument for S3 versioning enabled bucket.
+- :meth:`s3pathlib.core.rw.ReadAndWriteAPIMixin.read_bytes` and :meth:`s3pathlib.core.rw.ReadAndWriteAPIMixin.read_text` now support ``version_id`` and full list of ``get_object`` boto3 arguments.
+- :meth:`s3pathlib.core.uri.UriAPIMixin.console_url` now take the version id into consideration.
+- add :meth:`s3pathlib.core.is_test.IsTestAPIMixin.is_delete_marker` method.
+- :meth:`s3pathlib.core.base.BaseS3Path.__new__` now can take S3 URI and ARN directly without using the ``from_s3_uri`` and ``from_s3_arn`` method.
+
+New APIs:
+
+- add ``s3pathlib.better_client`` to the public API, it is a collection of more user friendly boto3 API, with type hint.
+- add :meth:`~s3pathlib.core.iter_object_versions.IterObjectVersionsAPIMixin.list_object_versions` method. It will return all objects, all versions, all delete markers in reverse chronological order.
+- The :meth:`~s3pathlib.core.is_test.IsTestAPIMixin.is_delete_marker` method can be used to check if the version is a delete marker.
+- :meth:`~s3pathlib.core.delete.DeleteAPIMixin.delete`: delete object, directory (recursively), specific object version, object versions, all objects all versions in directory. This API will replace the old :meth:`~s3pathlib.core.delete.DeleteAPIMixin.delete_if_exists` API in 3.X.Y.
 
 **Minor Improvements**
 
-- add JupyterNotebook document
+- use moto for unit test.
+- add tons of more unit test for edge cases.
+- prompt to confirm when delete everything in a bucket.
+
+**Bugfixes**
+
+- fix a bug that should not allow user to set value to attributes like ``bucket``, ``key``.
+
+**Miscellaneous**
+
+- completely rewrite the documentation in Jupyter notebook to provide interactive reading experience.
+
+**Imcompatible Change**
+
+- removed :meth:`~s3pathlib.core.joinpath.JoinPathAPIMixin.join_path`.
 
 
 1.4.1 (2023-02-16)
 ~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
 **Features and Improvements**
 
 - now the following API supports full list of native boto3 argument:
```

### Comparing `s3pathlib-1.4.1/s3pathlib/__init__.py` & `s3pathlib-2.0.1/s3pathlib/__init__.py`

 * *Files 20% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 __author_email__ = "husanhe@gmail.com"
 __maintainer__ = "Sanhe Hu"
 __maintainer_email__ = "sanhehu@amazon.com"
 __github_username__ = "aws-samples"
 
 try:
     from . import utils
+    from .better_client import api
     from .aws import context
     from .core import S3Path
 
     from iterproxy import and_, or_, not_
 except ImportError:  # pragma: no cover
     pass
 except:  # pragma: no cover
```

### Comparing `s3pathlib-1.4.1/s3pathlib/aws.py` & `s3pathlib-2.0.1/s3pathlib/aws.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,85 +1,92 @@
 # -*- coding: utf-8 -*-
 
 """
-Manage the AWS environment that s3pathlib dealing with.
+Manage the AWS environment that ``s3pathlib`` dealing with.
 """
 
-from typing import Optional
+import typing as T
 
 try:
     import boto3
 except ImportError:  # pragma: no cover
     pass
 except:  # pragma: no cover
     raise
 
+if T.TYPE_CHECKING:  # pragma: no cover
+    from mypy_boto3_s3 import S3Client
+    from mypy_boto3_sts import STSClient
+
 
 class Context:
     """
     A globally available context object managing AWS SDK credentials.
 
     TODO: use singleton pattern to create context object
     """
 
     def __init__(self):
-        self.boto_ses: Optional['boto3.session.Session'] = None
-        self._aws_region: Optional[str] = None
-        self._aws_account_id: Optional[str] = None
-        self._s3_client = None
-        self._sts_client = None
+        self.boto_ses: T.Optional["boto3.session.Session"] = None
+        self._aws_region: T.Optional[str] = None
+        self._aws_account_id: T.Optional[str] = None
+        self._s3_client: T.Optional["S3Client"] = None
+        self._sts_client: T.Optional["STSClient"] = None
 
         # try to create default session
         try:
             self.boto_ses = boto3.session.Session()
         except:  # pragma: no cover
             pass
 
-    def attach_boto_session(self, boto_ses):
+    def attach_boto_session(self, boto_ses: "boto3.session.Session"):
         """
-        Attach a custom boto session.
-
-        :type boto_ses: boto3.session.Session
+        Attach a custom boto session, also remove caches.
         """
         self.boto_ses = boto_ses
         self._s3_client = None
         self._sts_client = None
+        self._aws_account_id = None
+        self._aws_region = None
 
     @property
-    def s3_client(self):
+    def s3_client(self) -> "S3Client":
         """
         Access the s3 client.
 
         https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#client
         """
         if self._s3_client is None:
             self._s3_client = self.boto_ses.client("s3")
         return self._s3_client
 
     @property
-    def sts_client(self):
+    def sts_client(self) -> "STSClient":
         """
         Access the s3 client.
 
         https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#client
         """
         if self._sts_client is None:
             self._sts_client = self.boto_ses.client("sts")
         return self._sts_client
 
     @property
     def aws_account_id(self) -> str:
         """
-        The AWS Account ID of the current boto session/
+        The AWS Account ID of the current boto session.
         """
         if self._aws_account_id is None:
             self._aws_account_id = self.sts_client.get_caller_identity()["Account"]
         return self._aws_account_id
 
     @property
     def aws_region(self) -> str:
+        """
+        The AWS Region of the current boto session.
+        """
         if self._aws_region is None:
             self._aws_region = self.boto_ses.region_name
         return self._aws_region
 
 
 context = Context()
```

### Comparing `s3pathlib-1.4.1/s3pathlib/compat.py` & `s3pathlib-2.0.1/s3pathlib/compat.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,9 +1,15 @@
 # -*- coding: utf-8 -*-
 
+"""
+Provide compatibility with older versions of Python and dependent libraries.
+"""
+
+import sys
+
 try:
     import smart_open
 
     smart_open_version = smart_open.__version__
     (
         smart_open_version_major,
         smart_open_version_minor,
@@ -14,14 +20,19 @@
 except ImportError:  # pragma: no cover
     smart_open = None
     smart_open_version_major = None
     smart_open_version_minor = None
 except:  # pragma: no cover
     raise
 
+if sys.version_info.minor < 8:
+    from cached_property import cached_property
+else:
+    from functools import cached_property
+
 
 class Compat:  # pragma: no cover
     @property
     def smart_open_version_major(self) -> int:
         if smart_open_version_major is None:
             raise ImportError("You don't have smart_open installed")
         return smart_open_version_major
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/attribute.py` & `s3pathlib-2.0.1/s3pathlib/core/attribute.py`

 * *Files 2% similar despite different names*

```diff
@@ -54,14 +54,19 @@
 
     @property
     def parents(self: "S3Path") -> T.List["S3Path"]:
         """
         An immutable sequence providing access to the logical ancestors of
         the path.
 
+        Examples::
+
+            >>> S3Path("my-bucket", "my-folder", "my-file.json").parents
+            s3://my-bucket/my-folder/
+
         .. versionadded:: 1.0.6
         """
         if self.is_void():
             raise ValueError(f"void S3path doesn't support .parents method!")
         if self.is_relpath():
             raise ValueError(f"relative S3path doesn't support .parents method!")
         l = list()
@@ -347,13 +352,13 @@
 
         elif self.is_relpath():
             key = self.key
             if len(key):
                 return f"S3RelPath({key!r})"
             else:  # pragma: no cover
                 return "S3RelPath()"
-        else:
+        else: # bucket, folder or object
             uri = self.uri
             return "{}('{}')".format(classname, uri)
 
     def __str__(self: "S3Path"):
         return self.__repr__()
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/base.py` & `s3pathlib-2.0.1/s3pathlib/core/base.py`

 * *Files 9% similar despite different names*

```diff
@@ -52,19 +52,20 @@
 
         # first argument becomes the bucket
         >>> s3path = S3Path("bucket", "folder", "file.txt")
         # print S3Path object gives you info in S3 URI format
         >>> s3path
         S3Path('s3://bucket/folder/file.txt')
 
-        # last argument defines that it is a file
+        # If the last argument has a trailing slash ("/"), it indicates that
+        # it refers to a directory. Otherwise, it is assumed to be a file.
         >>> s3path.is_file()
         True
         >>> s3path.is_dir()
-        True
+        False
 
         # "/" separator will be automatically handled
         >>> S3Path("bucket", "folder/file.txt")
         S3Path('s3://bucket/folder/file.txt')
 
         >>> S3Path("bucket/folder/file.txt")
         S3Path('s3://bucket/folder/file.txt')
@@ -77,15 +78,26 @@
 
         # last argument defines that it is a directory
         >>> s3path.is_dir()
         True
         >>> s3path.is_file()
         False
 
+    You can also create it from S3 URI or ARN::
+
+        >>> S3Path("s3://bucket/folder/file.txt")
+        S3Path('s3://bucket/folder/file.txt')
+        >>> S3Path("arn:aws:s3:::bucket/folder/file.txt"),
+        S3Path('s3://bucket/folder/file.txt')
+
     .. versionadded:: 1.0.1
+
+    .. versionchanged:: 2.0.1
+
+        You can create S3Path from s3 uri or arn directly.
     """
 
     __slots__ = (
         "_bucket",
         "_parts",
         "_is_dir",
         "_cached_cparts",  # cached comparison parts
@@ -93,36 +105,51 @@
         "_meta",  # s3 object metadata cache object
     )
 
     def __new__(
         cls: T.Type["S3Path"],
         *args: T.Union[str, "S3Path"],
     ) -> "S3Path":
+        """
+        The constructor of :class:`S3Path`.
+        """
         return cls._from_parts(args)
 
     @classmethod
     def _from_parts(
         cls: T.Type["S3Path"],
         args: T.List[T.Union[str, "S3Path"]],
         init: bool = True,
     ) -> "S3Path":
+        """
+        Low level implementation of the constructor.
+        """
         _bucket = None
         _parts = list()
         _is_dir = None
 
         if len(args) == 0:
             return cls._from_parsed_parts(
                 bucket=_bucket,
                 parts=_parts,
                 is_dir=_is_dir,
             )
 
         # resolve self._bucket
         arg = args[0]
+
         if isinstance(arg, str):
+            # handle S3 URI and ARN
+            if arg.startswith("s3://"):
+                arg = arg[5:]
+            elif arg.startswith("arn:aws:s3:::"):
+                arg = arg[13:]
+            else:
+                pass
+
             utils.validate_s3_bucket(arg)
             parts = utils.split_parts(arg)
             _bucket = parts[0]
             _parts.extend(parts[1:])
         elif isinstance(arg, BaseS3Path):
             _bucket = arg._bucket
             _parts.extend(arg._parts)
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/comparison.py` & `s3pathlib-2.0.1/s3pathlib/core/comparison.py`

 * *Files identical despite different names*

### Comparing `s3pathlib-1.4.1/s3pathlib/core/copy.py` & `s3pathlib-2.0.1/s3pathlib/core/copy.py`

 * *Files 17% similar despite different names*

```diff
@@ -1,37 +1,40 @@
 # -*- coding: utf-8 -*-
 
 """
 Copy file from s3 to s3.
+
+.. _copy_file: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/client/copy_object.html
 """
 
 import typing as T
 from datetime import datetime
 
-from func_args import NOTHING
+from func_args import NOTHING, resolve_kwargs
 
-from .. import client as better_client
 from ..type import TagType, MetadataType
+from ..tag import encode_url_query
 
 from .resolve_s3_client import resolve_s3_client
 from ..aws import context
 
 if T.TYPE_CHECKING:  # pragma: no cover
     from .s3path import S3Path
     from boto_session_manager import BotoSesManager
 
 
 class CopyAPIMixin:
     """
-    A mixin class that implements copy method.
+    A mixin class that implements copy related methods.
     """
 
     def copy_file(
         self: "S3Path",
         dst: "S3Path",
+        version_id: str = NOTHING,
         metadata: T.Optional[MetadataType] = NOTHING,
         tags: T.Optional[TagType] = NOTHING,
         overwrite: bool = False,
         bsm: T.Optional["BotoSesManager"] = None,
         acl: str = NOTHING,
         cache_control: str = NOTHING,
         content_disposition: str = NOTHING,
@@ -62,77 +65,96 @@
         object_lock_mode: str = NOTHING,
         object_lock_retain_until_datetime: datetime = NOTHING,
         object_lock_legal_hold_status: str = NOTHING,
         expected_bucket_owner: str = NOTHING,
         expected_source_bucket_owner: str = NOTHING,
     ) -> dict:
         """
-        Copy an S3 directory to a different S3 directory, including all
-        sub-directory and files.
+        Copy an S3 file to a different S3 location.
 
         :param dst: copy to s3 object, it has to be an object
         :param overwrite: if False, none of the file will be uploaded / overwritten
-            if any of target s3 location already taken.
+            if any of target s3 location already taken. Note that if the target
+            S3 location is a versioning enabled bucket, logically you should be
+            able to put a new version to an existing file, but this if
+            ``overwrite`` is True, then it won't allow you to do that. You should
+            set ``overwrite`` to False if you want to put a new version.
 
         :return: number of object are copied, 0 or 1.
 
         .. versionadded:: 1.0.1
 
         .. versionchanged:: 1.3.1
 
             add ``metadata`` and ``tags`` argument
+
+        .. versionchanged:: 2.0.1
+
+            add ``version_id`` argument
         """
+        # preprocess input arguments
         self.ensure_object()
         dst.ensure_object()
         self.ensure_not_relpath()
         dst.ensure_not_relpath()
+
         if overwrite is False:
             dst.ensure_not_exists(bsm=bsm)
+
+        # prepare API kwargs
         s3_client = resolve_s3_client(context, bsm)
-        return better_client.copy_object(
-            s3_client,
-            src_bucket=self.bucket,
-            src_key=self.key,
-            dst_bucket=dst.bucket,
-            dst_key=dst.key,
-            metadata=metadata,
-            tags=tags,
-            acl=acl,
-            cache_control=cache_control,
-            content_disposition=content_disposition,
-            content_encoding=content_encoding,
-            content_language=content_language,
-            content_md5=content_md5,
-            content_type=content_type,
-            copy_source_if_match=copy_source_if_match,
-            copy_source_if_modified_since=copy_source_if_modified_since,
-            copy_source_if_none_match=copy_source_if_none_match,
-            copy_source_if_unmodified_since=copy_source_if_unmodified_since,
-            expires_datetime=expires_datetime,
-            grant_full_control=grant_full_control,
-            grant_read=grant_read,
-            grant_read_acp=grant_read_acp,
-            grant_write_acp=grant_write_acp,
-            server_side_encryption=server_side_encryption,
-            storage_class=storage_class,
-            website_redirect_location=website_redirect_location,
-            sse_customer_algorithm=sse_customer_algorithm,
-            sse_customer_key=sse_customer_key,
-            sse_kms_key_id=sse_kms_key_id,
-            sse_kms_encryption_context=sse_kms_encryption_context,
-            bucket_key_enabled=bucket_key_enabled,
-            copy_source_sse_customer_algorithm=copy_source_sse_customer_algorithm,
-            copy_source_sse_customer_key=copy_source_sse_customer_key,
-            request_payer=request_payer,
-            object_lock_mode=object_lock_mode,
-            object_lock_retain_until_datetime=object_lock_retain_until_datetime,
-            object_lock_legal_hold_status=object_lock_legal_hold_status,
-            expected_bucket_owner=expected_bucket_owner,
-            expected_source_bucket_owner=expected_source_bucket_owner,
+
+        kwargs = dict(
+            Bucket=dst.bucket,
+            Key=dst.key,
+            CopySource=resolve_kwargs(
+                Bucket=self.bucket,
+                Key=self.key,
+                VersionId=version_id,
+            ),
+            ACL=acl,
+            CacheControl=cache_control,
+            ContentDisposition=content_disposition,
+            ContentEncoding=content_encoding,
+            ContentLanguage=content_language,
+            ContentMD5=content_md5,
+            ContentType=content_type,
+            CopySourceIfMatch=copy_source_if_match,
+            CopySourceIfModifiedSince=copy_source_if_modified_since,
+            CopySourceIfNoneMatch=copy_source_if_none_match,
+            CopySourceIfUnmodifiedSince=copy_source_if_unmodified_since,
+            Expires=expires_datetime,
+            GrantFullControl=grant_full_control,
+            GrantRead=grant_read,
+            GrantReadACP=grant_read_acp,
+            GrantWriteACP=grant_write_acp,
+            ServerSideEncryption=server_side_encryption,
+            StorageClass=storage_class,
+            WebsiteRedirectLocation=website_redirect_location,
+            SSECustomerAlgorithm=sse_customer_algorithm,
+            SSECustomerKey=sse_customer_key,
+            SSEKMSKeyId=sse_kms_key_id,
+            SSEKMSEncryptionContext=sse_kms_encryption_context,
+            BucketKeyEnabled=bucket_key_enabled,
+            CopySourceSSECustomerAlgorithm=copy_source_sse_customer_algorithm,
+            CopySourceSSECustomerKey=copy_source_sse_customer_key,
+            RequestPayer=request_payer,
+            ObjectLockMode=object_lock_mode,
+            ObjectLockRetainUntilDate=object_lock_retain_until_datetime,
+            ObjectLockLegalHoldStatus=object_lock_legal_hold_status,
+            ExpectedBucketOwner=expected_bucket_owner,
+            ExpectedSourceBucketOwner=expected_source_bucket_owner,
         )
+        if metadata is not NOTHING:
+            kwargs["Metadata"] = metadata
+            kwargs["MetadataDirective"] = "REPLACE"
+        if tags is not NOTHING:
+            kwargs["Tagging"] = encode_url_query(tags)
+            kwargs["TaggingDirective"] = "REPLACE"
+        return s3_client.copy_object(**resolve_kwargs(**kwargs))
 
     def copy_dir(
         self: "S3Path",
         dst: "S3Path",
         metadata: T.Optional[MetadataType] = NOTHING,
         tags: T.Optional[TagType] = NOTHING,
         overwrite: bool = False,
@@ -168,38 +190,48 @@
         object_lock_retain_until_datetime: datetime = NOTHING,
         object_lock_legal_hold_status: str = NOTHING,
         expected_bucket_owner: str = NOTHING,
         expected_source_bucket_owner: str = NOTHING,
     ):
         """
         Copy an S3 directory to a different S3 directory, including all
-        sub-directory and files.
+        subdirectory and files.
 
         :param dst: copy to s3 directory, it has to be a directory
         :param overwrite: if False, none of the file will be uploaded / overwritten
-            if any of target s3 location already taken.
+            if any of target s3 location already taken. Note that if the
+            source dir is a versioning enabled bucket, it will always copy
+            the latest version of the object.
 
         :return: number of objects are copied
 
         .. versionadded:: 1.0.1
+
+        TODO: add an argument ``copy_all_history`` to copy all object and all
+            history if the source bucket is versioning enabled.
         """
+        # preprocess input arguments
         self.ensure_dir()
         dst.ensure_dir()
         self.ensure_not_relpath()
         dst.ensure_not_relpath()
+
+        # calculate to do list
         todo: T.List[T.Tuple["S3Path", "S3Path"]] = list()
         for p_src in self.iter_objects(bsm=bsm):
             p_relpath = p_src.relative_to(self)
             p_dst = dst.joinpath(p_relpath)
             todo.append((p_src, p_dst))
 
+        # ensure target location not exists for ``overwrite``
         if overwrite is False:
             for p_src, p_dst in todo:
                 p_dst.ensure_not_exists(bsm=bsm)
 
+        # do real copy
         for p_src, p_dst in todo:
             p_src.copy_file(
                 p_dst,
                 metadata=metadata,
                 tags=tags,
                 overwrite=True,
                 bsm=bsm,
@@ -238,14 +270,15 @@
             )
 
         return len(todo)
 
     def copy_to(
         self: "S3Path",
         dst: "S3Path",
+        version_id: str = NOTHING,
         metadata: T.Optional[MetadataType] = NOTHING,
         tags: T.Optional[TagType] = NOTHING,
         overwrite: bool = False,
         bsm: T.Optional["BotoSesManager"] = None,
         acl: str = NOTHING,
         cache_control: str = NOTHING,
         content_disposition: str = NOTHING,
@@ -279,22 +312,30 @@
         expected_bucket_owner: str = NOTHING,
         expected_source_bucket_owner: str = NOTHING,
     ) -> int:
         """
         Copy s3 object or s3 directory from one place to another place.
 
         :param dst: copy to s3 path
-        :param overwrite: if False, non of the file will be upload / overwritten
-            if any of target s3 location already taken.
+        :param overwrite: if False, none of the file will be uploaded / overwritten
+            if any of target s3 location already taken. Note that if the target
+            S3 location is a versioning enabled bucket, logically you should be
+            able to put a new version to an existing file, but this if
+            ``overwrite`` is True, then it won't allow you to do that. You should
+            set ``overwrite`` to False if you want to put a new version.
 
         .. versionadded:: 1.0.1
 
         .. versionchanged:: 1.3.1
 
             add ``metadata`` and ``tags`` argument
+
+        .. versionchanged:: 2.0.1
+
+            add ``version_id`` argument
         """
         if self.is_dir():
             return self.copy_dir(
                 dst=dst,
                 metadata=metadata,
                 tags=tags,
                 overwrite=overwrite,
@@ -331,14 +372,15 @@
                 object_lock_legal_hold_status=object_lock_legal_hold_status,
                 expected_bucket_owner=expected_bucket_owner,
                 expected_source_bucket_owner=expected_source_bucket_owner,
             )
         elif self.is_file():
             self.copy_file(
                 dst=dst,
+                version_id=version_id,
                 overwrite=overwrite,
                 bsm=bsm,
                 metadata=metadata,
                 tags=tags,
                 acl=acl,
                 cache_control=cache_control,
                 content_disposition=content_disposition,
@@ -417,16 +459,20 @@
         expected_source_bucket_owner: str = NOTHING,
     ) -> int:
         """
         Move s3 object or s3 directory from one place to another place. It is
         firstly :meth:`S3Path.copy_to` then :meth:`S3Path.delete_if_exists`
 
         :param dst: copy to s3 path
-        :param overwrite: if False, non of the file will be upload / overwritten
-            if any of target s3 location already taken.
+        :param overwrite: if False, none of the file will be uploaded / overwritten
+            if any of target s3 location already taken. Note that if the target
+            S3 location is a versioning enabled bucket, logically you should be
+            able to put a new version to an existing file, but this if
+            ``overwrite`` is True, then it won't allow you to do that. You should
+            set ``overwrite`` to False if you want to put a new version.
 
         .. versionadded:: 1.0.1
 
         .. versionchanged:: 1.3.1
 
             add ``metadata`` and ``tags`` argument
         """
@@ -465,9 +511,9 @@
             request_payer=request_payer,
             object_lock_mode=object_lock_mode,
             object_lock_retain_until_datetime=object_lock_retain_until_datetime,
             object_lock_legal_hold_status=object_lock_legal_hold_status,
             expected_bucket_owner=expected_bucket_owner,
             expected_source_bucket_owner=expected_source_bucket_owner,
         )
-        self.delete_if_exists(bsm=bsm)
+        self.delete(bsm=bsm)
         return count
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/delete.py` & `s3pathlib-2.0.1/s3pathlib/core/iter_object_versions.py`

 * *Files 24% similar despite different names*

```diff
@@ -1,77 +1,89 @@
 # -*- coding: utf-8 -*-
 
 """
-Delete S3 file or folder.
+List object versions related API.
+
+.. _bsm: https://github.com/aws-samples/boto-session-manager-project
+.. _ListObjectVersions: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3/paginator/ListObjectVersions.html
 """
 
 import typing as T
+
 from func_args import NOTHING
 
-from .resolve_s3_client import resolve_s3_client
-from .. import utils
 from ..aws import context
+from ..better_client.list_object_versions import paginate_list_object_versions
+from .iter_objects import S3PathIterProxy
+from .resolve_s3_client import resolve_s3_client
 
 if T.TYPE_CHECKING:  # pragma: no cover
     from .s3path import S3Path
     from boto_session_manager import BotoSesManager
 
 
-class DeleteAPIMixin:
+class IterObjectVersionsAPIMixin:
     """
-    A mixin class that implements delete method.
+    A mixin class that implements the iter object versions methods.
     """
 
-    def delete_if_exists(
+    def list_object_versions(
         self: "S3Path",
-        mfa: str = None,
-        version_id: str = None,
-        request_payer: str = None,
-        bypass_governance_retention: bool = None,
-        expected_bucket_owner: str = None,
-        include_folder: bool = True,
+        batch_size: int = 1000,
+        limit: int = NOTHING,
+        delimiter: str = NOTHING,
+        encoding_type: str = NOTHING,
+        expected_bucket_owner: str = NOTHING,
         bsm: T.Optional["BotoSesManager"] = None,
-    ):
+    ) -> S3PathIterProxy:
         """
-        Delete an object or an entire directory. Will do nothing
-        if it doesn't exist.
+        Recursively iterate objects under this prefix, yield :class:`S3Path`.
 
-        Ref: https://boto3.amazonaws.com/v1/documentation/api/latest/reference/services/s3.html#S3.Client.delete_object
+        :param batch_size: Number of s3 object returned per paginator,
+            valid value is from 1 ~ 1000. large number can reduce IO.
+        :param limit: Total number of s3 object to return.
+        :param delimiter: See ListObjectVersions_.
+        :param encoding_type: See ListObjectVersions_.
+        :param expected_bucket_owner: See ListObjectVersions_.
+        :param bsm: See bsm_.
 
-        :param include_folder: see :meth:`iter_objects`
-
-        :return: number of object is deleted
-
-        .. versionadded:: 1.0.1
+        .. versionadded:: 2.0.1
         """
         s3_client = resolve_s3_client(context, bsm)
-        if self.is_file():
-            if self.exists(bsm=bsm):
-                kwargs = dict(
-                    Bucket=self.bucket,
-                    Key=self.key,
-                )
-                additional_kwargs = utils.collect_not_null_kwargs(
-                    MFA=mfa,
-                    VersionId=version_id,
-                    RequestPayer=request_payer,
-                    BypassGovernanceRetention=bypass_governance_retention,
-                    ExpectedBucketOwner=expected_bucket_owner,
-                )
-                kwargs.update(additional_kwargs)
-                s3_client.delete_object(**kwargs)
-                return 1
-            else:
-                return 0
-        elif self.is_dir():
-            return utils.delete_dir(
+        bucket = self.bucket
+
+        def _iter_s3path() -> T.Iterable["S3Path"]:
+            proxy = paginate_list_object_versions(
                 s3_client=s3_client,
-                bucket=self.bucket,
+                bucket=bucket,
                 prefix=self.key,
-                mfa=mfa,
-                request_payer=request_payer,
-                bypass_governance_retention=bypass_governance_retention,
+                batch_size=batch_size,
+                limit=limit,
+                delimiter=delimiter,
+                encoding_type=encoding_type,
                 expected_bucket_owner=expected_bucket_owner,
-                include_folder=include_folder,
             )
-        else:  # pragma: no cover
-            raise ValueError
+            s3path_list = list()
+            for response in proxy:
+                (
+                    versions,
+                    delete_markers,
+                    _,
+                ) = proxy.extract_versions_and_delete_markers_and_common_prefixes(
+                    response
+                )
+
+                s3path_list.extend(
+                    [self._from_version_dict(bucket, dct=dct) for dct in versions]
+                )
+                s3path_list.extend(
+                    [
+                        self._from_delete_marker(bucket, dct=dct)
+                        for dct in delete_markers
+                    ]
+                )
+                for s3path in sorted(
+                    s3path_list, key=lambda x: x.last_modified_at, reverse=True
+                ):
+                    yield s3path
+
+        return S3PathIterProxy(_iter_s3path())
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/filterable_property.py` & `s3pathlib-2.0.1/s3pathlib/core/filterable_property.py`

 * *Files 2% similar despite different names*

```diff
@@ -48,14 +48,17 @@
         self._func = func
 
     def __get__(self, obj: T.Union['FilterableType', None], obj_type):
         if obj is None:
             return self
         return self._func(obj)
 
+    def __set__(self, obj: T.Union['FilterableType', None], value: T.Any):
+        raise AttributeError(f"can't set attribute S3Path.{self.__name__}")
+
     def __eq__(self, other):
         def filter_(obj):
             return self._func(obj) == other
 
         return filter_
 
     def __ne__(self, other):
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/is_test.py` & `s3pathlib-2.0.1/s3pathlib/core/is_test.py`

 * *Files 23% similar despite different names*

```diff
@@ -7,14 +7,20 @@
 - :meth:`~IsTestAPIMixin.is_dir`
 - :meth:`~IsTestAPIMixin.is_file`
 - :meth:`~IsTestAPIMixin.is_bucket`
 """
 
 import typing as T
 
+from ..exc import (
+    S3PathIsNotFolderError,
+    S3PathIsNotFileError,
+)
+from ..constants import IS_DELETE_MARKER
+
 if T.TYPE_CHECKING:  # pragma: no cover
     from .s3path import S3Path
 
 
 class IsTestAPIMixin:
     """
     A mixin class that implements the condition test methods.
@@ -76,22 +82,37 @@
         """
         return (
             (self._bucket is not None)
             and (len(self._parts) == 0)
             and (self._is_dir is True)
         )
 
+    def is_delete_marker(self: "S3Path") -> bool:
+        """
+        Test if it is a delete-marker. A delete-marker is just a version of
+        an object without content.
+
+        .. versionadded:: 2.0.1
+        """
+        if self.is_file():
+            if (self.version_id is not None) and (IS_DELETE_MARKER in self._meta):
+                return True
+            else:
+                return False
+        else:
+            return False
+
     def ensure_object(self: "S3Path") -> None:
         """
         A validator method that ensure it represents a S3 object.
 
         .. versionadded:: 1.0.1
         """
         if self.is_file() is not True:
-            raise TypeError(f"S3 URI: {self} IS NOT a valid s3 object!")
+            raise S3PathIsNotFileError.make(self.uri)
 
     def ensure_file(self: "S3Path") -> None:
         """
         A validator method that ensure it represents a S3 object.
 
         .. versionadded:: 1.2.1
         """
@@ -117,15 +138,15 @@
     def ensure_dir(self: "S3Path") -> None:
         """
         A validator method that ensure it represents a S3 dir.
 
         .. versionadded:: 1.0.1
         """
         if self.is_dir() is not True:
-            raise TypeError(f"{self} IS NOT a valid s3 directory!")
+            raise S3PathIsNotFolderError.make(self.uri)
 
     def ensure_not_dir(self: "S3Path") -> None:
         """
         A validator method that ensure it IS NOT a S3 dir.
 
         .. versionadded:: 1.2.1
         """
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/joinpath.py` & `s3pathlib-2.0.1/s3pathlib/core/joinpath.py`

 * *Files 22% similar despite different names*

```diff
@@ -13,67 +13,14 @@
     from .s3path import S3Path
 
 
 class JoinPathAPIMixin:
     """
     A mixin class that implements the join path operator.
     """
-
-    def join_path(self: "S3Path", *others: "S3Path") -> "S3Path":
-        """
-        Join with other relative path to form a new path
-
-        Example::
-
-            # create some s3path
-            >>> p1 = S3Path("bucket", "folder", "subfolder", "file.txt")
-            >>> p2 = p1.parent
-            >>> relpath1 = p1.relative_to(p2)
-
-            # preview value
-            >>> p1
-            S3Path('s3://bucket/folder/subfolder/file.txt')
-            >>> p2
-            S3Path('s3://bucket/folder/subfolder/')
-            >>> relpath1
-            S3Path('file.txt')
-
-            # join one relative path
-            >>> p2.join_path(relpath1)
-            S3Path('s3://bucket/folder/subfolder/file.txt')
-
-            # join multiple relative path
-            >>> p3 = p2.parent
-            >>> relpath2 = p2.relative_to(p3)
-            >>> p3.join_path(relpath2, relpath1)
-            S3Path('s3://bucket/folder/subfolder/file.txt')
-
-        :param others: many relative path
-
-        :return: a new :class:`S3Path`
-
-        .. versionadded:: 1.0.1
-        """
-        warn_deprecate(
-            func_name="S3Path.join_path",
-            version="2.1.1",
-            message="S3Path.joinpath",
-        )
-        args = [
-            self,
-        ]
-        for relp in others:
-            if relp.is_relpath() is False:
-                msg = (
-                    "you can only join with relative path! " "{} is not a relative path"
-                ).format(relp)
-                raise TypeError(msg)
-            args.append(relp)
-        return self._from_parts(args)
-
     def joinpath(self: "S3Path", *other: T.Union[str, "S3Path"]) -> "S3Path":
         """
         Join with other relative path or string parts.
 
         Example::
 
             # join with string parts
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/metadata.py` & `s3pathlib-2.0.1/s3pathlib/core/metadata.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,46 +1,29 @@
 # -*- coding: utf-8 -*-
 
 """
 Metadata related API.
 """
 
 import typing as T
-import warnings
 from datetime import datetime
 
+from .. import utils
+from ..constants import IS_DELETE_MARKER
+from ..better_client.head_object import head_object
+from ..aws import context
+
 from .resolve_s3_client import resolve_s3_client
 from .filterable_property import FilterableProperty
-from .. import utils, client as better_client
-from ..aws import context
 
 if T.TYPE_CHECKING:  # pragma: no cover
     from .s3path import S3Path
     from boto_session_manager import BotoSesManager
 
 
-def alert_upper_case(metadata: dict):
-    """
-    Alert if there is upper case used in user defined metadata.
-
-    Ref:
-
-    - https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingMetadata.html#UserMetadata
-    """
-    for k, v in metadata.items():
-        if k.lower() != k:
-            msg = (
-                f"based on this document "
-                f"https://docs.aws.amazon.com/AmazonS3/latest/userguide/UsingMetadata.html#UserMetadata "
-                f"Amazon will automatically convert user defined metadata to lower case, "
-                f"but you have a key: {k!r} in metadata"
-            )
-            warnings.warn(msg, UserWarning)
-
-
 class MetadataAPIMixin:
     """
     A mixin class that implements the metadata related methods.
 
     Note:
 
         1. only S3 object can have metadata.
@@ -52,24 +35,29 @@
         self: "S3Path",
         bsm: T.Optional["BotoSesManager"] = None,
     ) -> dict:
         """
         Call head_object() api, store metadata value.
         """
         s3_client = resolve_s3_client(context, bsm)
-        dct = better_client.head_object(s3_client, self.bucket, self.key)
+        dct = head_object(s3_client, self.bucket, self.key)
         self._meta = dct
         return dct
 
     def _get_meta_value(
         self: "S3Path",
         key: str,
         default: T.Any = None,
         bsm: T.Optional["BotoSesManager"] = None,
     ) -> T.Any:
+        """
+        Note:
+
+            This method is for those metadata fields that conditionally exists.
+        """
         if self._meta is None:
             self.head_object(bsm=bsm)
         return self._meta.get(key, default)
 
     def _get_or_pull_meta_value(
         self: "S3Path",
         key: str,
@@ -82,25 +70,29 @@
         """
         value = self._get_meta_value(key, default=None, bsm=bsm)
         if value is None:
             self.head_object(bsm=bsm)
         return self._meta[key]
 
     @FilterableProperty
-    def etag(self: "S3Path") -> str:
+    def etag(self: "S3Path") -> T.Optional[str]:
         """
         For small file, it is the md5 check sum. For large file, because it is
         created from multi part upload, it is the sum of md5 for each part and
         md5 of the sum.
 
         Ref: https://docs.aws.amazon.com/AmazonS3/latest/API/API_Object.html
 
         .. versionadded:: 1.0.1
         """
-        return self._get_or_pull_meta_value(key="ETag")[1:-1]
+        v = self._get_meta_value(key="ETag", default=None)
+        if v is None:
+            return v
+        else:
+            return v[1:-1]
 
     @FilterableProperty
     def last_modified_at(self: "S3Path") -> datetime:
         """
         Ref: https://docs.aws.amazon.com/AmazonS3/latest/API/API_Object.html
 
         .. versionadded:: 1.0.1
@@ -110,50 +102,67 @@
     @FilterableProperty
     def size(self: "S3Path") -> int:
         """
         Ref: https://docs.aws.amazon.com/AmazonS3/latest/API/API_Object.html
 
         .. versionadded:: 1.0.1
         """
-        return self._get_or_pull_meta_value(key="ContentLength")
+        return self._get_meta_value(key="ContentLength", default=0)
 
     @property
     def size_for_human(self: "S3Path") -> str:
         """
-        A human readable string version of the size.
+        A human-readable string version of the size.
 
         .. versionadded:: 1.0.1
         """
         return utils.repr_data_size(self.size)
 
+    @property
+    def _static_version_id(self: "S3Path") -> T.Optional[str]:
+        """
+        This method use the ``self._meta`` to get the version id. Unlike
+        other metadata property methods, this method does not call head_object().
+        """
+        if self._meta is None:
+            return None
+        else:
+            return self._meta.get("VersionId", None)
+
     @FilterableProperty
-    def version_id(self: "S3Path") -> int:
+    def version_id(self: "S3Path") -> T.Optional[str]:
         """
         Only available if you turned on versioning for the bucket.
 
         Ref: https://docs.aws.amazon.com/AmazonS3/latest/API/API_Object.html
 
         .. versionadded:: 1.0.1
+
+        .. versionchanged:: 2.0.1
+
+            return 'null' if it is not a version enabled bucket
         """
-        return self._get_meta_value(key="VersionId")
+        return self._get_meta_value(key="VersionId", default="null")
 
     @FilterableProperty
     def expire_at(self: "S3Path") -> datetime:
         """
-        Only available if you turned on TTL
+        Only available if you turned on TTL.
 
         Ref: https://docs.aws.amazon.com/AmazonS3/latest/API/API_Object.html
 
         .. versionadded:: 1.0.1
         """
         return self._get_meta_value(key="Expires")
 
     @property
     def metadata(self: "S3Path") -> dict:
         """
+        Access the metadata of the object.
+
         Ref: https://docs.aws.amazon.com/AmazonS3/latest/API/API_Object.html
 
         .. versionadded:: 1.0.1
         """
         return self._get_or_pull_meta_value(key="Metadata")
 
     def clear_cache(self: "S3Path") -> None:
@@ -196,15 +205,45 @@
         p = cls(bucket, dct["Key"])
         p._meta = {
             "Key": dct["Key"],
             "LastModified": dct["LastModified"],
             "ETag": dct["ETag"],
             "ContentLength": dct["Size"],
             "StorageClass": dct["StorageClass"],
+            "ChecksumAlgorithm": dct.get("ChecksumAlgorithm", []),
+            "Owner": dct.get("Owner", {}),
+        }
+        return p
+
+    @classmethod
+    def _from_version_dict(cls: T.Type["S3Path"], bucket: str, dct: dict) -> "S3Path":
+        p = cls(bucket, dct["Key"])
+        p._meta = {
+            "Key": dct["Key"],
+            "VersionId": dct["VersionId"],
+            "LastModified": dct["LastModified"],
+            "ETag": dct["ETag"],
+            "ContentLength": dct["Size"],
+            "StorageClass": dct["StorageClass"],
+            "IsLatest": dct["IsLatest"],
+            "ChecksumAlgorithm": dct.get("ChecksumAlgorithm", []),
+            "Owner": dct.get("Owner", {}),
+        }
+        return p
+
+    @classmethod
+    def _from_delete_marker(cls: T.Type["S3Path"], bucket: str, dct: dict) -> "S3Path":
+        p = cls(bucket, dct["Key"])
+        p._meta = {
+            "Key": dct["Key"],
+            "VersionId": dct["VersionId"],
+            "LastModified": dct["LastModified"],
+            "IsLatest": dct["IsLatest"],
             "Owner": dct.get("Owner", {}),
+            IS_DELETE_MARKER: True,
         }
         return p
 
     def update_metadata(self: "S3Path", metadata: dict):  # pragma: no cover
         raise NotImplementedError(
             "You CANNOT only update metadata without changing the content of the "
             "object! You can only do full replace ment via the .write_text() or "
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/relative.py` & `s3pathlib-2.0.1/s3pathlib/core/relative.py`

 * *Files 3% similar despite different names*

```diff
@@ -71,31 +71,34 @@
     def relative_to(self: "S3Path", other: "S3Path") -> "S3Path":
         """
         Return the relative path to another path. If the operation
         is not possible (because this is not a sub path of the other path),
         raise ``ValueError``.
 
         ``-`` is a syntax sugar for ``relative_to``. See more information at
-        :meth:`~S3Path.__sub__`.
+        :meth:`~RelativePathAPIMixin.__sub__`.
 
-        The relative path usually works with :meth:`join_path` to form a new
-        path. Or you can use the ``/`` syntax sugar as well. See more
-        information at :meth:`~S3Path.__truediv__`.
+        The relative path usually works with
+        :meth:`~s3pathlib.core.joinpath.JoinPathAPIMixin.joinpath` to form a new
+        path. Or you can use the ``/`` syntax sugar as well.
 
         Examples::
 
             >>> S3Path("bucket", "a/b/c").relative_to(S3Path("bucket", "a")).parts
             ['b', 'c']
 
             >>> S3Path("bucket", "a").relative_to(S3Path("bucket", "a")).parts
             []
 
             >>> S3Path("bucket", "a").relative_to(S3Path("bucket", "a/b/c")).parts
             ValueError ...
 
+            >>> S3Path("bucket") / S3Path("new_bucket/file.txt").relative_to(S3Path("new_bucket"))
+            S3Path('s3://bucket/file.txt')
+
         :param other: other :class:`S3Path` instance.
 
         :return: a relative path object, which is a special version of S3Path
 
         .. versionadded:: 1.0.1
         """
         if (
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/s3path.py` & `s3pathlib-2.0.1/s3pathlib/core/s3path.py`

 * *Files 19% similar despite different names*

```diff
@@ -14,14 +14,15 @@
 from .attribute import AttributeAPIMixin
 from .joinpath import JoinPathAPIMixin
 from .mutate import MutateAPIMixin
 from .metadata import MetadataAPIMixin
 from .bucket import BucketAPIMixin
 from .tagging import TaggingAPIMixin
 from .iter_objects import IterObjectsAPIMixin
+from .iter_object_versions import IterObjectVersionsAPIMixin
 from .exists import ExistsAPIMixin
 from .rw import ReadAndWriteAPIMixin
 from .delete import DeleteAPIMixin
 from .upload import UploadAPIMixin
 from .copy import CopyAPIMixin
 from .sync import SyncAPIMixin
 from .serde import SerdeAPIMixin
@@ -37,14 +38,15 @@
     AttributeAPIMixin,
     JoinPathAPIMixin,
     MutateAPIMixin,
     MetadataAPIMixin,
     BucketAPIMixin,
     TaggingAPIMixin,
     IterObjectsAPIMixin,
+    IterObjectVersionsAPIMixin,
     ExistsAPIMixin,
     ReadAndWriteAPIMixin,
     DeleteAPIMixin,
     UploadAPIMixin,
     CopyAPIMixin,
     SyncAPIMixin,
     SerdeAPIMixin,
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/serde.py` & `s3pathlib-2.0.1/s3pathlib/core/serde.py`

 * *Files identical despite different names*

### Comparing `s3pathlib-1.4.1/s3pathlib/core/sync.py` & `s3pathlib-2.0.1/s3pathlib/core/sync.py`

 * *Files 13% similar despite different names*

```diff
@@ -39,21 +39,32 @@
         include: T.Optional[str] = None,
         exclude: T.Optional[str] = None,
         acl: T.Optional[str] = None,
         only_show_errors: bool = False,
         no_progress: bool = False,
         page_size: T.Optional[str] = None,
         delete: bool = False,
+        verbose: bool = True,
     ):
         """
         Implement the `aws s3 sync <https://docs.aws.amazon.com/cli/latest/reference/s3/sync.html>`_
         CLI behavior.
 
         :param src:
         :param dst:
+        :param bsm:
+        :param quite:
+        :param include:
+        :param exclude:
+        :param acl:
+        :param only_show_errors:
+        :param no_progress:
+        :param page_size:
+        :param delete:
+        :param verbose:
 
         .. versionadded:: 1.2.1
 
         TODO: add support for all aws s3 sync supported arguments
         """
         args = [
             "aws",
@@ -106,15 +117,16 @@
         if page_size:  # pragma: no cover
             args.extend(["--page-size", str(page_size)])
         if delete:  # pragma: no cover
             args.append("--delete")
 
         if bsm is None:  # pragma: no cover
             with BotoSesManager(botocore_session=context.boto_ses._session).awscli():
-                print(" ".join(args))
+                if verbose:
+                    print(" ".join(args))
                 response = subprocess.run(args)
         else:  # pragma: no cover
             with bsm.awscli():
                 response = subprocess.run(args)
         if response.returncode != 0:  # pragma: no cover
             raise SystemError("'aws s3 sync' command failed!")
 
@@ -126,14 +138,15 @@
         include: T.Optional[str] = None,
         exclude: T.Optional[str] = None,
         acl: T.Optional[str] = None,
         only_show_errors: bool = False,
         no_progress: bool = False,
         page_size: T.Optional[str] = None,
         delete: bool = False,
+        verbose: bool = True,
     ):
         """
         Sync data from external place to this S3 location.
         """
         return self.sync(
             src=src,
             dst=self,
@@ -142,28 +155,30 @@
             include=include,
             exclude=exclude,
             acl=acl,
             only_show_errors=only_show_errors,
             no_progress=no_progress,
             page_size=page_size,
             delete=delete,
+            verbose=verbose,
         )
 
     def sync_to(
         self: "S3Path",
         dst: T.Union["S3Path", PathType],
         bsm: T.Optional["BotoSesManager"] = None,
         quite: bool = True,
         include: T.Optional[str] = None,
         exclude: T.Optional[str] = None,
         acl: T.Optional[str] = None,
         only_show_errors: bool = False,
         no_progress: bool = False,
         page_size: T.Optional[str] = None,
         delete: bool = False,
+        verbose: bool = True,
     ):
         """
         Sync the data at this S3 location to external place.
         """
         return self.sync(
             src=self,
             dst=dst,
@@ -172,8 +187,9 @@
             include=include,
             exclude=exclude,
             acl=acl,
             only_show_errors=only_show_errors,
             no_progress=no_progress,
             page_size=page_size,
             delete=delete,
+            verbose=verbose,
         )
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/upload.py` & `s3pathlib-2.0.1/s3pathlib/core/upload.py`

 * *Files 6% similar despite different names*

```diff
@@ -5,21 +5,22 @@
 """
 
 import typing as T
 
 from pathlib_mate import Path
 
 from .resolve_s3_client import resolve_s3_client
-from .. import utils
+from ..better_client.upload import upload_dir
 from ..type import PathType
 from ..aws import context
 
 if T.TYPE_CHECKING:  # pragma: no cover
     from .s3path import S3Path
     from boto_session_manager import BotoSesManager
+    from mypy_boto3_s3.type_defs import UploadFile
 
 
 class UploadAPIMixin:
     """
     A mixin class that implements upload method.
     """
 
@@ -27,15 +28,15 @@
         self: "S3Path",
         path: PathType,
         overwrite: bool = False,
         extra_args: dict = None,
         callback: callable = None,
         config=None,
         bsm: T.Optional["BotoSesManager"] = None,
-    ) -> dict:
+    ):
         """
         Upload a file from local file system to targeted S3 path
 
         Example::
 
             >>> s3path = S3Path("bucket", "artifacts", "deployment.zip")
             >>> s3path.upload_file(path="/tmp/build/deployment.zip", overwrite=True)
@@ -49,15 +50,15 @@
         """
         self.ensure_object()
         if overwrite is False:
             self.ensure_not_exists(bsm=bsm)
         p = Path(path)
         s3_client = resolve_s3_client(context, bsm)
         return s3_client.upload_file(
-            p.abspath,
+            Filename=p.abspath,
             Bucket=self.bucket,
             Key=self.key,
             ExtraArgs=extra_args,
             Callback=callback,
             Config=config,
         )
 
@@ -88,15 +89,15 @@
 
         :return: number of files uploaded
 
         .. versionadded:: 1.0.1
         """
         self.ensure_dir()
         s3_client = resolve_s3_client(context, bsm)
-        return utils.upload_dir(
+        return upload_dir(
             s3_client=s3_client,
             bucket=self.bucket,
             prefix=self.key,
             local_dir=local_dir,
             pattern=pattern,
             overwrite=overwrite,
         )
```

### Comparing `s3pathlib-1.4.1/s3pathlib/core/uri.py` & `s3pathlib-2.0.1/s3pathlib/core/uri.py`

 * *Files 19% similar despite different names*

```diff
@@ -110,38 +110,52 @@
             )
         else:
             return "s3://{}/".format(self._bucket)
 
     @property
     def console_url(self: 'S3Path') -> T.Optional[str]:
         """
-        Return an AWS S3 Console url that can inspect the details.
+        Return an url that can inspect the object, directory details in AWS Console.
 
         .. versionadded:: 1.0.1
+
+        .. versionchanged:: 2.0.1
+
+            now take the version id into consideration.
         """
         uri: str = self.uri
         if uri is None:
             return None
         else:
-            console_url = utils.make_s3_console_url(s3_uri=uri)
+            console_url = utils.make_s3_console_url(
+                s3_uri=uri,
+                version_id=self._static_version_id,
+            )
             return console_url
 
     @property
     def us_gov_cloud_console_url(self: 'S3Path') -> T.Optional[str]:
         """
-        Return an AWS US Gov Cloud S3 Console url that can inspect the details.
+        Return a Gov Cloud url that can inspect the object, directory details
+        in AWS Console.
 
         .. versionadded:: 1.0.5
+
+        .. versionchanged:: 2.0.1
+
+            now take the version id into consideration.
         """
         uri: str = self.uri
         if uri is None:
             return None
         else:
             console_url = utils.make_s3_console_url(
-                s3_uri=uri, is_us_gov_cloud=True
+                s3_uri=uri,
+                version_id=self._static_version_id,
+                is_us_gov_cloud=True,
             )
             return console_url
 
     @property
     def s3_select_console_url(self: 'S3Path') -> T.Optional[str]:
         """
         Return an AWS US Gov Cloud S3 Console url that can inspect data with s3 select.
@@ -207,13 +221,19 @@
         validate.validate_s3_uri(uri)
         bucket, key = utils.split_s3_uri(uri)
         return cls._from_parts([bucket, key])
 
     @classmethod
     def from_s3_arn(cls: T.Type['S3Path'], arn: str) -> 'S3Path':
         """
+        Construct an :class:`S3Path` from S3 ARN.
+
+        >>> p = S3Path.from_s3_arn("arn:aws:s3:::bucket/folder/file.txt")
+
+        >>> p
+        S3Path('s3://bucket/folder/file.txt')
 
-        :param arn:
-        :return:
+        >>> p.arn
+        'arn:aws:s3:::bucket/folder/file.txt'
         """
         validate.validate_s3_arn(arn)
         return cls._from_parts([arn.replace("arn:aws:s3:::", "", 1), ])
```

### Comparing `s3pathlib-1.4.1/s3pathlib/marker.py` & `s3pathlib-2.0.1/s3pathlib/marker.py`

 * *Files identical despite different names*

### Comparing `s3pathlib-1.4.1/s3pathlib/tests/helpers.py` & `s3pathlib-2.0.1/s3pathlib/tests/helpers.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # -*- coding: utf-8 -*-
 
 import sys
 import subprocess
 
-from .paths import dir_project_root, dir_htmlcov, bin_pytest
+from .paths import dir_project_root, dir_htmlcov, path_cov_index_html, bin_pytest
 
 if sys.platform == "win32":
     open_cmd = "open"
 else:
     open_cmd = "open"
 
 
@@ -33,45 +33,30 @@
         coverage
     :param root_dir: the dir to dump coverage results binary file
     :param htmlcov_dir: the dir to dump HTML output
     """
     module = normalize_module(module)
     args = [
         bin_pytest,
-        "-s", "--tb=native",
+        "-s",
+        "--tb=native",
         f"--rootdir={root_dir}",
         f"--cov={module}",
-        "--cov-report", "term-missing",
-        "--cov-report", f"html:{htmlcov_dir}",
+        "--cov-report",
+        "term-missing",
+        "--cov-report",
+        f"html:{htmlcov_dir}",
         script,
     ]
     subprocess.run(args)
 
 
-def run_cov_test(script: str, module: str, open_browser: bool = False):
+def run_cov_test(script: str, module: str, preview: bool = False):
     _run_cov_test(
         bin_pytest=f"{bin_pytest}",
         script=script,
         module=module,
         root_dir=f"{dir_project_root}",
         htmlcov_dir=f"{dir_htmlcov}",
     )
-    if open_browser:
-        _open_cov_report(module)
-
-
-def _open_cov_report(module: str):
-    module = normalize_module(module)
-    parts = module.split(".")
-    module_name = parts[-1]
-    module_path = str(dir_project_root.joinpath(*parts)) + ".py"
-    print(module_path)
-    found_cov_report_html = False
-    html_path = None
-    for p in dir_htmlcov.glob("**/*_py.html"):
-        if p.name.endswith(f"{module_name}_py.html"):
-            if module_path in p.read_text():
-                found_cov_report_html = True
-                html_path = str(p)
-                break
-    if found_cov_report_html:
-        subprocess.run([open_cmd, html_path])
+    if preview:
+        subprocess.run(["open", f"{path_cov_index_html}"])
```

### Comparing `s3pathlib-1.4.1/s3pathlib/validate.py` & `s3pathlib-2.0.1/s3pathlib/validate.py`

 * *Files identical despite different names*

### Comparing `s3pathlib-1.4.1/s3pathlib.egg-info/PKG-INFO` & `s3pathlib-2.0.1/s3pathlib.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 Metadata-Version: 2.1
 Name: s3pathlib
-Version: 1.4.1
+Version: 2.0.1
 Summary: Objective Oriented Interface for AWS S3, similar to pathlib.
 Home-page: https://github.com/aws-samples/s3pathlib-project
-Download-URL: https://pypi.python.org/pypi/s3pathlib/1.4.1#downloads
+Download-URL: https://pypi.python.org/pypi/s3pathlib/2.0.1#downloads
 Author: Sanhe Hu
 Author-email: husanhe@gmail.com
 Maintainer: Sanhe Hu
 Maintainer-email: sanhehu@amazon.com
 License: Apache License 2.0
 Platform: Windows
 Platform: MacOS
@@ -18,15 +18,14 @@
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Operating System :: MacOS
 Classifier: Operating System :: Unix
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3 :: Only
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Provides-Extra: tests
 Provides-Extra: docs
 License-File: LICENSE
@@ -36,26 +35,32 @@
 .. image:: https://readthedocs.org/projects/s3pathlib/badge/?version=latest
     :target: https://s3pathlib.readthedocs.io/en/latest/
     :alt: Documentation Status
 
 .. image:: https://github.com/aws-samples/s3pathlib-project/workflows/CI/badge.svg
     :target: https://github.com/aws-samples/s3pathlib-project/actions?query=workflow:CI
 
+.. image:: https://img.shields.io/badge/codecov-100%25-brightgreen
+    :target: https://github.com/aws-samples/s3pathlib-project/actions?query=workflow:CI
+
 .. image:: https://img.shields.io/pypi/v/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
 
 .. image:: https://img.shields.io/pypi/l/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
 
 .. image:: https://img.shields.io/pypi/pyversions/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
     
 .. image:: https://img.shields.io/pypi/dm/s3pathlib.svg
     :target: https://pypi.python.org/pypi/s3pathlib
 
+.. image:: https://img.shields.io/badge/STAR_Me_on_GitHub!--None.svg?style=social
+    :target: https://github.com/aws-samples/s3pathlib-project
+
 ------
 
 .. image:: https://img.shields.io/badge/Link-Document-orange.svg
     :target: https://s3pathlib.readthedocs.io/en/latest/
 
 .. image:: https://img.shields.io/badge/Link-API-blue.svg
     :target: https://s3pathlib.readthedocs.io/en/latest/py-modindex.html
@@ -71,38 +76,40 @@
 
 .. image:: https://img.shields.io/badge/Link-Download-blue.svg
     :target: https://pypi.org/pypi/s3pathlib#files
 
 
 Welcome to ``s3pathlib`` Documentation
 ==============================================================================
-
-``s3pathlib`` is the python package provides the Pythonic objective oriented programming (OOP) interface to manipulate AWS S3 object / directory. The api is similar to the ``pathlib`` `standard library <https://docs.python.org/3/library/pathlib.html>`_ and very intuitive for human.
+`s3pathlib <https://s3pathlib.readthedocs.io/en/latest/>`_ is a Python package that offers an object-oriented programming (OOP) interface to work with AWS S3 objects and directories. Its API is designed to be similar to the standard library `pathlib <https://docs.python.org/3/library/pathlib.html>`_ and is user-friendly. The package also `supports versioning <https://docs.aws.amazon.com/AmazonS3/latest/userguide/Versioning.html>`_ in AWS S3.
 
 .. note::
 
-    You may not viewing the full document, `FULL DOCUMENT IS HERE <https://s3pathlib.readthedocs.io/en/latest/>`_
+    You may not be viewing the full document, `FULL DOCUMENT IS HERE <https://s3pathlib.readthedocs.io/en/latest/>`_
 
 
 Quick Start
 ------------------------------------------------------------------------------
 .. note::
 
-    `COMPREHENSIVE DOCUMENT guide / features / best practice can be found at HERE <https://s3pathlib.readthedocs.io/en/latest/#full-table-of-content>`_
-
+    `COMPREHENSIVE DOCUMENT guide / features / best practice can be found at HERE <https://s3pathlib.readthedocs.io/en/latest/#comprehensive-guide>`_
 
-**Import the library, declare a S3 object**
+**Import the library, declare an S3Path object**
 
 .. code-block:: python
 
     # import
     >>> from s3pathlib import S3Path
 
     # construct from string, auto join parts
     >>> p = S3Path("bucket", "folder", "file.txt")
+    # construct from S3 URI works too
+    >>> p = S3Path("s3://bucket/folder/file.txt")
+    # construct from S3 ARN works too
+    >>> p = S3Path("arn:aws:s3:::bucket/folder/file.txt")
     >>> p.bucket
     'bucket'
     >>> p.key
     'folder/file.txt'
     >>> p.uri
     's3://bucket/folder/file.txt'
     >>> p.console_url # click to preview it in AWS console
@@ -122,14 +129,15 @@
     ...     boto3.session.Session(
     ...         region_name="us-east-1",
     ...         profile_name="my_aws_profile",
     ...     )
     ... )
 
     >>> p = S3Path("bucket", "folder", "file.txt")
+    >>> p.write_text("a lot of data ...")
     >>> p.etag
     '3e20b77868d1a39a587e280b99cec4a8'
     >>> p.size
     56789000
     >>> p.size_for_human
     '51.16 MB'
 
@@ -155,25 +163,25 @@
     >>> p.upload_dir("/my-repo", pattern="**/*.py", overwrite=False)
 
     # copy entire s3 folder to another s3 folder
     >>> p2 = S3Path("bucket", "github", "repos", "another-repo/")
     >>> p1.copy_to(p2, overwrite=True)
 
     # delete all objects in the folder, recursively, to clean up your test bucket
-    >>> p.delete_if_exists()
-    >>> p2.delete_if_exists()
+    >>> p.delete()
+    >>> p2.delete()
 
 **S3 Path Filter**
 
 Ever think of filter S3 object by it's attributes like: dirname, basename, file extension, etag, size, modified time? It is supposed to be simple in Python:
 
 .. code-block:: python
 
-    >>> root = S3Path("bucket") # assume you have a lots of files in this bucket
-    >>> iterproxy = root.iter_objects().filter(
+    >>> s3bkt = S3Path("bucket") # assume you have a lots of files in this bucket
+    >>> iterproxy = s3bkt.iter_objects().filter(
     ...     S3Path.size >= 10_000_000, S3Path.ext == ".csv" # add filter
     ... )
 
     >>> iterproxy.one() # fetch one
     S3Path('s3://bucket/larger-than-10MB-1.csv')
 
     >>> iterproxy.many(3) # fetch three
@@ -208,26 +216,25 @@
     # pandas IO
     >>> import pandas as pd
     >>> p = S3Path("bucket", "dataset.csv")
     >>> df = pd.DataFrame(...)
     >>> with p.open("w") as f:
     ...     df.to_csv(f)
 
+Now that you have a basic understanding of s3pathlib, let's read the `full document <https://s3pathlib.readthedocs.io/en/latest/#comprehensive-guide>`_ to explore its capabilities in greater depth.
+
 
 Getting Help
 ------------------------------------------------------------------------------
 Please use the ``python-s3pathlib`` tag on Stack Overflow to get help.
 
 Submit a ``I want help`` issue tickets on `GitHub Issues <https://github.com/aws-samples/s3pathlib-project/issues/new/choose>`_
 
 
-
 Contributing
 ------------------------------------------------------------------------------
 Please see the `Contribution Guidelines <https://github.com/aws-samples/s3pathlib-project/blob/main/CONTRIBUTING.rst>`_.
 
 
 Copyright
 ------------------------------------------------------------------------------
 s3pathlib is an open source project. See the `LICENSE <https://github.com/aws-samples/s3pathlib-project/blob/main/LICENSE>`_ file for more information.
-
-
```

### Comparing `s3pathlib-1.4.1/setup.py` & `s3pathlib-2.0.1/setup.py`

 * *Files 0% similar despite different names*

```diff
@@ -131,15 +131,14 @@
         "Intended Audience :: Developers",
         "Natural Language :: English",
         "Operating System :: Microsoft :: Windows",
         "Operating System :: MacOS",
         "Operating System :: Unix",
         "Programming Language :: Python",
         "Programming Language :: Python :: 3 :: Only",
-        "Programming Language :: Python :: 3.6",
         "Programming Language :: Python :: 3.7",
         "Programming Language :: Python :: 3.8",
         "Programming Language :: Python :: 3.9",
         "Programming Language :: Python :: 3.10",
     ]
     """
     Full list can be found at: https://pypi.python.org/pypi?%3Aaction=list_classifiers
```

