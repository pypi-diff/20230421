# Comparing `tmp/file-io-0.4.5.tar.gz` & `tmp/file-io-0.4.6.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "file-io-0.4.5.tar", last modified: Sat Feb 11 06:24:11 2023, max compression
+gzip compressed data, was "file-io-0.4.6.tar", last modified: Fri Apr 21 03:49:37 2023, max compression
```

## Comparing `file-io-0.4.5.tar` & `file-io-0.4.6.tar`

### file list

```diff
@@ -1,71 +1,71 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.982573 file-io-0.4.5/
--rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-02-11 06:23:55.000000 file-io-0.4.5/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-02-11 06:24:11.982573 file-io-0.4.5/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-02-11 06:23:55.000000 file-io-0.4.5/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.966573 file-io-0.4.5/file_io.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-02-11 06:24:11.000000 file-io-0.4.5/file_io.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-02-11 06:24:11.000000 file-io-0.4.5/file_io.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-02-11 06:24:11.000000 file-io-0.4.5/file_io.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      106 2023-02-11 06:24:11.000000 file-io-0.4.5/file_io.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-02-11 06:24:11.000000 file-io-0.4.5/file_io.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.966573 file-io-0.4.5/fileio/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.966573 file-io-0.4.5/fileio/aiopath/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/aiopath/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/aiopath/handle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/aiopath/scandir.py
--rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/aiopath/selectors.py
--rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/aiopath/wrap.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.970573 file-io-0.4.5/fileio/converters/
--rw-r--r--   0 runner    (1001) docker     (123)       58 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/converters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    26321 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/converters/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/converters/static.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.970573 file-io-0.4.5/fileio/core/
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    54396 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/core/_pathlib.py
--rw-r--r--   0 runner    (1001) docker     (123)    50842 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/core/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/core/baselib.py
--rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/core/flavours.py
--rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/core/generic.py
--rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/core/imports.py
--rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/core/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/core/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.974573 file-io-0.4.5/fileio/io/
--rw-r--r--   0 runner    (1001) docker     (123)      747 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      478 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_base.py
--rw-r--r--   0 runner    (1001) docker     (123)      966 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_base64.py
--rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_base64gzip.py
--rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_csv.py
--rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_generator.py
--rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_jsonlines.py
--rw-r--r--   0 runner    (1001) docker     (123)      632 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_msgpack.py
--rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_pickle.py
--rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_text.py
--rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_tsv.py
--rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/io/_yaml.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.978573 file-io-0.4.5/fileio/providers/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/providers/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/providers/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    22049 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/providers/filesys.py
--rw-r--r--   0 runner    (1001) docker     (123)    59038 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/providers/filesys_cloud.py
--rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/providers/gs_gcp.py
--rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/providers/methods.py
--rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/providers/s3_aws.py
--rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/providers/s3_minio.py
--rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/providers/tfio.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.978573 file-io-0.4.5/fileio/types/
--rw-r--r--   0 runner    (1001) docker     (123)      174 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/types/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    40893 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/types/classprops.py
--rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/types/common.py
--rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/types/etc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-02-11 06:24:11.982573 file-io-0.4.5/fileio/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      371 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/utils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    14580 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/utils/configs.py
--rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/utils/helpers.py
--rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/utils/lazylib.py
--rw-r--r--   0 runner    (1001) docker     (123)     4929 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/utils/logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/utils/ops.py
--rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-02-11 06:23:55.000000 file-io-0.4.5/fileio/utils/pooler.py
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-02-11 06:24:11.982573 file-io-0.4.5/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1445 2023-02-11 06:23:55.000000 file-io-0.4.5/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.528871 file-io-0.4.6/
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-21 03:49:25.000000 file-io-0.4.6/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-21 03:49:37.528871 file-io-0.4.6/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7621 2023-04-21 03:49:25.000000 file-io-0.4.6/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.524871 file-io-0.4.6/file_io.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     8204 2023-04-21 03:49:37.000000 file-io-0.4.6/file_io.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1394 2023-04-21 03:49:37.000000 file-io-0.4.6/file_io.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:49:37.000000 file-io-0.4.6/file_io.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      120 2023-04-21 03:49:37.000000 file-io-0.4.6/file_io.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 03:49:37.000000 file-io-0.4.6/file_io.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.524871 file-io-0.4.6/fileio/
+-rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.524871 file-io-0.4.6/fileio/aiopath/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/aiopath/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4516 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/aiopath/handle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1543 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/aiopath/scandir.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5864 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/aiopath/selectors.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1294 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/aiopath/wrap.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.524871 file-io-0.4.6/fileio/converters/
+-rw-r--r--   0 runner    (1001) docker     (123)       58 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/converters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26321 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/converters/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/converters/static.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.524871 file-io-0.4.6/fileio/core/
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    54396 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/core/_pathlib.py
+-rw-r--r--   0 runner    (1001) docker     (123)    50842 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/core/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/core/baselib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6364 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/core/flavours.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4483 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/core/generic.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3692 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/core/imports.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7222 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/core/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1448 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/core/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.528871 file-io-0.4.6/fileio/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      478 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)      966 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_base64.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1079 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_base64gzip.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3340 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_csv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1678 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_generator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2985 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4623 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_jsonlines.py
+-rw-r--r--   0 runner    (1001) docker     (123)      632 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_msgpack.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1018 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_pickle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1320 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_text.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3362 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_tsv.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3129 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/io/_yaml.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.528871 file-io-0.4.6/fileio/providers/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/providers/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1948 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/providers/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22049 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/providers/filesys.py
+-rw-r--r--   0 runner    (1001) docker     (123)    59038 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/providers/filesys_cloud.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8217 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/providers/gs_gcp.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3209 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/providers/methods.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7093 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/providers/s3_aws.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7253 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/providers/s3_minio.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3481 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/providers/tfio.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.528871 file-io-0.4.6/fileio/types/
+-rw-r--r--   0 runner    (1001) docker     (123)      174 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/types/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    40893 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/types/classprops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5551 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/types/common.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11699 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/types/etc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:49:37.528871 file-io-0.4.6/fileio/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      371 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/utils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14580 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/utils/configs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7429 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/utils/helpers.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11665 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/utils/lazylib.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4930 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/utils/logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4822 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/utils/ops.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2860 2023-04-21 03:49:25.000000 file-io-0.4.6/fileio/utils/pooler.py
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 03:49:37.528871 file-io-0.4.6/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1459 2023-04-21 03:49:25.000000 file-io-0.4.6/setup.py
```

### Comparing `file-io-0.4.5/LICENSE` & `file-io-0.4.6/LICENSE`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/PKG-INFO` & `file-io-0.4.6/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-io
-Version: 0.4.5
+Version: 0.4.6
 Summary: Deterministic File Lib to make working with Files across Object Storage easier
 Home-page: https://github.com/trisongz/file-io
 Author: Tri Songz
 Author-email: ts@growthengineai.com
 License: MIT Style
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `file-io-0.4.5/README.md` & `file-io-0.4.6/README.md`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/file_io.egg-info/PKG-INFO` & `file-io-0.4.6/file_io.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: file-io
-Version: 0.4.5
+Version: 0.4.6
 Summary: Deterministic File Lib to make working with Files across Object Storage easier
 Home-page: https://github.com/trisongz/file-io
 Author: Tri Songz
 Author-email: ts@growthengineai.com
 License: MIT Style
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `file-io-0.4.5/file_io.egg-info/SOURCES.txt` & `file-io-0.4.6/file_io.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/__init__.py` & `file-io-0.4.6/fileio/__init__.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/aiopath/handle.py` & `file-io-0.4.6/fileio/aiopath/handle.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/aiopath/scandir.py` & `file-io-0.4.6/fileio/aiopath/scandir.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/aiopath/selectors.py` & `file-io-0.4.6/fileio/aiopath/selectors.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/aiopath/wrap.py` & `file-io-0.4.6/fileio/aiopath/wrap.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/converters/base.py` & `file-io-0.4.6/fileio/converters/base.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/converters/static.py` & `file-io-0.4.6/fileio/converters/static.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/core/_pathlib.py` & `file-io-0.4.6/fileio/core/_pathlib.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/core/base.py` & `file-io-0.4.6/fileio/core/base.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/core/flavours.py` & `file-io-0.4.6/fileio/core/flavours.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/core/generic.py` & `file-io-0.4.6/fileio/core/generic.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/core/imports.py` & `file-io-0.4.6/fileio/core/imports.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/core/types.py` & `file-io-0.4.6/fileio/core/types.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/core/utils.py` & `file-io-0.4.6/fileio/core/utils.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/__init__.py` & `file-io-0.4.6/fileio/io/__init__.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_base64.py` & `file-io-0.4.6/fileio/io/_base64.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_base64gzip.py` & `file-io-0.4.6/fileio/io/_base64gzip.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_csv.py` & `file-io-0.4.6/fileio/io/_csv.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_generator.py` & `file-io-0.4.6/fileio/io/_generator.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_json.py` & `file-io-0.4.6/fileio/io/_json.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_jsonlines.py` & `file-io-0.4.6/fileio/io/_jsonlines.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_msgpack.py` & `file-io-0.4.6/fileio/io/_msgpack.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_pickle.py` & `file-io-0.4.6/fileio/io/_pickle.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_text.py` & `file-io-0.4.6/fileio/io/_text.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_tsv.py` & `file-io-0.4.6/fileio/io/_tsv.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/io/_yaml.py` & `file-io-0.4.6/fileio/io/_yaml.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/providers/base.py` & `file-io-0.4.6/fileio/providers/base.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/providers/filesys.py` & `file-io-0.4.6/fileio/providers/filesys.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/providers/filesys_cloud.py` & `file-io-0.4.6/fileio/providers/filesys_cloud.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/providers/gs_gcp.py` & `file-io-0.4.6/fileio/providers/gs_gcp.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/providers/methods.py` & `file-io-0.4.6/fileio/providers/methods.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/providers/s3_aws.py` & `file-io-0.4.6/fileio/providers/s3_aws.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/providers/s3_minio.py` & `file-io-0.4.6/fileio/providers/s3_minio.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/providers/tfio.py` & `file-io-0.4.6/fileio/providers/tfio.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/types/classprops.py` & `file-io-0.4.6/fileio/types/classprops.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/types/common.py` & `file-io-0.4.6/fileio/types/common.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/types/etc.py` & `file-io-0.4.6/fileio/types/etc.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/utils/configs.py` & `file-io-0.4.6/fileio/utils/configs.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/utils/helpers.py` & `file-io-0.4.6/fileio/utils/helpers.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/utils/lazylib.py` & `file-io-0.4.6/fileio/utils/lazylib.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/utils/logs.py` & `file-io-0.4.6/fileio/utils/logs.py`

 * *Files 0% similar despite different names*

```diff
@@ -75,15 +75,15 @@
     exception=None,
     depth=0,
     record=False,
     lazy=False,
     colors=False,
     raw=False,
     capture=True,
-    patcher=None,
+    patchers=None,
     extra={},
 )
 
 if _defaults.LOGURU_AUTOINIT and sys.stderr:
     logger.add(sys.stderr)
 
 _atexit.register(logger.remove)
```

### Comparing `file-io-0.4.5/fileio/utils/ops.py` & `file-io-0.4.6/fileio/utils/ops.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/fileio/utils/pooler.py` & `file-io-0.4.6/fileio/utils/pooler.py`

 * *Files identical despite different names*

### Comparing `file-io-0.4.5/setup.py` & `file-io-0.4.6/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 import sys
 from pathlib import Path
 from setuptools import setup, find_packages
 
 if sys.version_info.major != 3:
     raise RuntimeError("This package requires Python 3+")
 
-version = '0.4.5'
+version = '0.4.6'
 pkg_name = 'file-io'
 gitrepo = 'trisongz/file-io'
 root = Path(__file__).parent
 
 requirements = [
     'anyio',
     'aiofile',
     #'aiopath', # remove deps as 3.10 vs 3.9 is different
     'fsspec',
-    'loguru',
+    'loguru>=0.7.0,<0.8.0',
     'pydantic',
     'dill',
     'frozendict',
     'aiohttpx',
 ]
 
 extras = {
```

