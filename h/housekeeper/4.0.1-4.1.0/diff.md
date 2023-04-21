# Comparing `tmp/housekeeper-4.0.1.tar.gz` & `tmp/housekeeper-4.1.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/housekeeper-4.0.1.tar", last modified: Thu Mar 23 14:49:59 2023, max compression
+gzip compressed data, was "dist/housekeeper-4.1.0.tar", last modified: Fri Apr 21 14:00:47 2023, max compression
```

## Comparing `housekeeper-4.0.1.tar` & `housekeeper-4.1.0.tar`

### file list

```diff
@@ -1,102 +1,102 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/
--rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-03-23 14:49:50.000000 housekeeper-4.0.1/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)      195 2023-03-23 14:49:50.000000 housekeeper-4.0.1/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-03-23 14:49:59.000000 housekeeper-4.0.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-03-23 14:49:50.000000 housekeeper-4.0.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/housekeeper/
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      325 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/__main__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/housekeeper/archive/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/archive/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/housekeeper/cli/
--rw-r--r--   0 runner    (1001) docker     (123)       47 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/cli/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6006 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/cli/add.py
--rw-r--r--   0 runner    (1001) docker     (123)     1585 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/cli/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6983 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/cli/delete.py
--rw-r--r--   0 runner    (1001) docker     (123)     5797 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/cli/get.py
--rw-r--r--   0 runner    (1001) docker     (123)     1781 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/cli/include.py
--rw-r--r--   0 runner    (1001) docker     (123)      898 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/cli/init.py
--rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/cli/tables.py
--rw-r--r--   0 runner    (1001) docker     (123)      363 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/constants.py
--rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/date.py
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/exc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/files.py
--rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/include.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/housekeeper/store/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/housekeeper/store/api/
--rw-r--r--   0 runner    (1001) docker     (123)      109 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/api/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5862 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/api/add.py
--rw-r--r--   0 runner    (1001) docker     (123)      939 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/api/base.py
--rw-r--r--   0 runner    (1001) docker     (123)      954 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/api/core.py
--rw-r--r--   0 runner    (1001) docker     (123)     6389 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/api/find.py
--rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/api/schema.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/housekeeper/store/filters/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/filters/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/filters/bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/filters/file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/filters/file_tags_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      768 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/filters/tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/filters/version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/filters/version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     3144 2023-03-23 14:49:50.000000 housekeeper-4.0.1/housekeeper/store/models.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/housekeeper.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-03-23 14:49:58.000000 housekeeper-4.0.1/housekeeper.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-03-23 14:49:58.000000 housekeeper-4.0.1/housekeeper.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:49:58.000000 housekeeper-4.0.1/housekeeper.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-03-23 14:49:58.000000 housekeeper-4.0.1/housekeeper.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 14:49:58.000000 housekeeper-4.0.1/housekeeper.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-03-23 14:49:58.000000 housekeeper-4.0.1/housekeeper.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       12 2023-03-23 14:49:58.000000 housekeeper-4.0.1/housekeeper.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-03-23 14:49:50.000000 housekeeper-4.0.1/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       64 2023-03-23 14:49:50.000000 housekeeper-4.0.1/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)      117 2023-03-23 14:49:59.000000 housekeeper-4.0.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-03-23 14:49:50.000000 housekeeper-4.0.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/tests/cli/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/tests/cli/add/
--rw-r--r--   0 runner    (1001) docker     (123)      562 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/add/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     6030 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/add/test_cli_add_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/add/test_cli_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     3775 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/add/test_cli_add_tags.py
--rw-r--r--   0 runner    (1001) docker     (123)     7112 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/add/test_cli_add_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/tests/cli/delete/
--rw-r--r--   0 runner    (1001) docker     (123)     3193 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/delete/test_cli_delete_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     2109 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/delete/test_cli_delete_file.py
--rw-r--r--   0 runner    (1001) docker     (123)     2981 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/delete/test_cli_delete_files.py
--rw-r--r--   0 runner    (1001) docker     (123)      789 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/delete/test_cli_delete_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/tests/cli/get/
--rw-r--r--   0 runner    (1001) docker     (123)     5639 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/get/test_get_bundle.py
--rw-r--r--   0 runner    (1001) docker     (123)     6277 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/get/test_get_files.py
--rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/get/test_get_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     3522 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/get/test_get_version.py
--rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/test_cli_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     9023 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/cli/test_cli_include.py
--rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/conftest.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/tests/fixtures/
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/tests/fixtures/vcfs/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/fixtures/vcfs/example.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/fixtures/vcfs/example.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/fixtures/vcfs/family.2.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/fixtures/vcfs/family.3.vcf
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/fixtures/vcfs/family.vcf
--rw-r--r--   0 runner    (1001) docker     (123)     2027 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/helper_functions.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 14:49:59.000000 housekeeper-4.0.1/tests/store/
--rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)     3622 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_add_core.py
--rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_add_file.py
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_add_schema.py
--rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_file_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_file_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)      908 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_find_tag.py
--rw-r--r--   0 runner    (1001) docker     (123)     2055 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_store_api.py
--rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_store_models.py
--rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_tag_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_version_bundle_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/store/test_version_filters.py
--rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/test_date.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-03-23 14:49:50.000000 housekeeper-4.0.1/tests/test_include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-21 14:00:36.000000 housekeeper-4.1.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      195 2023-04-21 14:00:36.000000 housekeeper-4.1.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-21 14:00:47.000000 housekeeper-4.1.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-21 14:00:36.000000 housekeeper-4.1.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      325 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/__main__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/archive/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)       47 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6148 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1608 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7096 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/delete.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5941 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/get.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1858 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/include.py
+-rw-r--r--   0 runner    (1001) docker     (123)      949 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/init.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6615 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/cli/tables.py
+-rw-r--r--   0 runner    (1001) docker     (123)      363 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/constants.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1727 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/date.py
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/exc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1388 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1968 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/include.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/store/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/store/api/
+-rw-r--r--   0 runner    (1001) docker     (123)      109 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6010 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/add.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1480 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6363 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/find.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3504 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/api/schema.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper/store/filters/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1109 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/file_tags_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      768 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/filters/version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3156 2023-04-21 14:00:36.000000 housekeeper-4.1.0/housekeeper/store/models.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4800 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2569 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       12 2023-04-21 14:00:47.000000 housekeeper-4.1.0/housekeeper.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 14:00:36.000000 housekeeper-4.1.0/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 14:00:36.000000 housekeeper-4.1.0/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      117 2023-04-21 14:00:47.000000 housekeeper-4.1.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3614 2023-04-21 14:00:36.000000 housekeeper-4.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/cli/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/cli/add/
+-rw-r--r--   0 runner    (1001) docker     (123)      562 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6214 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/test_cli_add_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3925 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/test_cli_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/test_cli_add_tags.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7216 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/add/test_cli_add_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2782 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/cli/delete/
+-rw-r--r--   0 runner    (1001) docker     (123)     3321 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/delete/test_cli_delete_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2284 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/delete/test_cli_delete_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3040 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/delete/test_cli_delete_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      789 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/delete/test_cli_delete_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/cli/get/
+-rw-r--r--   0 runner    (1001) docker     (123)     5750 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/get/test_get_bundle.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6357 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/get/test_get_files.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2705 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/get/test_get_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3631 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/get/test_get_version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4439 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/test_cli_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9231 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/cli/test_cli_include.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11490 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/fixtures/
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/26a90105b99c05381328317f913e9509e373b64f.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/fixtures/vcfs/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/example.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/example.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/family.2.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/family.3.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/fixtures/vcfs/family.vcf
+-rw-r--r--   0 runner    (1001) docker     (123)     2107 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/helper_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:00:47.000000 housekeeper-4.1.0/tests/store/
+-rw-r--r--   0 runner    (1001) docker     (123)     2373 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4024 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_add_core.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1683 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_add_file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_add_schema.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1701 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2485 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_file_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1488 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_file_tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)      908 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_find_tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2205 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_store_api.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1243 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_store_models.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2721 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_tag_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2225 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_version_bundle_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2305 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/store/test_version_filters.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2661 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/test_date.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-21 14:00:36.000000 housekeeper-4.1.0/tests/test_include.py
```

### Comparing `housekeeper-4.0.1/LICENSE` & `housekeeper-4.1.0/LICENSE`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/PKG-INFO` & `housekeeper-4.1.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.0.1
+Version: 4.1.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.0.1/README.md` & `housekeeper-4.1.0/README.md`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/cli/add.py` & `housekeeper-4.1.0/housekeeper/cli/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -62,27 +62,30 @@
         data["files"] = []
 
     try:
         new_bundle, new_version = store.add_bundle(data)
     except FileNotFoundError as err:
         LOG.warning("File %s does not exist", err)
         raise click.Abort
-    store.add_commit(new_bundle)
+    store.session.add(new_bundle)
     new_version.bundle: Bundle = new_bundle
-    store.add_commit(new_version)
+    store.session.add(new_version)
+    store.session.commit()
     LOG.info("new bundle added: %s (%s)", new_bundle.name, new_bundle.id)
 
 
 @add.command("file")
 @click.option("-t", "--tag", "tags", multiple=True, help="tag to associate the file by")
 @click.option("-b", "--bundle-name", help="name of bundle that file should be added to")
 @click.option("-j", "--json", help="json formatted input")
 @click.argument("path", required=False)
 @click.pass_context
-def file_cmd(context: click.Context, tags: List[str], bundle_name: str, json: str, path: str):
+def file_cmd(
+    context: click.Context, tags: List[str], bundle_name: str, json: str, path: str
+):
     """Add a file to the latest version of a bundle."""
     LOG.info("Running add file")
     store: Store = context.obj["store"]
     validate_args(arg=path, json=json, arg_name="path")
 
     data: Dict = {}
     if json:
@@ -100,27 +103,28 @@
     if bundle is None:
         LOG.warning("unknown bundle: %s", bundle_name)
         raise click.Abort
 
     tags = data.get("tags", tags)
 
     new_file = store.add_file(file_path=file_path, bundle=bundle, tags=tags)
-    store.add_commit(new_file)
+    store.session.add(new_file)
+    store.session.commit()
     LOG.info("new file added: %s (%s)", new_file.path, new_file.id)
 
 
 @add.command("version")
 @click.option("-j", "--json", help="Input in json format")
 @click.option("--created-at", help="Date when created")
 @click.argument("bundle_name", required=False)
 @click.pass_context
 def version_cmd(context: click.Context, bundle_name: str, created_at: str, json: str):
     """Add a new version to a bundle."""
     LOG.info("Running add version")
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
 
     validate_args(arg=bundle_name, json=json, arg_name="bundle_name")
 
     data: Dict = {"bundle_name": bundle_name, "created_at": created_at}
     if json:
         data: Dict = load_json(json)
         bundle_name = data["bundle_name"]
@@ -136,15 +140,16 @@
     data["created_at"] = get_date(data.get("created_at"))
     new_version = store.add_version(data, bundle)
 
     if not new_version:
         LOG.warning("Seems like version already exists for the bundle")
         raise click.Abort
 
-    store.add_commit(new_version)
+    store.session.add(new_version)
+    store.session.commit()
     LOG.info("new version (%s) added to bundle %s", new_version.id, bundle.name)
 
 
 @add.command("tag")
 @click.argument("tags", nargs=-1)
 @click.option("-f", "--file-id", type=int)
 @click.pass_context
@@ -167,25 +172,26 @@
     tag_name: str
     for tag_name in tags:
         tag: Tag = store.get_tag(tag_name)
 
         if not tag:
             LOG.info("%s: tag created", tag_name)
             tag: Tag = store.new_tag(tag_name)
-            store.add_commit(tag)
+            store.session.add(tag)
+            store.session.commit()
 
         if not file:
             continue
 
         if tag in file.tags:
             LOG.info("%s: tag already added", tag_name)
             continue
 
         file.tags.append(tag)
 
-    store.commit()
+    store.session.commit()
 
     if not file:
         return
 
     all_tags: Generator = (tag.name for tag in file.tags)
     LOG.info("file tags: %s", ", ".join(all_tags))
```

### Comparing `housekeeper-4.0.1/housekeeper/cli/core.py` & `housekeeper-4.1.0/housekeeper/cli/core.py`

 * *Files 18% similar despite different names*

```diff
@@ -17,15 +17,21 @@
 @click.group()
 @click.option("-c", "--config", type=click.File())
 @click.option("-d", "--database", help="path/URI of the SQL database")
 @click.option("-r", "--root", type=click.Path(exists=True), help="Housekeeper root dir")
 @click.option("-l", "--log-level", default="INFO")
 @click.version_option(housekeeper.__version__, prog_name=housekeeper.__title__)
 @click.pass_context
-def base(context: click.Context, config: click.File, database: Optional[str], root: Optional[str], log_level: str):
+def base(
+    context: click.Context,
+    config: click.File,
+    database: Optional[str],
+    root: Optional[str],
+    log_level: str,
+):
     """Housekeeper - Access your files!"""
     coloredlogs.install(level=log_level)
     config_values = {}
     if config:
         config_values = yaml.full_load(config)
     context.obj = config_values
     db_path = database or context.obj.get("database")
```

### Comparing `housekeeper-4.0.1/housekeeper/cli/delete.py` & `housekeeper-4.1.0/housekeeper/cli/delete.py`

 * *Files 3% similar despite different names*

```diff
@@ -20,41 +20,41 @@
 
 @delete.command("bundle")
 @click.option("-y", "--yes", is_flag=True, help="skip checks")
 @click.argument("bundle_name")
 @click.pass_context
 def bundle_cmd(context, yes, bundle_name):
     """Delete a empty bundle, that is a bundle without versions."""
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
     bundle = store.get_bundle_by_name(bundle_name=bundle_name)
     if bundle is None:
         LOG.warning("bundle %s not found", bundle_name)
         raise click.Abort
 
     if bundle.versions:
         LOG.warning("Can not delete bundle, please remove all versions first")
         raise click.Abort
 
     question = f"Remove bundle {bundle.name} from database?"
     if not (yes or click.confirm(question)):
         raise click.Abort
 
-    bundle.delete()
-    store.commit()
+    store.session.delete(bundle)
+    store.session.commit()
     LOG.info("Bundle deleted: %s", bundle.name)
 
 
 @delete.command("version")
 @click.option("-b", "--bundle-name", help="Fetch all versions from a bundle")
 @click.option("-i", "--version-id", type=int, help="Fetch a specific version")
 @click.option("-y", "--yes", is_flag=True, help="skip checks")
 @click.pass_context
 def version_cmd(context, bundle_name, version_id, yes):
     """Delete a version from database"""
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
     if not (bundle_name or version_id):
         LOG.info("Please select a bundle or a version")
         raise click.Abort
 
     if bundle_name:
         bundle = store.get_bundle_by_name(bundle_name=bundle_name)
         if not bundle:
@@ -85,16 +85,16 @@
 
     if not (yes or click.confirm(question)):
         raise click.Abort
 
     if version_obj.included_at:
         shutil.rmtree(version_obj.full_path, ignore_errors=True)
 
-    version_obj.delete()
-    store.commit()
+    store.session.delete(version_obj)
+    store.session.commit()
     LOG.info("version deleted: %s", version_obj.full_path)
 
 
 @delete.command("files")
 @click.option("--yes", is_flag=True, help="skip checks")
 @click.option("-t", "--tag", multiple=True, help="file tag")
 @click.option("-b", "--bundle-name", help="bundle name")
@@ -112,15 +112,15 @@
 def files_cmd(
     context, yes, tag, bundle_name, before, notondisk, list_files, list_files_verbose
 ):
     """Delete files based on tags."""
 
     validate_delete_options(tag=tag, bundle_name=bundle_name)
     before_date = parse_date(before) if before else None
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
 
     if bundle_name:
         validate_bundle_exists(store=store, bundle_name=bundle_name)
 
     files = store.get_files_before(
         bundle_name=bundle_name, tag_names=tag, before_date=before_date
     )
@@ -179,16 +179,17 @@
         click.echo(file.full_path)
 
 
 def delete_file(file: File, store: Store):
     file_path = Path(file.full_path)
     if file_should_be_unlinked(file):
         file_path.unlink()
-    file.delete()
-    store.commit()
+
+    store.session.delete(file)
+    store.session.commit()
     LOG.info(f"{file.full_path} deleted")
 
 
 def file_should_be_unlinked(file: File):
     """Check if file should be unlinked."""
     file_path = Path(file.full_path)
     return file.is_included and (file_path.exists() or file_path.is_symlink())
@@ -204,25 +205,25 @@
 
 @delete.command("file")
 @click.option("-y", "--yes", is_flag=True, help="skip checks")
 @click.argument("file_id", type=int)
 @click.pass_context
 def file_cmd(context, yes, file_id):
     """Delete a file."""
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
     file = store.get_file_by_id(file_id=file_id)
     if not file:
         LOG.info("file not found")
         raise click.Abort
 
     if file.is_included:
         question = f"remove file from file system and database: {file.full_path}"
     else:
         question = f"remove file from database: {file.full_path}"
 
     if yes or click.confirm(question):
         if file.is_included and Path(file.full_path).exists():
             Path(file.full_path).unlink()
 
-        file.delete()
-        store.commit()
+        store.session.delete(file)
+        store.session.commit()
         LOG.info("file deleted")
```

### Comparing `housekeeper-4.0.1/housekeeper/cli/get.py` & `housekeeper-4.1.0/housekeeper/cli/get.py`

 * *Files 3% similar despite different names*

```diff
@@ -3,14 +3,16 @@
 import logging
 from typing import List
 
 import click
 from rich.console import Console
 
 from housekeeper.store.api import schema
+from housekeeper.store.api.core import Store
+from housekeeper.store.models import Version
 
 from .tables import (
     get_bundles_table,
     get_files_table,
     get_tags_table,
     get_versions_table,
 )
@@ -33,15 +35,15 @@
     "--compact",
     is_flag=True,
     help="print compact filenames IFF verobe flag present",
 )
 @click.pass_context
 def bundle_cmd(context, bundle_name, bundle_id, json, verbose, compact):
     """Get bundle information from database"""
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
     bundles = store.bundles()
 
     if bundle_name:
         bundle = store.get_bundle_by_name(bundle_name=bundle_name)
         bundles = [bundle] if bundle else []
 
     if bundle_id:
@@ -82,27 +84,27 @@
     "--compact",
     is_flag=True,
     help="print compact filenames IFF verobe flag present",
 )
 @click.pass_context
 def version_cmd(context, bundle_name, json, version_id, verbose, compact):
     """Get versions from database"""
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
     if not (bundle_name or version_id):
         LOG.info("Please select a bundle or a version")
         return
     if bundle_name:
         bundle = store.get_bundle_by_name(bundle_name=bundle_name)
         if not bundle:
             LOG.info("Could not find bundle %s", bundle_name)
             return
         version_objs = bundle.versions
 
     if version_id:
-        version = store.Version.get(version_id)
+        version: Version = store.get_version_by_id(version_id=version_id)
         if not version:
             LOG.warning("Could not find version %s", version_id)
             raise click.Abort
         version_objs = [version]
 
     version_template = schema.VersionSchema()
     result = []
@@ -143,15 +145,15 @@
     version_id: int,
     verbose: bool,
     bundle: str,
     json: bool,
     compact: bool,
 ):
     """Get files from database"""
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
     file_objs = store.get_files(
         bundle_name=bundle, tag_names=tag_names, version_id=version_id
     )
     template = schema.FileSchema()
     result = []
     for file in file_objs:
         result.append(template.dump(file))
@@ -164,15 +166,15 @@
 
 @get.command("tag")
 @click.option("-j", "--json", is_flag=True, help="Output to json format")
 @click.option("-n", "--name", multiple=True, help="Specify a tag name")
 @click.pass_context
 def tag_cmd(context, json, name):
     """Get the tags from database"""
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
     LOG.info("Fetch tags")
     tag_objs = store.get_tags()
     template = schema.TagSchema()
     result = []
     for tag_obj in tag_objs:
         if name and (tag_obj.name not in name):
             continue
```

### Comparing `housekeeper-4.0.1/housekeeper/cli/include.py` & `housekeeper-4.1.0/housekeeper/cli/include.py`

 * *Files 9% similar despite different names*

```diff
@@ -2,36 +2,37 @@
 import datetime as dt
 import logging
 
 import click
 
 from housekeeper.exc import VersionIncludedError
 from housekeeper.include import include_version
+from housekeeper.store.api.core import Store
 
 LOG = logging.getLogger(__name__)
 
 
 @click.command()
 @click.option("--version-id", type=int, help="version id of the bundle version")
 @click.argument("bundle_name", required=False)
 @click.pass_context
 def include(context: click.Context, bundle_name: str, version_id: int):
     """Include a bundle of files into the internal space.
 
     Use bundle name if you simply want to include the latest version.
     """
     LOG.info("Running include")
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
     if not (version_id or bundle_name):
         LOG.warning("Please use bundle name or version-id")
         raise click.Abort
 
     if version_id:
         LOG.info("Use version %s", version_id)
-        version_obj = store.Version.get(version_id)
+        version_obj = store.get_version_by_id(version_id=version_id)
         if version_obj is None:
             LOG.warning("version not found")
             raise click.Abort
 
     if bundle_name:
         bundle = store.get_bundle_by_name(bundle_name=bundle_name)
         if bundle is None:
@@ -48,9 +49,9 @@
     try:
         include_version(context.obj["root"], version_obj)
     except VersionIncludedError as error:
         LOG.warning(error.message)
         raise click.Abort
 
     version_obj.included_at = dt.datetime.now()
-    store.commit()
+    store.session.commit()
     click.echo(click.style("included all files!", fg="green"))
```

### Comparing `housekeeper-4.0.1/housekeeper/cli/init.py` & `housekeeper-4.1.0/housekeeper/cli/init.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,22 +1,22 @@
 """Initialise HK db from CLI"""
 import logging
-
 import click
+from housekeeper.store.api.core import Store
 
 LOG = logging.getLogger(__name__)
 
 
 @click.command()
 @click.option("--reset", is_flag=True, help="reset database before setting up tables")
 @click.option("--force", is_flag=True, help="bypass manual confirmations")
 @click.pass_context
 def init(context, reset, force):
     """Setup the database."""
-    store = context.obj["store"]
+    store: Store = context.obj["store"]
     existing_tables = store.engine.table_names()
     if force or reset:
         if existing_tables and not force:
             message = f"Delete existing tables? [{', '.join(existing_tables)}]"
             click.confirm(click.style(message, fg="yellow"), abort=True)
         store.drop_all()
     elif existing_tables:
```

### Comparing `housekeeper-4.0.1/housekeeper/cli/tables.py` & `housekeeper-4.1.0/housekeeper/cli/tables.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/date.py` & `housekeeper-4.1.0/housekeeper/date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/files.py` & `housekeeper-4.1.0/housekeeper/files.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/include.py` & `housekeeper-4.1.0/housekeeper/include.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/store/api/add.py` & `housekeeper-4.1.0/housekeeper/store/api/add.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,29 +1,32 @@
 """This module handles adding things to the store"""
 
 import datetime as dt
 import logging
 from pathlib import Path
 from typing import Dict, List, Tuple
+from sqlalchemy.orm import Session
 
 from housekeeper.store import models
 from housekeeper.store.api.base import BaseHandler
 from housekeeper.store.api.find import FindHandler
 
 LOG = logging.getLogger(__name__)
 
 
 class AddHandler(BaseHandler):
     """Handles adding things to the store"""
 
-    def __init__(self):
-        super().__init__()
-        AddHandler.version = FindHandler.version
+    def __init__(self, session: Session):
+        super().__init__(session=session)
         AddHandler.get_bundle_by_name = FindHandler.get_bundle_by_name
         AddHandler.get_tag = FindHandler.get_tag
+        AddHandler.get_version_by_date_and_bundle_name = (
+            FindHandler.get_version_by_date_and_bundle_name
+        )
 
     def new_bundle(self, name: str, created_at: dt.datetime = None) -> models.Bundle:
         """Create a new file bundle."""
         new_bundle = self.Bundle(name=name, created_at=created_at)
         LOG.info("Created new bundle: %s", new_bundle.name)
         return new_bundle
```

### Comparing `housekeeper-4.0.1/housekeeper/store/api/find.py` & `housekeeper-4.1.0/housekeeper/store/api/find.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,15 @@
 """
 This module handles finding things in the store/database
 """
 import datetime as dt
 import logging
 from pathlib import Path
-from typing import List, Optional, Set
-
-from sqlalchemy.orm import Query
+from typing import List
+from sqlalchemy.orm import Query, Session
 
 from housekeeper.store.filters.bundle_filters import BundleFilters, apply_bundle_filter
 from housekeeper.store.filters.file_filters import FileFilter, apply_file_filter
 from housekeeper.store.filters.file_tags_filters import (
     FileTagFilter,
     apply_file_tag_filter,
 )
@@ -29,14 +28,17 @@
 
 LOG = logging.getLogger(__name__)
 
 
 class FindHandler(BaseHandler):
     """Handler for searching the database"""
 
+    def __init__(self, session: Session):
+        super().__init__(session=session)
+
     def bundles(self):
         """Fetch bundles."""
         LOG.info("Fetching all bundles")
         return self._get_query(table=Bundle)
 
     def get_bundle_by_id(self, bundle_id: int) -> Bundle:
         """Fetch a bundle by id from the store."""
@@ -85,18 +87,14 @@
         ).first()
 
     def get_tags(self) -> Query:
         """Return all tags from the database."""
         LOG.info("Fetching all tags")
         return self._get_query(table=Tag)
 
-    def _get_tag_query(self) -> Query:
-        """Return a tag query."""
-        return self.Tag.query
-
     def get_file_by_id(self, file_id: int):
         """Get a file by record id."""
         return apply_file_filter(
             files=self._get_query(table=File),
             filter_functions=[FileFilter.FILTER_BY_ID],
             file_id=file_id,
         ).first()
```

### Comparing `housekeeper-4.0.1/housekeeper/store/api/schema.py` & `housekeeper-4.1.0/housekeeper/store/api/schema.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/store/filters/bundle_filters.py` & `housekeeper-4.1.0/housekeeper/store/filters/bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/store/filters/file_filters.py` & `housekeeper-4.1.0/housekeeper/store/filters/file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/store/filters/file_tags_filters.py` & `housekeeper-4.1.0/housekeeper/store/filters/file_tags_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/store/filters/tag_filters.py` & `housekeeper-4.1.0/housekeeper/store/filters/tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/store/filters/version_bundle_filters.py` & `housekeeper-4.1.0/housekeeper/store/filters/version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/store/filters/version_filters.py` & `housekeeper-4.1.0/housekeeper/store/filters/version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/housekeeper/store/models.py` & `housekeeper-4.1.0/housekeeper/store/models.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 """Module for the models"""
 
 import datetime as dt
 from pathlib import Path
 
-import alchy
+from sqlalchemy.ext.declarative import declarative_base
 from sqlalchemy import Column, ForeignKey, Table, UniqueConstraint, orm, types
 
-Model = alchy.make_declarative_base(Base=alchy.ModelBase)
+Model = declarative_base()
 
 
 file_tag_link = Table(
     "file_tag_link",
     Model.metadata,
     Column("file_id", types.Integer, ForeignKey("file.id"), nullable=False),
     Column("tag_id", types.Integer, ForeignKey("tag.id"), nullable=False),
```

### Comparing `housekeeper-4.0.1/housekeeper.egg-info/PKG-INFO` & `housekeeper-4.1.0/housekeeper.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: housekeeper
-Version: 4.0.1
+Version: 4.1.0
 Summary: Housekeeper takes care of files
 Home-page: https://github.com/Clinical-Genomics/housekeeper
 Author: Robin Andeer
 Author-email: mans.magnusson@scilifelab.se
 License: MIT
 Description: 
         # Housekeeper
```

### Comparing `housekeeper-4.0.1/housekeeper.egg-info/SOURCES.txt` & `housekeeper-4.1.0/housekeeper.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/setup.py` & `housekeeper-4.1.0/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -43,15 +43,15 @@
 
 
 setup(
     name=NAME,
     # Versions should comply with PEP440. For a discussion on
     # single-sourcing the version across setup.py and the project code,
     # see http://packaging.python.org/en/latest/tutorial.html#version
-    version="4.0.1",
+    version="4.1.0",
     description=DESCRIPTION,
     long_description=LONG_DESCRIPTION,
     long_description_content_type="text/markdown",
     # What does your project relate to? Separate with spaces.
     keywords="housekeeper development",
     author=AUTHOR,
     author_email=EMAIL,
```

### Comparing `housekeeper-4.0.1/tests/cli/add/conftest.py` & `housekeeper-4.1.0/tests/cli/add/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/cli/add/test_cli_add_bundle.py` & `housekeeper-4.1.0/tests/cli/add/test_cli_add_bundle.py`

 * *Files 2% similar despite different names*

```diff
@@ -2,36 +2,40 @@
 import json
 import logging
 
 from click import Context
 from click.testing import CliRunner
 
 from housekeeper.cli.add import bundle_cmd
+from housekeeper.store.api.core import Store
+from housekeeper.store.models import Bundle
 
 
 def test_add_existing_bundle(populated_context: Context, cli_runner: CliRunner, caplog):
     """Test to add a bundle that exists"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a existing bundle
-    bundle_obj = store.Bundle.query.first()
+    bundle_obj = store._get_query(table=Bundle).first()
     assert bundle_obj
     bundle_name = bundle_obj.name
 
     # WHEN trying to add a bundle that exists
     result = cli_runner.invoke(bundle_cmd, [bundle_name], obj=populated_context)
 
     # THEN assert it has a non zero exit status
     assert result.exit_code == 1
     # THEN check that the error message is displayed
     assert "already exists" in caplog.text
 
 
-def test_add_simple_bundle(base_context: Context, cli_runner: CliRunner, case_id: str, caplog):
+def test_add_simple_bundle(
+    base_context: Context, cli_runner: CliRunner, case_id: str, caplog
+):
     """Test to add a new bundle by only specifying bundle name"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a empty store and a cli runner
     bundle_name = case_id
 
     # WHEN trying to add a bundle with only the bundle name
     result = cli_runner.invoke(bundle_cmd, [bundle_name], obj=base_context)
@@ -66,30 +70,34 @@
     """Test to add a new bundle using json AND bundle_name as input.
 
     This test should fail since it will be confusing to provide inconsistent information
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a empty store, a cli runner and a bundle in json format
     # WHEN trying to add a bundle with both json and bundle_name as input
-    result = cli_runner.invoke(bundle_cmd, [case_id, "--json", bundle_data_json], obj=base_context)
+    result = cli_runner.invoke(
+        bundle_cmd, [case_id, "--json", bundle_data_json], obj=base_context
+    )
 
     # THEN assert the call failed
     assert result.exit_code == 1
     # THEN check that the proper information is displayed
     assert "not input both json and bundle_name" in caplog.text
 
 
 def test_add_bundle_json(
     base_context: Context, cli_runner: CliRunner, bundle_data_json: str, caplog
 ):
     """Test to add a new bundle using json as input"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a empty store, a cli runner and a bundle in json format
     # WHEN trying to add a bundle
-    result = cli_runner.invoke(bundle_cmd, ["--json", bundle_data_json], obj=base_context)
+    result = cli_runner.invoke(
+        bundle_cmd, ["--json", bundle_data_json], obj=base_context
+    )
 
     # THEN assert it succeded
     assert result.exit_code == 0
     # THEN check that the proper information is displayed
     assert "new bundle added" in caplog.text
 
 
@@ -102,15 +110,17 @@
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a empty store, a cli runner and a bundle in json format without files
     bundle_data = json.loads(bundle_data_json)
     bundle_data.pop("files")
     bundle_data_json = json.dumps(bundle_data)
 
     # WHEN trying to add a bundle
-    result = cli_runner.invoke(bundle_cmd, ["--json", bundle_data_json], obj=base_context)
+    result = cli_runner.invoke(
+        bundle_cmd, ["--json", bundle_data_json], obj=base_context
+    )
 
     # THEN assert it succeded
     assert result.exit_code == 0
     # THEN check that the proper information is displayed even if there where no files added
     assert "new bundle added" in caplog.text
 
 
@@ -126,15 +136,17 @@
     # existing files
     non_existing = "a_non_existing_file.txt"
     bundle_data = json.loads(bundle_data_json)
     bundle_data["files"][0]["path"] = non_existing
     bundle_data_json = json.dumps(bundle_data)
 
     # WHEN trying to add a bundle
-    result = cli_runner.invoke(bundle_cmd, ["--json", bundle_data_json], obj=base_context)
+    result = cli_runner.invoke(
+        bundle_cmd, ["--json", bundle_data_json], obj=base_context
+    )
 
     # THEN assert it succeded
     assert result.exit_code == 1
     # THEN check that the proper information is displayed
     assert f"File {non_existing} does not exist" in caplog.text
 
 
@@ -147,13 +159,15 @@
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a empty store, a cli runner and a bundle in json format without files
     bundle_data = json.loads(bundle_data_json)
     bundle_data.pop("created_at")
     bundle_data_json = json.dumps(bundle_data)
 
     # WHEN trying to add a bundle
-    result = cli_runner.invoke(bundle_cmd, ["--json", bundle_data_json], obj=base_context)
+    result = cli_runner.invoke(
+        bundle_cmd, ["--json", bundle_data_json], obj=base_context
+    )
 
     # THEN assert it succeded
     assert result.exit_code == 1
     # THEN check that the proper information is displayed even if there where no files added
     assert "Bundle date is required" in caplog.text
```

### Comparing `housekeeper-4.0.1/tests/cli/add/test_cli_add_file.py` & `housekeeper-4.1.0/tests/cli/add/test_cli_add_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/cli/add/test_cli_add_tags.py` & `housekeeper-4.1.0/tests/cli/add/test_cli_add_tags.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,11 +1,13 @@
 """Tests for adding tags via CLI"""
 import logging
 
 from housekeeper.cli.add import tag_cmd
+from housekeeper.store.api.core import Store
+from housekeeper.store.models import File
 
 
 def test_add_tags_no_args(populated_context, cli_runner, caplog):
     """Test to add a two tags to the database"""
     # GIVEN a context with a populated store, and a cli runner
     caplog.set_level(logging.DEBUG)
     # GIVEN that there is no tag input
@@ -39,57 +41,61 @@
     assert db_tags.intersection(set([tag1, tag2]))
 
 
 def test_add_existing_tag_existing_file(populated_context, cli_runner, caplog):
     """Test to add a existing tag to a file that exists"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store, and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a existing file id
     file_id = 1
-    file_obj = store.File.get(file_id)
+    file_obj: File = store.get_file_by_id(file_id=file_id)
     # GIVEN that the new tag already exists for the file
     tag = file_obj.tags[0].name
 
     # WHEN trying to add the existing tag to the file
-    result = cli_runner.invoke(tag_cmd, [tag, "-f", str(file_id)], obj=populated_context)
+    result = cli_runner.invoke(
+        tag_cmd, [tag, "-f", str(file_id)], obj=populated_context
+    )
     # THEN assert it has a non zero exit status
     assert result.exit_code == 0
     # THEN check that it communicates that the tag existed
     assert f"{tag}: tag already added" in caplog.text
 
 
 def test_add_tag_existing_file(populated_context, cli_runner, caplog):
     """Test to add a non existing tag to a file that exists"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store, and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a existing file id
     file_id = 1
-    file_obj = store.File.get(file_id)
+    file_obj: File = store.get_file_by_id(file_id=file_id)
     assert file_obj
     # GIVEN a new tag
     tag = "new-tag"
 
     # WHEN trying to add a tag to the existing file
-    result = cli_runner.invoke(tag_cmd, [tag, "-f", str(file_id)], obj=populated_context)
+    result = cli_runner.invoke(
+        tag_cmd, [tag, "-f", str(file_id)], obj=populated_context
+    )
     # THEN assert it has a zero exit status
     assert result.exit_code == 0
     # THEN check that the tag is displayed in the output
     assert f"{tag}: tag created" in caplog.text
 
 
 def test_add_tag_non_existing_file(populated_context, cli_runner, caplog):
     """Test to add a tag to a file that not exist"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a non existing file id
     missing_file_id = 42
-    file_obj = store.File.get(missing_file_id)
+    file_obj = store.get_file_by_id(file_id=missing_file_id)
     assert not file_obj
 
     # WHEN trying to add a tag to the non existing file
     result = cli_runner.invoke(
         tag_cmd, ["new-tag", "-f", str(missing_file_id)], obj=populated_context
     )
     # THEN assert it has a non zero exit status
```

### Comparing `housekeeper-4.0.1/tests/cli/add/test_cli_add_version.py` & `housekeeper-4.1.0/tests/cli/add/test_cli_add_version.py`

 * *Files 8% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import json
 import logging
 
 from click import Context
 from click.testing import CliRunner
 
 from housekeeper.cli.add import version_cmd
+from housekeeper.store.api.core import Store
 from housekeeper.store.models import Bundle
 
 
 def test_add_version_non_input(
     populated_context: Context, cli_runner: CliRunner, caplog
 ):
     """Test to add a version to a bundle without providing input
@@ -33,15 +34,15 @@
 ):
     """Test to add a version to a non existing bundle
 
     The CLI should exit with non zero since the bundle does not exist
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a non existing bundle
     bundle_name = "non_existing"
     bundle: Bundle = store.get_bundle_by_name(bundle_name=bundle_name)
     assert not bundle
 
     # WHEN trying to add a version to a non existing bundle
     result = cli_runner.invoke(version_cmd, [bundle_name], obj=populated_context)
@@ -57,17 +58,17 @@
 ):
     """Test to add a version to a existing bundle
 
     The functionality should work as expected since the bundle exists
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a existing bundle
-    bundle: Bundle = store.Bundle.query.first()
+    bundle: Bundle = store._get_query(table=Bundle).first()
     assert isinstance(bundle, Bundle)
 
     # GIVEN the name of a existing bundle
     bundle_name: str = bundle.name
 
     # WHEN trying to add a version to an existing bundle
     result = cli_runner.invoke(version_cmd, [bundle_name], obj=populated_context)
@@ -84,17 +85,17 @@
 ):
     """Test to add a version to an existing bundle when the date is the same
 
     It should not be possible to add two versions with the same dates
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a existing bundle
-    bundle: Bundle = store.Bundle.query.first()
+    bundle: Bundle = store._get_query(table=Bundle).first()
     assert isinstance(bundle, Bundle)
     bundle_name: str = bundle.name
 
     # WHEN trying to add a version to an existing bundle
     result = cli_runner.invoke(
         version_cmd,
         [bundle_name, "--created-at", timestamp_string],
@@ -115,15 +116,15 @@
 ):
     """Test to add a new empty version to existing bundle using json as input
 
     This should work since there is no problem to add a version without files
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     version_data = json.loads(empty_version_data_json)
     # GIVEN a bundle with one version
     bundle = store.get_bundle_by_name(bundle_name=version_data["bundle_name"])
     assert isinstance(bundle, Bundle)
     assert len(bundle.versions) == 1
     # GIVEN version information without files, in json format
     assert version_data["files"] == []
@@ -145,15 +146,15 @@
 
 def test_add_version_with_files_json(
     populated_context: Context, cli_runner: CliRunner, version_data_json: str, caplog
 ):
     """Test to add a new version with files to existing bundle using json as input"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     version_data = json.loads(version_data_json)
     # GIVEN a bundle with one version
     bundle = store.get_bundle_by_name(bundle_name=version_data["bundle_name"])
     assert isinstance(bundle, Bundle)
     assert len(bundle.versions) == 1
     # GIVEN version information without files, in json format
     assert version_data["files"] != []
```

### Comparing `housekeeper-4.0.1/tests/cli/conftest.py` & `housekeeper-4.1.0/tests/cli/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/cli/delete/test_cli_delete_bundle.py` & `housekeeper-4.1.0/tests/cli/delete/test_cli_delete_bundle.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Tests for delete CLI functions"""
 import logging
 from click import Context
 from click.testing import CliRunner
 
 from housekeeper.cli import delete
+from housekeeper.store.api.core import Store
 
 
-def test_delete_non_existing_bundle(base_context: Context, cli_runner: CliRunner, caplog):
+def test_delete_non_existing_bundle(
+    base_context: Context, cli_runner: CliRunner, caplog
+):
     """Test to delete a non existing bundle"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a store and a cli runner
     # GIVEN a case name that does not exist
     case_name = "hello"
     assert not base_context["store"].get_bundle_by_name(bundle_name=case_name)
 
@@ -25,15 +28,15 @@
 
 def test_delete_existing_bundle_with_version(
     populated_context: Context, cli_runner: CliRunner, case_id: str, caplog
 ):
     """Test to delete an existing bundle with versions"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a bundle with versions
     bundle_obj = store.get_bundle_by_name(bundle_name=case_id)
     assert len(bundle_obj.versions) > 0
 
     # WHEN trying to delete a bundle
     result = cli_runner.invoke(delete.bundle_cmd, [case_id], obj=populated_context)
 
@@ -43,37 +46,45 @@
 
 def test_delete_existing_bundle_no_versions_no_confirmation(
     populated_context: Context, cli_runner: CliRunner, case_id: str, caplog
 ):
     """Test to delete an existing bundle without confirmation"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a bundle without versions
-    cli_runner.invoke(delete.version_cmd, ["-b", case_id], obj=populated_context, input="Yes")
+    cli_runner.invoke(
+        delete.version_cmd, ["-b", case_id], obj=populated_context, input="Yes"
+    )
     bundle_obj = store.get_bundle_by_name(bundle_name=case_id)
     assert len(bundle_obj.versions) == 0
 
     # WHEN trying to delete a bundle
-    result = cli_runner.invoke(delete.bundle_cmd, [case_id], obj=populated_context, input="no")
+    result = cli_runner.invoke(
+        delete.bundle_cmd, [case_id], obj=populated_context, input="no"
+    )
     # THEN assert it exits non zero
     assert result.exit_code == 1
 
 
 def test_delete_existing_bundle_no_versions_with_confirmation(
     populated_context: Context, cli_runner: CliRunner, case_id: str, caplog
 ):
     """Test to delete an existing bundle without confirmation"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a bundle without versions
-    cli_runner.invoke(delete.version_cmd, ["-b", case_id], obj=populated_context, input="Yes")
+    cli_runner.invoke(
+        delete.version_cmd, ["-b", case_id], obj=populated_context, input="Yes"
+    )
     bundle_obj = store.get_bundle_by_name(bundle_name=case_id)
     assert len(bundle_obj.versions) == 0
 
     # WHEN trying to delete a bundle
-    result = cli_runner.invoke(delete.bundle_cmd, [case_id], obj=populated_context, input="Yes")
+    result = cli_runner.invoke(
+        delete.bundle_cmd, [case_id], obj=populated_context, input="Yes"
+    )
     # THEN assert it exits non zero
     assert result.exit_code == 0
     # THEN it should communicate that it was deleted
     assert "Bundle deleted" in caplog.text
```

### Comparing `housekeeper-4.0.1/tests/cli/delete/test_cli_delete_file.py` & `housekeeper-4.1.0/tests/cli/delete/test_cli_delete_file.py`

 * *Files 9% similar despite different names*

```diff
@@ -1,24 +1,26 @@
 """Tests for delete CLI functions"""
 
 import logging
 from click import Context
 from click.testing import CliRunner
 
 from housekeeper.cli import delete
+from housekeeper.store.api.core import Store
+from housekeeper.store.models import File
 
 
 def test_delete_non_existing_file(base_context: Context, cli_runner: CliRunner, caplog):
     """Test to delete a non existing file"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a store, a file id and a cli runner
     file_id = 1
     # GIVEN that the file does not exist
     store = base_context["store"]
-    file_obj = store.File.get(file_id)
+    file_obj: File = store.get_file_by_id(file_id=file_id)
     assert not file_obj
 
     # WHEN trying to delete the non existing file
     result = cli_runner.invoke(delete.file_cmd, [str(file_id)], obj=base_context)
 
     # THEN assert it exits non zero
     assert result.exit_code == 1
@@ -27,18 +29,18 @@
 
 
 def test_delete_existing_file_with_confirmation(
     populated_context: Context, cli_runner: CliRunner, caplog
 ):
     """Test to delete an existing file using confirmation"""
     # GIVEN a context with a populated store, a file id and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     file_id = 1
     # GIVEN that the file exists
-    file_obj = store.File.get(file_id)
+    file_obj: File = store.get_file_by_id(file_id=file_id)
     assert file_obj
 
     # WHEN trying to delete the file
     result = cli_runner.invoke(delete.file_cmd, [str(file_id)], obj=populated_context)
 
     # THEN it should ask if you are sure
     assert "remove file from" in result.output
@@ -46,18 +48,20 @@
 
 def test_delete_existing_file_no_confirmation(
     populated_context: Context, cli_runner: CliRunner, caplog
 ):
     """Test to delete a existing file without confirmation"""
     caplog.set_level(logging.DEBUG)
     # GIVEN a context with a populated store, a file id and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     file_id = 1
     # GIVEN that the file exists
-    file_obj = store.File.get(file_id)
+    file_obj: File = store.get_file_by_id(file_id=file_id)
     assert file_obj
 
     # WHEN trying to delete the file
-    result = cli_runner.invoke(delete.file_cmd, [str(file_id), "--yes"], obj=populated_context)
+    result = cli_runner.invoke(
+        delete.file_cmd, [str(file_id), "--yes"], obj=populated_context
+    )
 
     # THEN file delete should be in output
     assert "file deleted" in caplog.text
```

### Comparing `housekeeper-4.0.1/tests/cli/delete/test_cli_delete_files.py` & `housekeeper-4.1.0/tests/cli/delete/test_cli_delete_files.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,14 +1,15 @@
 """Tests for delete CLI functions"""
 
 import logging
 from click import Context
 from click.testing import CliRunner
 
 from housekeeper.cli import delete
+from housekeeper.store.api.core import Store
 from housekeeper.store.models import Bundle
 
 
 def test_delete_files_non_specified(
     base_context: Context, cli_runner: CliRunner, caplog
 ):
     """Test to delete files without specifying bundle name or tag"""
@@ -48,15 +49,15 @@
 def test_delete_existing_bundle_with_confirmation(
     populated_context: Context, cli_runner: CliRunner, case_id: str, caplog
 ):
     """Test to delete an existing bundle with confirmation"""
     caplog.set_level(logging.DEBUG)
 
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
 
     # GIVEN a existing bundle
     bundle: Bundle = store._get_query(table=Bundle).first()
     assert bundle
     case_id = bundle.name
 
     # WHEN trying to delete files without specifying bundle name or tag
@@ -71,15 +72,15 @@
 def test_delete_existing_bundle_no_confirmation(
     populated_context: Context, cli_runner: CliRunner, case_id: str, caplog
 ):
     """Test to delete an existing bundle without confirmation"""
     caplog.set_level(logging.DEBUG)
 
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
 
     # GIVEN a existing bundle
     bundle: Bundle = store._get_query(table=Bundle).first()
     assert bundle
 
     case_id = bundle.name
```

### Comparing `housekeeper-4.0.1/tests/cli/delete/test_cli_delete_version.py` & `housekeeper-4.1.0/tests/cli/delete/test_cli_delete_version.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/cli/get/test_get_bundle.py` & `housekeeper-4.1.0/tests/cli/get/test_get_bundle.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 """Tests for adding via CLI"""
 from housekeeper.cli.get import bundle_cmd
+from housekeeper.store.api.core import Store
 from housekeeper.store.models import Bundle
 
 
 def test_get_existing_bundle_name(populated_context, cli_runner, helpers):
     """Test to fetch an existing bundle based on name"""
 
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
 
     # GIVEN a existing bundle
     bundle: Bundle = store._get_query(table=Bundle).first()
     assert bundle
 
     bundle_name = bundle.name
 
@@ -24,15 +25,15 @@
     assert bundle_name in output
 
 
 def test_get_existing_bundle_verbose(populated_context, cli_runner, helpers):
     """Test to fetch an existing bundle based on name with verbose information"""
 
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
 
     # GIVEN a existing bundle
     bundle: Bundle = store._get_query(table=Bundle).first()
     assert bundle
     bundle_name = bundle.name
 
     # WHEN trying to fetch the bundle based on bundle name
@@ -62,15 +63,15 @@
 
 
 def test_get_non_existing_bundle_populated_store(
     populated_context, cli_runner, other_case_id, helpers
 ):
     """Test to fetch a non existing bundle based on name when bundles exists"""
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
 
     # GIVEN a non empty store
     assert helpers.count_iterable(store.bundles()) > 0
 
     # GIVEN a bundle name that does not exist in database
     assert store.get_bundle_by_name(bundle_name=other_case_id) is None
 
@@ -82,18 +83,18 @@
     # THEN assert that no bundle was written to terminal
     assert other_case_id not in output
 
 
 def test_get_existing_bundle_id(populated_context, cli_runner, helpers):
     """Test to fetch an existing bundle based on bundle id"""
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
 
     # GIVEN a existing bundle
-    bundle = store.Bundle.query.first()
+    bundle = store._get_query(table=Bundle).first()
     bundle_id = bundle.id
 
     # WHEN trying to fetch a bundle based on bundle id
     json_bundles = helpers.get_json(
         cli_runner.invoke(
             bundle_cmd, ["-i", bundle_id, "--json"], obj=populated_context
         ).output
@@ -104,18 +105,18 @@
     assert len(json_bundles) == 1
 
 
 def test_get_bundle_json(populated_context, cli_runner, helpers):
     """Test to fetch a bundle in json format"""
 
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
 
     # GIVEN a existing bundle
-    bundle = store.Bundle.query.first()
+    bundle = store._get_query(table=Bundle).first()
     bundle_id = bundle.id
 
     # WHEN fetching the bundle in json format
     json_bundles = helpers.get_json(
         cli_runner.invoke(
             bundle_cmd, ["-i", bundle_id, "--json"], obj=populated_context
         ).output
@@ -130,15 +131,15 @@
 
 def test_get_bundles_multiple_bundles(
     populated_context, cli_runner, helpers, other_bundle
 ):
     """Test to get all bundles when there are more than one bundle"""
 
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     helpers.add_bundle(store, other_bundle)
 
     # GIVEN a store with more than one bundles
     nr_bundles = helpers.count_iterable(store.bundles())
     assert nr_bundles > 1
 
     # WHEN fetching all bundles by not specifying any bundle
```

### Comparing `housekeeper-4.0.1/tests/cli/get/test_get_files.py` & `housekeeper-4.1.0/tests/cli/get/test_get_files.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,12 @@
 """Tests for cli get file functionality"""
 from pathlib import Path
 from housekeeper.cli.get import files_cmd
 from housekeeper.cli.tables import squash_names, _get_suffix
+from housekeeper.store.api.core import Store
 
 
 def test_get_files_no_files(base_context, cli_runner, helpers):
     """Test to get all files when there are no files"""
     # GIVEN a context with a populated store and a cli runner
     store = base_context["store"]
     # GIVEN a store without files
@@ -21,15 +22,15 @@
     # THEN assert that no files where fetched
     assert len(json_bundles) == 0
 
 
 def test_get_files_json(populated_context, cli_runner, helpers):
     """Test to get all files from a populated store"""
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a store with some files
     nr_files = helpers.count_iterable(store.get_files())
     assert nr_files > 0
 
     # WHEN fetching all files by not specifying any file
     json_bundles = helpers.get_json(
         cli_runner.invoke(files_cmd, ["--json"], obj=populated_context).output
@@ -39,15 +40,15 @@
     assert len(json_bundles) == nr_files
 
 
 def test_get_files(populated_context, cli_runner):
     """Test to get all files from a populated store in human friendly format"""
     # GIVEN a context with a populated store and a cli runner
     # GIVEN a store with some files
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a file name
     file_obj = store.get_files().first()
     file_name = Path(file_obj.path).name
 
     # WHEN fetching all files by not specifying any file
     result = cli_runner.invoke(files_cmd, [], obj=populated_context)
 
@@ -56,15 +57,15 @@
     # THEN assert that the full file path is not shown
     assert file_obj.path not in result.output
 
 
 def test_get_files_tag(populated_context, cli_runner, helpers, vcf_tag_name):
     """Test to get files with a specific tag from a populated store"""
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a store with some files that are tagged
     nr_files = helpers.count_iterable(store.get_files(tag_names=[vcf_tag_name]))
     assert nr_files > 0
 
     # WHEN fetching all files by not specifying any file
     json_bundles = helpers.get_json(
         cli_runner.invoke(
@@ -77,15 +78,15 @@
 
 
 def test_get_files_multiple_tags(
     populated_context, cli_runner, helpers, vcf_tag_name, family_tag_name
 ):
     """Test to get files with multiple tags tag from a populated store"""
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a store with some files that are tagged
     nr_files = helpers.count_iterable(
         store.get_files(tag_names=[vcf_tag_name, family_tag_name])
     )
     assert nr_files > 0
 
     # WHEN fetching all files by not specifying any file
@@ -100,15 +101,15 @@
     # THEN assert that all files where fetched
     assert len(json_bundles) == nr_files
 
 
 def test_get_files_rare_tag(populated_context, cli_runner, helpers, family_tag_name):
     """Test to get files with a tag that is not on all files from a populated store"""
     # GIVEN a context with a populated store and a cli runner
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a store with some files that are tagged
     total_nr_files = helpers.count_iterable(store.get_files())
     nr_tag_files = helpers.count_iterable(store.get_files(tag_names=[family_tag_name]))
     # GIVEN a tag that only fetches a subset of the files
     assert nr_tag_files < total_nr_files
 
     # WHEN fetching all files with that tag
```

### Comparing `housekeeper-4.0.1/tests/cli/get/test_get_tag.py` & `housekeeper-4.1.0/tests/cli/get/test_get_tag.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/cli/get/test_get_version.py` & `housekeeper-4.1.0/tests/cli/get/test_get_version.py`

 * *Files 7% similar despite different names*

```diff
@@ -2,14 +2,15 @@
 import logging
 
 from datetime import datetime
 from click import Context
 from click.testing import CliRunner
 
 from housekeeper.cli.get import version_cmd
+from housekeeper.store.api.core import Store
 from housekeeper.store.models import Bundle, Version
 
 
 def test_get_version_no_input(
     populated_context: Context, cli_runner: CliRunner, caplog
 ):
     """Test to get all versions when no input is given
@@ -32,16 +33,16 @@
     populated_context: Context, cli_runner: CliRunner, helpers
 ):
     """Test to get all versions from a bundle by using the bundle name.
 
     This should return all versions
     """
     # GIVEN a context that is populated
-    store = populated_context["store"]
-    bundle_obj: Bundle = store.Bundle.query.first()
+    store: Store = populated_context["store"]
+    bundle_obj: Bundle = store._get_query(table=Bundle).first()
     version_obj: Version = bundle_obj.versions[0]
     bundle_name: str = bundle_obj.name
 
     # WHEN running the include files command
     result = cli_runner.invoke(version_cmd, ["-b", bundle_name], obj=populated_context)
 
     # THEN assert that the version path was created
@@ -52,15 +53,15 @@
     populated_context: Context, cli_runner: CliRunner, caplog
 ):
     """
     Test to get all versions from a bundle that does not exist
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context that is populated
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a non existing bundle name
     bundle_name = "hello"
     assert not store.get_bundle_by_name(bundle_name=bundle_name)
 
     # WHEN running the include files command
     cli_runner.invoke(version_cmd, ["-b", bundle_name], obj=populated_context)
 
@@ -70,16 +71,16 @@
 
 def test_get_version_json(populated_context: Context, cli_runner: CliRunner, helpers):
     """Test to get all versions from a bundle by using the bundle name in json format.
 
     This should return all versions
     """
     # GIVEN a context that is populated
-    store = populated_context["store"]
-    bundle_obj = store.Bundle.query.first()
+    store: Store = populated_context["store"]
+    bundle_obj = store._get_query(table=Bundle).first()
     bundle_name = bundle_obj.name
 
     # WHEN running the include files command
     result = cli_runner.invoke(
         version_cmd, ["-b", bundle_name, "--json"], obj=populated_context
     )
 
@@ -91,16 +92,16 @@
     populated_context: Context, cli_runner: CliRunner, helpers
 ):
     """Test to get all versions from a bundle by using the bundle name in json format.
 
     This should return all versions
     """
     # GIVEN a context that is populated
-    store = populated_context["store"]
-    bundle_obj: Bundle = store.Bundle.query.first()
+    store: Store = populated_context["store"]
+    bundle_obj: Bundle = store._get_query(table=Bundle).first()
     version_obj: Version = bundle_obj.versions[0]
     version_id: int = version_obj.id
 
     # WHEN running the include files command
     result = cli_runner.invoke(version_cmd, ["-i", version_id], obj=populated_context)
 
     # THEN assert that the program exits succesfully
```

### Comparing `housekeeper-4.0.1/tests/cli/test_cli_core.py` & `housekeeper-4.1.0/tests/cli/test_cli_core.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/cli/test_cli_include.py` & `housekeeper-4.1.0/tests/cli/test_cli_include.py`

 * *Files 6% similar despite different names*

```diff
@@ -2,27 +2,28 @@
 import logging
 from datetime import datetime
 from click import Context
 from click.testing import CliRunner
 
 from housekeeper.cli.include import include
 from housekeeper.cli.add import bundle_cmd
-from housekeeper.store.models import Bundle
+from housekeeper.store.api.core import Store
+from housekeeper.store.models import Bundle, Version
 
 
 def test_include_files_creates_bundle_dir(
     populated_context: Context, cli_runner: CliRunner
 ):
     """Test to include the files of a version for a bundle_name
 
     The bundle should not exist before and after command is run it should have been created
     """
     # GIVEN a context that is populated
-    store = populated_context["store"]
-    bundle: Bundle = store.Bundle.query.first()
+    store: Store = populated_context["store"]
+    bundle: Bundle = store._get_query(table=Bundle).first()
     bundle_name: str = bundle.name
     # GIVEN that the latest version of the bundle is not included
     assert bundle.versions[0].included_at is None
     # GIVEN that no folder has been created since case is not included
     bundle_path = populated_context["root"] / bundle.name
     assert not bundle_path.exists()
 
@@ -37,16 +38,16 @@
     populated_context: Context, cli_runner: CliRunner
 ):
     """Test to include the files of a version for a bundle_name
 
     The version bundle should not exist before and after command is run it should have been created
     """
     # GIVEN a context that is populated
-    store = populated_context["store"]
-    bundle: Bundle = store.Bundle.query.first()
+    store: Store = populated_context["store"]
+    bundle: Bundle = store._get_query(table=Bundle).first()
     version_obj = bundle.versions[0]
     bundle_name: str = bundle.name
     # GIVEN that the latest version of the bundle is not included
     assert version_obj.included_at is None
     # GIVEN that no version specific folder has been created since version is not included
     version_path = (
         populated_context["root"] / bundle.name / str(version_obj.created_at.date())
@@ -64,16 +65,16 @@
     populated_context: Context, cli_runner: CliRunner
 ):
     """Test to include the files of a version for a bundle_name
 
     The files should have been hard linked after command has been run
     """
     # GIVEN a context that is populated
-    store = populated_context["store"]
-    bundle: Bundle = store.Bundle.query.first()
+    store: Store = populated_context["store"]
+    bundle: Bundle = store._get_query(table=Bundle).first()
     version_obj = bundle.versions[0]
     bundle_name: str = bundle.name
     # GIVEN that the latest version of the bundle is not included
     assert version_obj.included_at is None
     # GIVEN that no version specific folder has been created since version is not included
     version_path = (
         populated_context["root"] / bundle.name / str(version_obj.created_at.date())
@@ -96,16 +97,16 @@
     populated_context: Context, cli_runner: CliRunner
 ):
     """Test to include the files of a version by specifying the version id
 
     The folder should have been created
     """
     # GIVEN a context that is populated
-    store = populated_context["store"]
-    bundle: Bundle = store.Bundle.query.first()
+    store: Store = populated_context["store"]
+    bundle: Bundle = store._get_query(table=Bundle).first()
     version_obj = bundle.versions[0]
     version_id = version_obj.id
     # GIVEN that the latest version of the bundle is not included
     assert version_obj.included_at is None
     # GIVEN that no version specific folder has been created since version is not included
     version_path = (
         populated_context["root"] / bundle.name / str(version_obj.created_at.date())
@@ -151,18 +152,18 @@
 ):
     """Test to include the files of a version that does not exist
 
     The command should exit since a valid version is needed
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context that is populated
-    store = populated_context["store"]
+    store: Store = populated_context["store"]
     # GIVEN a version that does not exists
     version_id = 10
-    assert not store.Version.get(version_id)
+    assert not store.get_version_by_id(version_id=version_id)
 
     # WHEN running the include files specifying the non existing version
     result = cli_runner.invoke(
         include, ["--version-id", version_id], obj=populated_context
     )
 
     # THEN assert that the command exists with zero code 1
@@ -198,19 +199,20 @@
 ):
     """Test to include the files in the latest version of a bundle that does not have versions
 
     The command should exit since a valid bundle with versions are needed
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN context with a bundle without versions
-    store = base_context["store"]
+    store: Store = base_context["store"]
     bundle_name = "hello"
 
     new_bundle = store.new_bundle(name=bundle_name, created_at=timestamp)
-    store.add_commit(new_bundle)
+    store.session.add(new_bundle)
+    store.session.commit()
 
     bundle = store.get_bundle_by_name(bundle_name=bundle_name)
     assert len(bundle.versions) == 0
 
     # WHEN running the include files specifying bundle without versions
     result = cli_runner.invoke(include, [bundle_name], obj=base_context)
 
@@ -225,16 +227,16 @@
 ):
     """Test to include the files of a version that is already included
 
     The command should exit since the version can not be included again
     """
     caplog.set_level(logging.DEBUG)
     # GIVEN a context that is populated and a version that is already included
-    store = populated_context["store"]
-    version_obj = store.Version.query.first()
+    store: Store = populated_context["store"]
+    version_obj = store._get_query(table=Version).first()
     version_id = version_obj.id
     result = cli_runner.invoke(
         include, ["--version-id", version_id], obj=populated_context
     )
 
     # WHEN trying to include the version again
     result = cli_runner.invoke(
```

### Comparing `housekeeper-4.0.1/tests/conftest.py` & `housekeeper-4.1.0/tests/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/helper_functions.py` & `housekeeper-4.1.0/tests/helper_functions.py`

 * *Files 10% similar despite different names*

```diff
@@ -34,30 +34,36 @@
         output = Helpers.get_stdout(output)
         return json.loads(output)
 
     @staticmethod
     def add_bundle(store: Store, bundle: dict) -> None:
         """Add and commit bundle to housekeeper store"""
         bundle_obj, _ = store.add_bundle(bundle)
-        store.add_commit(bundle_obj)
+        store.session.add(bundle_obj)
+        store.session.commit()
 
     @staticmethod
-    def create_bundle_data(case_id: str, files: List[dict], created_at: dt.datetime = None) -> dict:
+    def create_bundle_data(
+        case_id: str, files: List[dict], created_at: dt.datetime = None
+    ) -> dict:
         """
         Create a new bundle_data dictionary with the given parameters.
 
         :param case_id: The name of the bundle.
         :param files: A list of dictionaries representing file data.
         :param created_at: The timestamp when the bundle was created (optional).
         :return: A dictionary representing the bundle data.
         """
         if created_at is None:
             created_at = dt.datetime.now()
 
-        files = [{"path": str(file_data["file"]), "archive": True, "tags": file_data["tags"]} for file_data in files]
+        files = [
+            {"path": str(file_data["file"]), "archive": True, "tags": file_data["tags"]}
+            for file_data in files
+        ]
 
         data = {
             "name": case_id,
             "created_at": created_at,
             "files": files,
         }
```

### Comparing `housekeeper-4.0.1/tests/store/conftest.py` & `housekeeper-4.1.0/tests/store/conftest.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/store/test_add_core.py` & `housekeeper-4.1.0/tests/store/test_add_core.py`

 * *Files 19% similar despite different names*

```diff
@@ -1,107 +1,111 @@
 """Tests for store core functions"""
 
-from housekeeper.store import models
+from housekeeper.store.models import Bundle, File, Tag, Version
+from housekeeper.store.api.core import Store
 
 # tag tests
 
 
-def test_create_tag_obj(store, vcf_tag_name):
+def test_create_tag_obj(store: Store, vcf_tag_name):
     """Test to create a tag object"""
     # GIVEN a store and a tag name
     # WHEN creating a tag
     new_tag = store.new_tag(vcf_tag_name)
     # THEN assert a tag object was created
-    assert isinstance(new_tag, models.Tag)
+    assert isinstance(new_tag, Tag)
     assert new_tag.name == vcf_tag_name
 
 
-def test_add_tag(store, vcf_tag_obj):
+def test_add_tag(store: Store, vcf_tag_obj):
     """Test to add a tag"""
     # GIVEN a store without tags
-    assert store.Tag.query.count() == 0
+    assert store._get_query(table=Tag).count() == 0
     # WHEN adding a tag
-    store.add_commit(vcf_tag_obj)
+    store.session.add(vcf_tag_obj)
+    store.session.commit()
     # THEN assert the new tag was added
-    assert store.Tag.query.count() == 1
-    assert store.Tag.query.first() == vcf_tag_obj
+    assert store._get_query(table=Tag).count() == 1
+    assert store._get_query(table=Tag).first() == vcf_tag_obj
 
 
 # version tests
 
 
-def test_create_version_obj(store, timestamp):
+def test_create_version_obj(store: Store, timestamp):
     """Test to create a version object"""
     # GIVEN a store and a time stamp
     # WHEN creating a version
     new_version = store.new_version(created_at=timestamp, expires_at=timestamp)
     # THEN assert a version object was created
-    assert isinstance(new_version, models.Version)
+    assert isinstance(new_version, Version)
     assert new_version.created_at == timestamp
 
 
 # bundle tests
 
 
-def test_create_bundle_obj(store, bundle_data):
+def test_create_bundle_obj(store: Store, bundle_data):
     """Test to create a bundle object"""
     # GIVEN some bundle information
     # WHEN adding the new bundle
     bundle_obj = store.add_bundle(bundle_data)[0]
     # THEN the bundle should have correct name
     assert bundle_obj.name == bundle_data["name"]
     # THEN the bundle should have correct creation time
     assert bundle_obj.created_at == bundle_data["created_at"]
     # THEN assert that a version was added
     assert len(bundle_obj.versions) == 1
     # THEN assert that all files where added to the bundle
     assert len(bundle_obj.versions[0].files) == len(bundle_data["files"])
 
 
-def test_add_bundle(store, bundle_obj):
+def test_add_bundle(store: Store, bundle_obj):
     """Test to add a bundle to the store"""
     # GIVEN a store without files, tags, versions or bundles
-    assert store.Bundle.query.count() == 0
-    assert store.Tag.query.count() == 0
-    assert store.Version.query.count() == 0
-    assert store.File.query.count() == 0
+    assert store._get_query(table=Bundle).count() == 0
+    assert store._get_query(table=Tag).count() == 0
+    assert store._get_query(table=Version).count() == 0
+    assert store._get_query(table=File).count() == 0
     # WHEN adding the new bundle
-    store.add_commit(bundle_obj)
+    store.session.add(bundle_obj)
+    store.session.commit()
     # THEN assert that a bundle was added
-    assert store.Bundle.query.count() == 1
+    assert store._get_query(table=Bundle).count() == 1
     # THEN assert that the bundle is correct
-    assert store.Bundle.query.first() == bundle_obj
+    assert store._get_query(table=Bundle).first() == bundle_obj
     # THEN assert some tags where added
-    assert store.Tag.query.count() > 0
+    assert store._get_query(table=Tag).count() > 0
     # THEN assert some files where added
-    assert store.File.query.count() > 0
+    assert store._get_query(table=File).count() > 0
     # THEN assert we have a version
-    assert store.Version.query.count() > 0
+    assert store._get_query(table=Version).count() > 0
 
 
-def test_add_bundle_twice(populated_store, bundle_data):
+def test_add_bundle_twice(populated_store: Store, bundle_data):
     """Test to add a bundle twice"""
     store = populated_store
     # GIVEN a store ppopulated with a bundle
-    assert store.Bundle.query.count() > 0
+    assert store._get_query(table=Bundle).count() > 0
     # WHEN adding the same bundle again
     new_bundle = store.add_bundle(bundle_data)
     # THEN it should return None
     assert new_bundle is None
 
 
-def test_add_two_versions_of_bundle(populated_store, second_bundle_data):
+def test_add_two_versions_of_bundle(populated_store: Store, second_bundle_data):
     """Test to add two versions of the same bundle"""
-    store = populated_store
+    store: Store = populated_store
     # GIVEN a populated store and some modified bundle data
-    assert store.Bundle.query.count() > 0
+    assert store._get_query(table=Bundle).count() > 0
 
     # WHEN adding the modified bundle to the database
     new_bundle_obj = store.add_bundle(second_bundle_data)[0]
-    store.add_commit(new_bundle_obj)
+    store.session.add(new_bundle_obj)
+    store.session.commit()
 
     # THEN there should still be one bundle
-    assert store.Bundle.query.count() == 1
+    assert store._get_query(table=Bundle).count() == 1
     # THEN there should be two versions
-    assert store.Version.query.count() == 2
+    assert store._get_query(table=Version).count() == 2
     # THEN tere should be all four files
-    assert store.File.query.count() == 4
+    assert store._get_query(table=File).count() == 4
```

### Comparing `housekeeper-4.0.1/tests/store/test_add_file.py` & `housekeeper-4.1.0/tests/store/test_add_file.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/store/test_bundle_filters.py` & `housekeeper-4.1.0/tests/store/test_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/store/test_file_filters.py` & `housekeeper-4.1.0/tests/store/test_file_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/store/test_file_tag_filters.py` & `housekeeper-4.1.0/tests/store/test_file_tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/store/test_find_tag.py` & `housekeeper-4.1.0/tests/store/test_find_tag.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/store/test_store_api.py` & `housekeeper-4.1.0/tests/store/test_store_api.py`

 * *Files 18% similar despite different names*

```diff
@@ -1,38 +1,41 @@
 """Tests for the store api"""
 import datetime
 from typing import List
+from housekeeper.store.api.core import Store
 
 from housekeeper.store.models import File
 
 
 def test_get_files_before(populated_store, bundle_data_old, time_stamp_now):
     """
     Test return all files when two bundles are added.
     """
-    store = populated_store
+    store: Store = populated_store
     # GIVEN a store with two bundles and two files in each bundle
     bundle_old_obj, _ = store.add_bundle(data=bundle_data_old)
-    store.add_commit(bundle_old_obj)
+    store.session.add(bundle_old_obj)
+    store.session.commit()
 
     # WHEN fetching all files in the database
     files = store.get_files_before(before_date=time_stamp_now)
 
     # THEN all four files should be fetched
     assert len(files) == 4
 
 
 def test_get_past_files(populated_store, bundle_data_old, timestamp, old_timestamp):
     """
     test fetch files where not all files are older than before date
     """
-    store = populated_store
+    store: Store = populated_store
     # GIVEN a store with two bundles and two files in each bundle
     bundle_old_obj, _ = store.add_bundle(data=bundle_data_old)
-    store.add_commit(bundle_old_obj)
+    store.session.add(bundle_old_obj)
+    store.session.commit()
 
     # WHEN fetching all files before the oldest date
     date = old_timestamp + datetime.timedelta(days=10)
     assert old_timestamp < date < timestamp
     files: List[File] = store.get_files_before(before_date=date)
 
     # THEN a list of Files is returned
@@ -44,18 +47,19 @@
 
 def test_get_no_get_files_before_oldest(
     populated_store, bundle_data_old, old_timestamp, timestamp
 ):
     """
     Test get files where no files are older than before date.
     """
-    store = populated_store
+    store: Store = populated_store
     # GIVEN a store with two bundles and two files in each bundle
     bundle_old_obj, _ = store.add_bundle(data=bundle_data_old)
-    store.add_commit(bundle_old_obj)
+    store.session.add(bundle_old_obj)
+    store.session.commit()
 
     # WHEN fetching all files before the oldest date
     date = old_timestamp - datetime.timedelta(days=10)
     assert date < old_timestamp < timestamp
     files: List[File] = store.get_files_before(before_date=date)
 
     # THEN assert no files where that old
```

### Comparing `housekeeper-4.0.1/tests/store/test_store_models.py` & `housekeeper-4.1.0/tests/store/test_store_models.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/store/test_tag_filters.py` & `housekeeper-4.1.0/tests/store/test_tag_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/store/test_version_bundle_filters.py` & `housekeeper-4.1.0/tests/store/test_version_bundle_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/store/test_version_filters.py` & `housekeeper-4.1.0/tests/store/test_version_filters.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/test_date.py` & `housekeeper-4.1.0/tests/test_date.py`

 * *Files identical despite different names*

### Comparing `housekeeper-4.0.1/tests/test_include.py` & `housekeeper-4.1.0/tests/test_include.py`

 * *Files identical despite different names*

