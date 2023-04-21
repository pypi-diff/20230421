# Comparing `tmp/synapseclient-2.7.0.tar.gz` & `tmp/synapseclient-2.7.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "synapseclient-2.7.0.tar", last modified: Fri Sep 16 17:51:21 2022, max compression
+gzip compressed data, was "synapseclient-2.7.1.tar", last modified: Fri Apr 21 02:24:18 2023, max compression
```

## Comparing `synapseclient-2.7.0.tar` & `synapseclient-2.7.1.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.305595 synapseclient-2.7.0/
--rw-r--r--   0 runner    (1001) docker     (116)    11346 2022-09-16 17:51:04.000000 synapseclient-2.7.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (116)       60 2022-09-16 17:51:04.000000 synapseclient-2.7.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (116)     9753 2022-09-16 17:51:21.305595 synapseclient-2.7.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     6786 2022-09-16 17:51:04.000000 synapseclient-2.7.0/README.md
--rw-r--r--   0 runner    (1001) docker     (116)      219 2022-09-16 17:51:04.000000 synapseclient-2.7.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (116)      170 2022-09-16 17:51:21.305595 synapseclient-2.7.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (116)     4378 2022-09-16 17:51:04.000000 synapseclient-2.7.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.297595 synapseclient-2.7.0/synapseclient/
--rw-r--r--   0 runner    (1001) docker     (116)     2205 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/.synapseConfig
--rw-r--r--   0 runner    (1001) docker     (116)    10515 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    62616 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/__main__.py
--rw-r--r--   0 runner    (1001) docker     (116)    13165 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/activity.py
--rw-r--r--   0 runner    (1001) docker     (116)    14566 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/annotations.py
--rw-r--r--   0 runner    (1001) docker     (116)   192200 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/client.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.301595 synapseclient-2.7.0/synapseclient/core/
--rw-r--r--   0 runner    (1001) docker     (116)      302 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    14358 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/cache.py
--rw-r--r--   0 runner    (1001) docker     (116)       84 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/config.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.301595 synapseclient-2.7.0/synapseclient/core/constants/
--rw-r--r--   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/constants/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     2179 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/constants/concrete_types.py
--rw-r--r--   0 runner    (1001) docker     (116)       47 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/constants/config_file_constants.py
--rw-r--r--   0 runner    (1001) docker     (116)      116 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/constants/limits.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.301595 synapseclient-2.7.0/synapseclient/core/credentials/
--rw-r--r--   0 runner    (1001) docker     (116)      181 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/credentials/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)     1000 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/credentials/cached_sessions.py
--rw-r--r--   0 runner    (1001) docker     (116)     6160 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/credentials/cred_data.py
--rw-r--r--   0 runner    (1001) docker     (116)    10606 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/credentials/credential_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)     4400 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/cumulative_transfer_progress.py
--rw-r--r--   0 runner    (1001) docker     (116)      542 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/dozer.py
--rw-r--r--   0 runner    (1001) docker     (116)     5354 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3463 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/lock.py
--rw-r--r--   0 runner    (1001) docker     (116)     3034 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/logging_setup.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.301595 synapseclient-2.7.0/synapseclient/core/models/
--rw-r--r--   0 runner    (1001) docker     (116)      354 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/models/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)      777 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/models/custom_json.py
--rw-r--r--   0 runner    (1001) docker     (116)      777 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/models/dict_object.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.301595 synapseclient-2.7.0/synapseclient/core/multithread_download/
--rw-r--r--   0 runner    (1001) docker     (116)      240 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/multithread_download/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    15019 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/multithread_download/download_threads.py
--rw-r--r--   0 runner    (1001) docker     (116)     2352 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/pool_provider.py
--rw-r--r--   0 runner    (1001) docker     (116)    10515 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/remote_file_storage_wrappers.py
--rw-r--r--   0 runner    (1001) docker     (116)     6342 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/retry.py
--rw-r--r--   0 runner    (1001) docker     (116)     9380 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/sts_transfer.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.301595 synapseclient-2.7.0/synapseclient/core/upload/
--rw-r--r--   0 runner    (1001) docker     (116)      487 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/upload/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    22537 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/upload/multipart_upload.py
--rw-r--r--   0 runner    (1001) docker     (116)    10111 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/upload/upload_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)    32442 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/utils.py
--rw-r--r--   0 runner    (1001) docker     (116)     6173 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/core/version_check.py
--rw-r--r--   0 runner    (1001) docker     (116)    31930 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/entity.py
--rw-r--r--   0 runner    (1001) docker     (116)     9339 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (116)      216 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/synapsePythonClient
--rw-r--r--   0 runner    (1001) docker     (116)    97630 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/table.py
--rw-r--r--   0 runner    (1001) docker     (116)     3744 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/team.py
--rw-r--r--   0 runner    (1001) docker     (116)     5414 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseclient/wiki.py
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.297595 synapseclient-2.7.0/synapseclient.egg-info/
--rw-r--r--   0 runner    (1001) docker     (116)     9753 2022-09-16 17:51:21.000000 synapseclient-2.7.0/synapseclient.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (116)     2048 2022-09-16 17:51:21.000000 synapseclient-2.7.0/synapseclient.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-16 17:51:21.000000 synapseclient-2.7.0/synapseclient.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (116)       57 2022-09-16 17:51:21.000000 synapseclient-2.7.0/synapseclient.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (116)        1 2022-09-16 17:51:16.000000 synapseclient-2.7.0/synapseclient.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (116)      346 2022-09-16 17:51:21.000000 synapseclient-2.7.0/synapseclient.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (116)       27 2022-09-16 17:51:21.000000 synapseclient-2.7.0/synapseclient.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (116)        0 2022-09-16 17:51:21.305595 synapseclient-2.7.0/synapseutils/
--rw-r--r--   0 runner    (1001) docker     (116)      967 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseutils/__init__.py
--rw-r--r--   0 runner    (1001) docker     (116)    34034 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseutils/copy_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3176 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseutils/describe_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)    53112 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseutils/migrate_functions.py
--rw-r--r--   0 runner    (1001) docker     (116)     3291 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseutils/monitor.py
--rw-r--r--   0 runner    (1001) docker     (116)    44835 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseutils/sync.py
--rw-r--r--   0 runner    (1001) docker     (116)     3028 2022-09-16 17:51:04.000000 synapseclient-2.7.0/synapseutils/walk_functions.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.926428 synapseclient-2.7.1/
+-rw-r--r--   0 runner    (1001) docker     (122)    11346 2023-04-21 02:24:02.000000 synapseclient-2.7.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       60 2023-04-21 02:24:02.000000 synapseclient-2.7.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-04-21 02:24:18.926428 synapseclient-2.7.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     6786 2023-04-21 02:24:02.000000 synapseclient-2.7.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (122)      219 2023-04-21 02:24:02.000000 synapseclient-2.7.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (122)      170 2023-04-21 02:24:18.926428 synapseclient-2.7.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     4406 2023-04-21 02:24:02.000000 synapseclient-2.7.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/
+-rw-r--r--   0 runner    (1001) docker     (122)     2205 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/.synapseConfig
+-rw-r--r--   0 runner    (1001) docker     (122)    10913 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    62616 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/__main__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    13165 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/activity.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14566 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/annotations.py
+-rw-r--r--   0 runner    (1001) docker     (122)   192200 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/client.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/core/
+-rw-r--r--   0 runner    (1001) docker     (122)      302 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    14358 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/cache.py
+-rw-r--r--   0 runner    (1001) docker     (122)       84 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/config.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/core/constants/
+-rw-r--r--   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/constants/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2179 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/constants/concrete_types.py
+-rw-r--r--   0 runner    (1001) docker     (122)       47 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/constants/config_file_constants.py
+-rw-r--r--   0 runner    (1001) docker     (122)      116 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/constants/limits.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/core/credentials/
+-rw-r--r--   0 runner    (1001) docker     (122)      181 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/credentials/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)     1000 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/credentials/cached_sessions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6160 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/credentials/cred_data.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10606 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/credentials/credential_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)     4400 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/cumulative_transfer_progress.py
+-rw-r--r--   0 runner    (1001) docker     (122)      542 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/dozer.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5354 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3463 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/lock.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3034 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/logging_setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient/core/models/
+-rw-r--r--   0 runner    (1001) docker     (122)      354 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/models/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/models/custom_json.py
+-rw-r--r--   0 runner    (1001) docker     (122)      777 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/models/dict_object.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.926428 synapseclient-2.7.1/synapseclient/core/multithread_download/
+-rw-r--r--   0 runner    (1001) docker     (122)      240 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/multithread_download/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    15019 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/multithread_download/download_threads.py
+-rw-r--r--   0 runner    (1001) docker     (122)     2352 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/pool_provider.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10515 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/remote_file_storage_wrappers.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6342 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/retry.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9380 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/sts_transfer.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.926428 synapseclient-2.7.1/synapseclient/core/upload/
+-rw-r--r--   0 runner    (1001) docker     (122)      487 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/upload/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    22537 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/upload/multipart_upload.py
+-rw-r--r--   0 runner    (1001) docker     (122)    10111 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/upload/upload_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    32442 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/utils.py
+-rw-r--r--   0 runner    (1001) docker     (122)     6173 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/core/version_check.py
+-rw-r--r--   0 runner    (1001) docker     (122)    31930 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/entity.py
+-rw-r--r--   0 runner    (1001) docker     (122)     9339 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (122)      216 2023-04-21 02:24:03.000000 synapseclient-2.7.1/synapseclient/synapsePythonClient
+-rw-r--r--   0 runner    (1001) docker     (122)    97630 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/table.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3744 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/team.py
+-rw-r--r--   0 runner    (1001) docker     (122)     5414 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseclient/wiki.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.922428 synapseclient-2.7.1/synapseclient.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     9751 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2048 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       57 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 02:24:13.000000 synapseclient-2.7.1/synapseclient.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (122)      369 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       27 2023-04-21 02:24:18.000000 synapseclient-2.7.1/synapseclient.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 02:24:18.926428 synapseclient-2.7.1/synapseutils/
+-rw-r--r--   0 runner    (1001) docker     (122)      967 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (122)    34034 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/copy_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3176 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/describe_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)    53112 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/migrate_functions.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3291 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/monitor.py
+-rw-r--r--   0 runner    (1001) docker     (122)    44835 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/sync.py
+-rw-r--r--   0 runner    (1001) docker     (122)     3028 2023-04-21 02:24:02.000000 synapseclient-2.7.1/synapseutils/walk_functions.py
```

### Comparing `synapseclient-2.7.0/LICENSE` & `synapseclient-2.7.1/LICENSE`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/PKG-INFO` & `synapseclient-2.7.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapseclient
-Version: 2.7.0
+Version: 2.7.1
 Summary: A client for Synapse, a collaborative compute space  that allows scientists to share and analyze data together.
 Home-page: https://www.synapse.org
 Author: The Synapse Engineering Team
 Author-email: platform@sagebase.org
 License: Apache
 Project-URL: Documentation, https://python-docs.synapse.org
 Project-URL: Source Code, https://github.com/Sage-Bionetworks/synapsePythonClient
@@ -202,14 +202,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 Provides-Extra: pysftp
 Provides-Extra: boto3
 Provides-Extra: docs
 Provides-Extra: tests
```

### Comparing `synapseclient-2.7.0/README.md` & `synapseclient-2.7.1/README.md`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/setup.py` & `synapseclient-2.7.1/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -41,14 +41,15 @@
     "pytest-xdist[psutil]>=2.2,<3.0.0",
 ]
 
 install_requires = [
     "requests>=2.22.0,<3.0",
     "keyring>=15,<23.5",
     "deprecated>=1.2.4,<2.0",
+    "importlib-metadata<5.0",
 ]
 
 # on Linux specify a cryptography dependency that will not
 # require a Rust compiler to compile from source (< 3.4).
 # on Linux cryptography is a transitive dependency
 # (keyring -> SecretStorage -> cryptography)
 # SecretStorage doesn't pin a version so otherwise if cryptography
@@ -68,18 +69,18 @@
 
 setuptools.setup(
     # basic
     name="synapseclient",
     version=__version__,
     packages=setuptools.find_packages(exclude=["tests", "tests.*"]),
     # requirements
-    python_requires=">=3.7.*",
+    python_requires=">=3.7",
     install_requires=install_requires,
     extras_require={
-        "pandas": ["pandas>=0.25.0,<2.0"],
+        "pandas": ["pandas>=0.25.0,<1.5"],
         "pysftp": ["pysftp>=0.2.8,<0.3"],
         "boto3": ["boto3>=1.7.0,<2.0"],
         "docs": ["sphinx>=3.0,<4.0", "sphinx-argparse>=0.2,<0.3"],
         "tests": test_deps,
         ':sys_platform=="linux"': ["keyrings.alt==3.1"],
     },
     # command line
```

### Comparing `synapseclient-2.7.0/synapseclient/.synapseConfig` & `synapseclient-2.7.1/synapseclient/.synapseConfig`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/__init__.py` & `synapseclient-2.7.1/synapseclient/__init__.py`

 * *Files 3% similar despite different names*

```diff
@@ -17,14 +17,28 @@
 `Java <https://github.com/Sage-Bionetworks/Synapse-Repository-Services/tree/develop/client/synapseJavaClient>`_, and
 the `web <https://www.synapse.org/>`_. The Python client can also be used from the
 `command line <CommandLineClient.html>`_.
 
 If you're just getting started with Synapse, have a look at the Getting Started guides for
 `Synapse <https://docs.synapse.org/articles/getting_started.html>`_.
 
+
+Next Major Release (3.0.0)
+==========================
+- Support only pandas `>=` 1.5
+- Remove support for Python 3.7 due to its end of life.
+- Remove support for login via passwords for best security practices.
+- There will be major cosmetic changes to the cli such as
+  removing all camel case or non-standard single dash long command line interface (cli)
+  parameters.
+  Example: command line arguments like `-parent` will become
+  `--parent`.  Commands that support camel case like `--parentId`
+  will be changed to `--parent-id`.
+
+
 Installation
 ============
 
 The `synapseclient <https://pypi.python.org/pypi/synapseclient/>`_ package is available from PyPI. It can be installed
 or upgraded with pip. Note that synapseclient requires Python 3, and if you have both Python 2 and Python 3
 installations your system, the pip command associated with Python 3 may be named pip3 to distinguish it from a
 Python 2 associated command. Prefixing the pip installation with sudo may be necessary if you are installing Python
@@ -52,19 +66,14 @@
 
 Next, either install the package in the site-packages directory ``python setup.py install`` or
  ``python setup.py develop`` to make the installation follow the head without having to reinstall::
 
     python setup.py <install or develop>
 
 
-Python 2 Support
-----------------
-
-synapseclient versions 2.0 and above require Python 3.6 or greater. Python 2.7 is no longer supported.
-
 Connecting to Synapse
 =====================
 
 To use Synapse, you'll need to `register <https://www.synapse.org/register>`_ for an account. The Synapse
 website can authenticate using a Google account, but you'll need to take the extra step of creating a Synapse password
 to use the programmatic clients.
```

### Comparing `synapseclient-2.7.0/synapseclient/__main__.py` & `synapseclient-2.7.1/synapseclient/__main__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/activity.py` & `synapseclient-2.7.1/synapseclient/activity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/annotations.py` & `synapseclient-2.7.1/synapseclient/annotations.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/client.py` & `synapseclient-2.7.1/synapseclient/client.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/cache.py` & `synapseclient-2.7.1/synapseclient/core/cache.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/constants/concrete_types.py` & `synapseclient-2.7.1/synapseclient/core/constants/concrete_types.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/credentials/cached_sessions.py` & `synapseclient-2.7.1/synapseclient/core/credentials/cached_sessions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/credentials/cred_data.py` & `synapseclient-2.7.1/synapseclient/core/credentials/cred_data.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/credentials/credential_provider.py` & `synapseclient-2.7.1/synapseclient/core/credentials/credential_provider.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/cumulative_transfer_progress.py` & `synapseclient-2.7.1/synapseclient/core/cumulative_transfer_progress.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/dozer.py` & `synapseclient-2.7.1/synapseclient/core/dozer.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/exceptions.py` & `synapseclient-2.7.1/synapseclient/core/exceptions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/lock.py` & `synapseclient-2.7.1/synapseclient/core/lock.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/logging_setup.py` & `synapseclient-2.7.1/synapseclient/core/logging_setup.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/models/custom_json.py` & `synapseclient-2.7.1/synapseclient/core/models/custom_json.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/models/dict_object.py` & `synapseclient-2.7.1/synapseclient/core/models/dict_object.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/multithread_download/download_threads.py` & `synapseclient-2.7.1/synapseclient/core/multithread_download/download_threads.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/pool_provider.py` & `synapseclient-2.7.1/synapseclient/core/pool_provider.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/remote_file_storage_wrappers.py` & `synapseclient-2.7.1/synapseclient/core/remote_file_storage_wrappers.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/retry.py` & `synapseclient-2.7.1/synapseclient/core/retry.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/sts_transfer.py` & `synapseclient-2.7.1/synapseclient/core/sts_transfer.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/upload/multipart_upload.py` & `synapseclient-2.7.1/synapseclient/core/upload/multipart_upload.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/upload/upload_functions.py` & `synapseclient-2.7.1/synapseclient/core/upload/upload_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/utils.py` & `synapseclient-2.7.1/synapseclient/core/utils.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/core/version_check.py` & `synapseclient-2.7.1/synapseclient/core/version_check.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/entity.py` & `synapseclient-2.7.1/synapseclient/entity.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/evaluation.py` & `synapseclient-2.7.1/synapseclient/evaluation.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/table.py` & `synapseclient-2.7.1/synapseclient/table.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/team.py` & `synapseclient-2.7.1/synapseclient/team.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient/wiki.py` & `synapseclient-2.7.1/synapseclient/wiki.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseclient.egg-info/PKG-INFO` & `synapseclient-2.7.1/synapseclient.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: synapseclient
-Version: 2.7.0
+Version: 2.7.1
 Summary: A client for Synapse, a collaborative compute space  that allows scientists to share and analyze data together.
 Home-page: https://www.synapse.org
 Author: The Synapse Engineering Team
 Author-email: platform@sagebase.org
 License: Apache
 Project-URL: Documentation, https://python-docs.synapse.org
 Project-URL: Source Code, https://github.com/Sage-Bionetworks/synapsePythonClient
@@ -202,14 +202,14 @@
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Intended Audience :: Developers
 Classifier: Intended Audience :: Science/Research
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Topic :: Software Development :: Libraries
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Bio-Informatics
-Requires-Python: >=3.7.*
+Requires-Python: >=3.7
 Description-Content-Type: text/markdown
 Provides-Extra: pandas
 Provides-Extra: pysftp
 Provides-Extra: boto3
 Provides-Extra: docs
 Provides-Extra: tests
```

### Comparing `synapseclient-2.7.0/synapseclient.egg-info/SOURCES.txt` & `synapseclient-2.7.1/synapseclient.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseutils/__init__.py` & `synapseclient-2.7.1/synapseutils/__init__.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseutils/copy_functions.py` & `synapseclient-2.7.1/synapseutils/copy_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseutils/describe_functions.py` & `synapseclient-2.7.1/synapseutils/describe_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseutils/migrate_functions.py` & `synapseclient-2.7.1/synapseutils/migrate_functions.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseutils/monitor.py` & `synapseclient-2.7.1/synapseutils/monitor.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseutils/sync.py` & `synapseclient-2.7.1/synapseutils/sync.py`

 * *Files identical despite different names*

### Comparing `synapseclient-2.7.0/synapseutils/walk_functions.py` & `synapseclient-2.7.1/synapseutils/walk_functions.py`

 * *Files identical despite different names*

