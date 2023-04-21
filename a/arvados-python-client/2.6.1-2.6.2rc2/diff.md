# Comparing `tmp/arvados-python-client-2.6.1.tar.gz` & `tmp/arvados-python-client-2.6.2rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was ".upload_dist/arvados-python-client-2.6.1.tar", last modified: Mon Apr 17 21:06:13 2023, max compression
+gzip compressed data, was ".upload_dist/arvados-python-client-2.6.2rc2.tar", last modified: Fri Apr 21 19:29:28 2023, max compression
```

## Comparing `arvados-python-client-2.6.1.tar` & `arvados-python-client-2.6.2rc2.tar`

### file list

```diff
@@ -1,93 +1,98 @@
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/LICENSE-2.0.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      168 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/MANIFEST.in
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2952 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2088 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/README.rst
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/arvados/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6450 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2329 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/_normalize_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/_ranges.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       22 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/arvados/_version.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17005 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    49239 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    76777 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/collection.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/arvados/commands/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2125 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/_util.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    31921 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/arv_copy.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18701 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/federation_migrate.py
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13261 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23760 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3357 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11841 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/migrate19.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57541 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/run.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4765 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/commands/ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1629 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/config.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      896 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9017 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/diskcache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    64081 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/keep.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8472 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2635 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3750 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/timer.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19413 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados/vocabulary.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/arvados_python_client.egg-info/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2952 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/arvados_python_client.egg-info/PKG-INFO
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1964 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/arvados_python_client.egg-info/SOURCES.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/arvados_python_client.egg-info/dependency_links.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.6.1/arvados_python_client.egg-info/not-zip-safe
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      244 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/arvados_python_client.egg-info/requires.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/arvados_python_client.egg-info/top_level.txt
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/arvados_version.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/bin/
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/bin/arv-copy
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/bin/arv-federation-migrate
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/bin/arv-get
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/bin/arv-keepdocker
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/bin/arv-ls
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/bin/arv-migrate-docker19
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/bin/arv-normalize
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/bin/arv-put
--rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/bin/arv-ws
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/setup.cfg
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2026 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/setup.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/tests/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10182 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/arvados_testutil.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/keepstub.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/manifest_examples.py
-drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:13.000000 arvados-python-client-2.6.1/tests/performance/
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/performance/__init__.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/performance/performance_profiler.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/performance/test_a_sample.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    38152 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/run_test_server.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/slow_test.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18619 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_api.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_arv_copy.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8686 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_arv_get.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10021 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_arv_keepdocker.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_arv_ls.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_arv_normalize.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_arv_put.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_arv_ws.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43464 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_arvfile.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_benchmark_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_cache.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77435 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_collections.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_crunch.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_errors.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_events.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    82578 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_keep_client.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_keep_locator.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_retry.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2425 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_retry_job_helpers.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_safeapi.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_sdk.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11619 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_stream.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7865 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_util.py
--rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2023-04-17 21:06:09.000000 arvados-python-client-2.6.1/tests/test_vocabulary.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11358 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/LICENSE-2.0.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      230 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/MANIFEST.in
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2088 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/README.rst
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     6450 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2329 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/_normalize_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3492 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/arvados/_pycurlhelper.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9074 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/_ranges.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       25 2023-04-21 19:29:27.000000 arvados-python-client-2.6.2rc2/arvados/_version.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    17005 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    49239 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2075 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    76777 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/collection.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados/commands/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2125 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/_util.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    31921 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/arv_copy.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    18701 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/federation_migrate.py
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    13261 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    23760 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3357 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11841 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/migrate19.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    57541 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9932 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/run.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4765 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/commands/ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1629 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/config.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      896 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     9017 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/diskcache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3037 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    13462 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    12489 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/arvados/http_to_keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    61059 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/arvados/keep.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8472 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2635 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3750 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      583 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/timer.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    19413 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4718 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados/vocabulary.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)   370019 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/arvados-v1-discovery.json
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2955 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/PKG-INFO
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2077 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/SOURCES.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/dependency_links.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        1 2018-09-21 15:00:39.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/not-zip-safe
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      278 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/requires.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       14 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/top_level.txt
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2107 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/arvados_version.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/bin/
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      172 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-copy
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      182 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-federation-migrate
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      202 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-get
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      174 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-keepdocker
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      225 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-ls
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      173 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-migrate-docker19
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)     1291 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-normalize
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      167 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-put
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)      166 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/bin/arv-ws
+-rwxr-xr-x   0 jenkins   (1001) jenkins   (1002)    12910 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/discovery2pydoc.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)       38 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/setup.cfg
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4676 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/setup.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/tests/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10182 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/arvados_testutil.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8748 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/keepstub.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      982 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/manifest_examples.py
+drwxr-xr-x   0 jenkins   (1001) jenkins   (1002)        0 2023-04-21 19:29:28.000000 arvados-python-client-2.6.2rc2/tests/performance/
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)        0 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/performance/__init__.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1394 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/performance/performance_profiler.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      510 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/performance/test_a_sample.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    38152 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/run_test_server.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      246 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/slow_test.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18619 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_api.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3622 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_copy.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8686 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_get.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    10021 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_keepdocker.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     4088 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_ls.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1196 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_normalize.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    68490 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_put.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)      837 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arv_ws.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    43464 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_arvfile.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3606 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_benchmark_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2925 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_cache.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    77435 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_collections.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1045 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_crunch.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3076 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_errors.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    16223 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_events.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    18037 2023-04-21 19:29:20.000000 arvados-python-client-2.6.2rc2/tests/test_http.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    82578 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_keep_client.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     3597 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_keep_locator.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     8293 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_retry.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2425 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_retry_job_helpers.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     2467 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_safeapi.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     1625 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_sdk.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    11619 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_stream.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)     7865 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_util.py
+-rw-r--r--   0 jenkins   (1001) jenkins   (1002)    14073 2023-04-17 21:06:09.000000 arvados-python-client-2.6.2rc2/tests/test_vocabulary.py
```

### Comparing `arvados-python-client-2.6.1/LICENSE-2.0.txt` & `arvados-python-client-2.6.2rc2/LICENSE-2.0.txt`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/PKG-INFO` & `arvados-python-client-2.6.2rc2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.6.1
+Version: 2.6.2rc2
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.6.1/README.rst` & `arvados-python-client-2.6.2rc2/README.rst`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/__init__.py` & `arvados-python-client-2.6.2rc2/arvados/__init__.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/_normalize_stream.py` & `arvados-python-client-2.6.2rc2/arvados/_normalize_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/_ranges.py` & `arvados-python-client-2.6.2rc2/arvados/_ranges.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/api.py` & `arvados-python-client-2.6.2rc2/arvados/api.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/arvfile.py` & `arvados-python-client-2.6.2rc2/arvados/arvfile.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/cache.py` & `arvados-python-client-2.6.2rc2/arvados/cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/collection.py` & `arvados-python-client-2.6.2rc2/arvados/collection.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/_util.py` & `arvados-python-client-2.6.2rc2/arvados/commands/_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/arv_copy.py` & `arvados-python-client-2.6.2rc2/arvados/commands/arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/federation_migrate.py` & `arvados-python-client-2.6.2rc2/arvados/commands/federation_migrate.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/get.py` & `arvados-python-client-2.6.2rc2/arvados/commands/get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/keepdocker.py` & `arvados-python-client-2.6.2rc2/arvados/commands/keepdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/ls.py` & `arvados-python-client-2.6.2rc2/arvados/commands/ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/migrate19.py` & `arvados-python-client-2.6.2rc2/arvados/commands/migrate19.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/put.py` & `arvados-python-client-2.6.2rc2/arvados/commands/put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/run.py` & `arvados-python-client-2.6.2rc2/arvados/commands/run.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/commands/ws.py` & `arvados-python-client-2.6.2rc2/arvados/commands/ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/config.py` & `arvados-python-client-2.6.2rc2/arvados/config.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/crunch.py` & `arvados-python-client-2.6.2rc2/arvados/crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/diskcache.py` & `arvados-python-client-2.6.2rc2/arvados/diskcache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/errors.py` & `arvados-python-client-2.6.2rc2/arvados/errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/events.py` & `arvados-python-client-2.6.2rc2/arvados/events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/keep.py` & `arvados-python-client-2.6.2rc2/arvados/keep.py`

 * *Files 3% similar despite different names*

```diff
@@ -40,14 +40,15 @@
 
 import arvados
 import arvados.config as config
 import arvados.errors
 import arvados.retry as retry
 import arvados.util
 import arvados.diskcache
+from arvados._pycurlhelper import PyCurlHelper
 
 _logger = logging.getLogger('arvados.keep')
 global_client_object = None
 
 
 # Monkey patch TCP constants when not available (apple). Values sourced from:
 # http://www.opensource.apple.com/source/xnu/xnu-2422.115.4/bsd/netinet/tcp.h
@@ -401,26 +402,18 @@
 
     def get(self):
         with self._lk:
             return self._val
 
 
 class KeepClient(object):
+    DEFAULT_TIMEOUT = PyCurlHelper.DEFAULT_TIMEOUT
+    DEFAULT_PROXY_TIMEOUT = PyCurlHelper.DEFAULT_PROXY_TIMEOUT
 
-    # Default Keep server connection timeout:  2 seconds
-    # Default Keep server read timeout:       256 seconds
-    # Default Keep server bandwidth minimum:  32768 bytes per second
-    # Default Keep proxy connection timeout:  20 seconds
-    # Default Keep proxy read timeout:        256 seconds
-    # Default Keep proxy bandwidth minimum:   32768 bytes per second
-    DEFAULT_TIMEOUT = (2, 256, 32768)
-    DEFAULT_PROXY_TIMEOUT = (20, 256, 32768)
-
-
-    class KeepService(object):
+    class KeepService(PyCurlHelper):
         """Make requests to a single Keep service, and track results.
 
         A KeepService is intended to last long enough to perform one
         transaction (GET or PUT) against one Keep service. This can
         involve calling either get() or put() multiple times in order
         to retry after transient failures. However, calling both get()
         and put() on a single instance -- or using the same instance
@@ -435,14 +428,15 @@
         )
 
         def __init__(self, root, user_agent_pool=queue.LifoQueue(),
                      upload_counter=None,
                      download_counter=None,
                      headers={},
                      insecure=False):
+            super(KeepClient.KeepService, self).__init__()
             self.root = root
             self._user_agent_pool = user_agent_pool
             self._result = {'error': None}
             self._usable = True
             self._session = None
             self._socket = None
             self.get_headers = {'Accept': 'application/octet-stream'}
@@ -472,38 +466,14 @@
         def _put_user_agent(self, ua):
             try:
                 ua.reset()
                 self._user_agent_pool.put(ua, block=False)
             except:
                 ua.close()
 
-        def _socket_open(self, *args, **kwargs):
-            if len(args) + len(kwargs) == 2:
-                return self._socket_open_pycurl_7_21_5(*args, **kwargs)
-            else:
-                return self._socket_open_pycurl_7_19_3(*args, **kwargs)
-
-        def _socket_open_pycurl_7_19_3(self, family, socktype, protocol, address=None):
-            return self._socket_open_pycurl_7_21_5(
-                purpose=None,
-                address=collections.namedtuple(
-                    'Address', ['family', 'socktype', 'protocol', 'addr'],
-                )(family, socktype, protocol, address))
-
-        def _socket_open_pycurl_7_21_5(self, purpose, address):
-            """Because pycurl doesn't have CURLOPT_TCP_KEEPALIVE"""
-            s = socket.socket(address.family, address.socktype, address.protocol)
-            s.setsockopt(socket.SOL_SOCKET, socket.SO_KEEPALIVE, 1)
-            # Will throw invalid protocol error on mac. This test prevents that.
-            if hasattr(socket, 'TCP_KEEPIDLE'):
-                s.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPIDLE, 75)
-            s.setsockopt(socket.IPPROTO_TCP, socket.TCP_KEEPINTVL, 75)
-            self._socket = s
-            return s
-
         def get(self, locator, method="GET", timeout=None):
             # locator is a KeepLocator object.
             url = self.root + str(locator)
             _logger.debug("Request: %s %s", method, url)
             curl = self._get_user_agent()
             ok = None
             try:
@@ -521,14 +491,16 @@
                     if self.insecure:
                         curl.setopt(pycurl.SSL_VERIFYPEER, 0)
                         curl.setopt(pycurl.SSL_VERIFYHOST, 0)
                     else:
                         curl.setopt(pycurl.CAINFO, arvados.util.ca_certs_path())
                     if method == "HEAD":
                         curl.setopt(pycurl.NOBODY, True)
+                    else:
+                        curl.setopt(pycurl.HTTPGET, True)
                     self._setcurltimeouts(curl, timeout, method=="HEAD")
 
                     try:
                         curl.perform()
                     except Exception as e:
                         raise arvados.errors.HttpError(0, str(e))
                     finally:
@@ -665,51 +637,14 @@
                          len(body),
                          t.msecs,
                          1.0*len(body)/2**20/t.secs if t.secs > 0 else 0)
             if self.upload_counter:
                 self.upload_counter.add(len(body))
             return True
 
-        def _setcurltimeouts(self, curl, timeouts, ignore_bandwidth=False):
-            if not timeouts:
-                return
-            elif isinstance(timeouts, tuple):
-                if len(timeouts) == 2:
-                    conn_t, xfer_t = timeouts
-                    bandwidth_bps = KeepClient.DEFAULT_TIMEOUT[2]
-                else:
-                    conn_t, xfer_t, bandwidth_bps = timeouts
-            else:
-                conn_t, xfer_t = (timeouts, timeouts)
-                bandwidth_bps = KeepClient.DEFAULT_TIMEOUT[2]
-            curl.setopt(pycurl.CONNECTTIMEOUT_MS, int(conn_t*1000))
-            if not ignore_bandwidth:
-                curl.setopt(pycurl.LOW_SPEED_TIME, int(math.ceil(xfer_t)))
-                curl.setopt(pycurl.LOW_SPEED_LIMIT, int(math.ceil(bandwidth_bps)))
-
-        def _headerfunction(self, header_line):
-            if isinstance(header_line, bytes):
-                header_line = header_line.decode('iso-8859-1')
-            if ':' in header_line:
-                name, value = header_line.split(':', 1)
-                name = name.strip().lower()
-                value = value.strip()
-            elif self._headers:
-                name = self._lastheadername
-                value = self._headers[name] + ' ' + header_line.strip()
-            elif header_line.startswith('HTTP/'):
-                name = 'x-status-line'
-                value = header_line
-            else:
-                _logger.error("Unexpected header line: %s", header_line)
-                return
-            self._lastheadername = name
-            self._headers[name] = value
-            # Returning None implies all bytes were written
-
 
     class KeepWriterQueue(queue.Queue):
         def __init__(self, copies, classes=[]):
             queue.Queue.__init__(self) # Old-style superclass
             self.wanted_copies = copies
             self.wanted_storage_classes = classes
             self.successful_copies = 0
```

### Comparing `arvados-python-client-2.6.1/arvados/retry.py` & `arvados-python-client-2.6.2rc2/arvados/retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/safeapi.py` & `arvados-python-client-2.6.2rc2/arvados/safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/stream.py` & `arvados-python-client-2.6.2rc2/arvados/stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/timer.py` & `arvados-python-client-2.6.2rc2/arvados/timer.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/util.py` & `arvados-python-client-2.6.2rc2/arvados/util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados/vocabulary.py` & `arvados-python-client-2.6.2rc2/arvados/vocabulary.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/arvados_python_client.egg-info/PKG-INFO` & `arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 1.1
 Name: arvados-python-client
-Version: 2.6.1
+Version: 2.6.2rc2
 Summary: Arvados client library
 Home-page: https://arvados.org
 Author: Arvados
 Author-email: info@arvados.org
 License: Apache 2.0
 Download-URL: https://github.com/arvados/arvados.git
 Description: .. Copyright (C) The Arvados Authors. All rights reserved.
```

### Comparing `arvados-python-client-2.6.1/arvados_python_client.egg-info/SOURCES.txt` & `arvados-python-client-2.6.2rc2/arvados_python_client.egg-info/SOURCES.txt`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,29 @@
 LICENSE-2.0.txt
 MANIFEST.in
 README.rst
+arvados-v1-discovery.json
 arvados_version.py
+discovery2pydoc.py
 setup.py
 arvados/__init__.py
 arvados/_normalize_stream.py
+arvados/_pycurlhelper.py
 arvados/_ranges.py
 arvados/_version.py
 arvados/api.py
 arvados/arvfile.py
 arvados/cache.py
 arvados/collection.py
 arvados/config.py
 arvados/crunch.py
 arvados/diskcache.py
 arvados/errors.py
 arvados/events.py
+arvados/http_to_keep.py
 arvados/keep.py
 arvados/retry.py
 arvados/safeapi.py
 arvados/stream.py
 arvados/timer.py
 arvados/util.py
 arvados/vocabulary.py
@@ -66,14 +70,15 @@
 tests/test_arvfile.py
 tests/test_benchmark_collections.py
 tests/test_cache.py
 tests/test_collections.py
 tests/test_crunch.py
 tests/test_errors.py
 tests/test_events.py
+tests/test_http.py
 tests/test_keep_client.py
 tests/test_keep_locator.py
 tests/test_retry.py
 tests/test_retry_job_helpers.py
 tests/test_safeapi.py
 tests/test_sdk.py
 tests/test_stream.py
```

### Comparing `arvados-python-client-2.6.1/arvados_version.py` & `arvados-python-client-2.6.2rc2/arvados_version.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/bin/arv-normalize` & `arvados-python-client-2.6.2rc2/bin/arv-normalize`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/arvados_testutil.py` & `arvados-python-client-2.6.2rc2/tests/arvados_testutil.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/keepstub.py` & `arvados-python-client-2.6.2rc2/tests/keepstub.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/manifest_examples.py` & `arvados-python-client-2.6.2rc2/tests/manifest_examples.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/performance/performance_profiler.py` & `arvados-python-client-2.6.2rc2/tests/performance/performance_profiler.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/run_test_server.py` & `arvados-python-client-2.6.2rc2/tests/run_test_server.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_api.py` & `arvados-python-client-2.6.2rc2/tests/test_api.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_arv_copy.py` & `arvados-python-client-2.6.2rc2/tests/test_arv_copy.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_arv_get.py` & `arvados-python-client-2.6.2rc2/tests/test_arv_get.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_arv_keepdocker.py` & `arvados-python-client-2.6.2rc2/tests/test_arv_keepdocker.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_arv_ls.py` & `arvados-python-client-2.6.2rc2/tests/test_arv_ls.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_arv_normalize.py` & `arvados-python-client-2.6.2rc2/tests/test_arv_normalize.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_arv_put.py` & `arvados-python-client-2.6.2rc2/tests/test_arv_put.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_arv_ws.py` & `arvados-python-client-2.6.2rc2/tests/test_arv_ws.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_arvfile.py` & `arvados-python-client-2.6.2rc2/tests/test_arvfile.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_benchmark_collections.py` & `arvados-python-client-2.6.2rc2/tests/test_benchmark_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_cache.py` & `arvados-python-client-2.6.2rc2/tests/test_cache.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_collections.py` & `arvados-python-client-2.6.2rc2/tests/test_collections.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_crunch.py` & `arvados-python-client-2.6.2rc2/tests/test_crunch.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_errors.py` & `arvados-python-client-2.6.2rc2/tests/test_errors.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_events.py` & `arvados-python-client-2.6.2rc2/tests/test_events.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_keep_client.py` & `arvados-python-client-2.6.2rc2/tests/test_keep_client.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_keep_locator.py` & `arvados-python-client-2.6.2rc2/tests/test_keep_locator.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_retry.py` & `arvados-python-client-2.6.2rc2/tests/test_retry.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_retry_job_helpers.py` & `arvados-python-client-2.6.2rc2/tests/test_retry_job_helpers.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_safeapi.py` & `arvados-python-client-2.6.2rc2/tests/test_safeapi.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_sdk.py` & `arvados-python-client-2.6.2rc2/tests/test_sdk.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_stream.py` & `arvados-python-client-2.6.2rc2/tests/test_stream.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_util.py` & `arvados-python-client-2.6.2rc2/tests/test_util.py`

 * *Files identical despite different names*

### Comparing `arvados-python-client-2.6.1/tests/test_vocabulary.py` & `arvados-python-client-2.6.2rc2/tests/test_vocabulary.py`

 * *Files identical despite different names*

