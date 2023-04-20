# Comparing `tmp/aerospike-8.0.0.tar.gz` & `tmp/aerospike-9.0.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "/home/jnguyen/clients/aerospike-client-python/dist/tmpewhwkx2g/aerospike-8.0.0.tar", last modified: Fri Nov 18 23:36:09 2022, max compression
+gzip compressed data, was "aerospike-9.0.0.tar", last modified: Wed Jan  4 00:50:47 2023, max compression
```

## Comparing `aerospike-8.0.0.tar` & `aerospike-9.0.0.tar`

### file list

```diff
@@ -1,1621 +1,1621 @@
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      434 2022-11-18 21:52:58.000000 aerospike-8.0.0/.build.yml
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4734 2022-11-18 21:52:58.000000 aerospike-8.0.0/.clang-format
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/.github/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/.github/workflows/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2391 2022-11-18 23:24:47.000000 aerospike-8.0.0/.github/workflows/tests.yml
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      121 2022-10-20 21:22:20.000000 aerospike-8.0.0/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      193 2022-11-18 21:56:05.000000 aerospike-8.0.0/.gitmodules
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4378 2022-11-18 22:05:26.000000 aerospike-8.0.0/BUILD.md
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11357 2022-09-19 18:31:26.000000 aerospike-8.0.0/LICENSE
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      187 2022-10-24 21:56:49.000000 aerospike-8.0.0/MANIFEST.in
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4962 2022-11-18 23:36:09.000000 aerospike-8.0.0/PKG-INFO
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4227 2022-11-18 21:52:58.000000 aerospike-8.0.0/README.rst
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5604 2022-11-18 21:52:58.000000 aerospike-8.0.0/Releases.md
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        6 2022-11-18 21:52:58.000000 aerospike-8.0.0/VERSION
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1122 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/.build.yml
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       43 2022-11-07 20:38:50.000000 aerospike-8.0.0/aerospike-client-c/.git
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/.github/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/.github/workflows/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      787 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/.github/workflows/build.yml
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2872 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/.github/workflows/codeql.yml
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      809 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      466 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/.gitmodules
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    51706 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/LICENSE.md
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11774 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6275 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/README.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      217 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8913 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/README.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      175 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_batch_get/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_batch_get/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_batch_get/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_batch_get/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8088 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_batch_get/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5704 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_get/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_get/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_get/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_get/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5487 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_get/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_query/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_query/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_query/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_query/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7695 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_query/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_scan/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_scan/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_scan/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_scan/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5911 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_scan/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      241 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/append/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/append/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/append/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/append/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4968 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/append/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/expire/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/expire/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/expire/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/expire/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3846 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/expire/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/generation/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/generation/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/generation/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/generation/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6580 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/generation/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/get/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/get/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/get/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/get/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6015 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/get/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/incr/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/incr/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/incr/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/incr/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6231 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/incr/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/list/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/list/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/list/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/list/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3845 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/list/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/map/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/map/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/map/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/map/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5646 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/map/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/put/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/put/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/put/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/put/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5941 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/put/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/touch/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/touch/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/touch/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/touch/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3818 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/touch/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/udf/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/udf/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/udf/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/udf/src/lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      569 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/udf/src/lua/basic_udf.lua
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/udf/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5663 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/basic_examples/udf/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/batch_examples/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       52 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/batch_examples/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/batch_examples/get/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/batch_examples/get/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/batch_examples/get/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/batch_examples/get/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24403 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/batch_examples/get/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       77 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   296047 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/geospatial_simple.png
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      291 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/lua/geo_filter_amen.lua
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6792 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/simple/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/simple/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   296047 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/simple/geospatial_simple.png
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/simple/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/simple/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5893 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/simple/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/project/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5789 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/examples/project/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       80 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/aggregate/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/aggregate/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/aggregate/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/aggregate/src/lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2260 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/aggregate/src/lua/query_udf.lua
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/aggregate/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10504 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/aggregate/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/simple/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/simple/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/simple/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/simple/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10407 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/query_examples/simple/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       83 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/background/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/background/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/background/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/background/src/lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      232 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/background/src/lua/bg_scan_udf.lua
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/background/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5591 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/background/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/standard/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/standard/Makefile
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/standard/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/standard/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14104 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/scan_examples/standard/src/main/example.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/utils/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/utils/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/utils/src/include/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3723 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/examples/utils/src/include/example_utils.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/examples/utils/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25877 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/examples/utils/src/main/example_utils.c
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      297 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/install_libev
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      343 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/install_libevent
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      312 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/install_libuv
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       72 2022-11-07 20:38:51.000000 aerospike-8.0.0/aerospike-client-c/modules/common/.git
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      177 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5469 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      382 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/README.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/project/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1293 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/project/rules.mk
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6371 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/project/settings.mk
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2379 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/project/test.mk
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3631 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_aerospike.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1094 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arch.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30555 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arraylist.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4983 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arraylist_iterator.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4471 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19937 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic_gcc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21016 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic_win.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5129 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_boolean.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1624 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_buffer.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4278 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_buffer_pool.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25884 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_bytes.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2398 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_dir.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6037 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_double.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8041 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_geojson.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3038 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_hashmap.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2146 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_hashmap_iterator.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6383 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_integer.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3093 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_iterator.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    41289 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_list.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1153 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_list_iterator.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4878 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_log.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2434 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_log_macros.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11807 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_map.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1140 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_map_iterator.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6909 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_module.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1690 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_monitor.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7740 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1745 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack_ext.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1251 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack_serializer.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1717 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_nil.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10358 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_orderedmap.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4157 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_pair.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2263 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_password.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4866 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_queue.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5402 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_queue_mt.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3547 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_random.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20805 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_rec.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2014 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_result.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3307 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_serializer.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      864 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_sleep.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1168 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_std.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5935 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_stream.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9270 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_string.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3928 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_string_builder.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6804 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_stringmap.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1390 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_thread.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2259 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_thread_pool.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2544 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_timer.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1325 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_types.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1137 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_udf_context.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1535 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_util.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5016 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_val.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4588 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_vector.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      873 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/ssl_util.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2443 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/alloc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2081 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_b64.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3749 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_byte_order.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10776 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_clock.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2074 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_crypto.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2920 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_digest.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7770 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_hash_math.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6994 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_ll.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5020 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_queue.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1129 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_random.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1446 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_aerospike.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12643 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10838 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_hooks.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2564 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_iterator.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2035 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_iterator_hooks.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2670 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_boolean.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1183 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_buffer.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3660 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_buffer_pool.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14188 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_bytes.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2222 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_double.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4041 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_geojson.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2171 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_integer.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1415 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_iterator.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3838 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_list.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1166 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_log.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3742 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_map.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2469 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_module.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    64367 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1699 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack_ext.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5208 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack_serializer.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1378 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_nil.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14070 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_orderedmap.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2322 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_pair.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3348 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_password.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5196 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_queue.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3249 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_queue_mt.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2677 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_random.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1948 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_rec.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2910 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_result.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1640 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_serializer.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1152 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_stream.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5303 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_string.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4878 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_string_builder.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3492 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_thread_pool.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2098 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_timer.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6169 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_val.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2748 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_vector.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    31923 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/crypt_blowfish.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1009 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/crypt_blowfish.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11607 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/ssl_util.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2514 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_alloc.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9521 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_b64.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1516 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_clock.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18498 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_crypto.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      787 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_digest.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7281 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_ll.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14585 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_queue.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3868 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_random.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      573 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/common.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/msgpack/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15140 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/msgpack/msgpack_direct.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4937 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/msgpack/msgpack_rountrip.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10169 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/test.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10446 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/test.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2792 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/test_common.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1187 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/test_common.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1295 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/password.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1942 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/random.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4142 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/string_builder.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14955 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_arraylist.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3410 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_boolean.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5926 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_bytes.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1369 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_double.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11516 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_hashmap.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1652 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_integer.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1106 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_nil.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13133 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_orderedmap.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4845 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_queue.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5054 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_queue_mt.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1115 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_string.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13044 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common/aerospike-common.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16004 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common/aerospike-common.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6869 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/aerospike-common-test.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3692 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/aerospike-common-test.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1555 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common.sln
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/props/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1668 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/props/base.props
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      784 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/vs/props/test.props
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/xcode/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common-test.xcodeproj/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20945 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common-test.xcodeproj/project.pbxproj
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcodeproj/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    32074 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcodeproj/project.pbxproj
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcworkspace/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      246 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcworkspace/contents.xcworkspacedata
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcworkspace/xcshareddata/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      238 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       69 2022-11-07 20:38:51.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/.git
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       52 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1086 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/.travis.yml
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7495 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/CMakeLists.txt
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1528 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/COPYRIGHT
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7907 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/HISTORY
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3868 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/INSTALL
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3695 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1478 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/README.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/cmake/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4014 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/cmake/FindLua.cmake
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1036 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/cmake/FindReadline.cmake
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13372 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/cmake/dist.cmake
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11671 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/cmake/lua.cmake
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      307 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/dist.info
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22482 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/contents.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3305 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/cover.png
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4232 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/logo.gif
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3619 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/lua.1
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1306 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/lua.css
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3951 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/lua.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3617 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/luac.1
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3896 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/luac.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      341 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/manual.css
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   254745 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/manual.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      834 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/doc/readme.html
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      912 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      972 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/README
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      678 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/all.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      191 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/lua.hpp
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   116114 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/lua.ico
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      658 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/lua.pc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   119793 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/lua_lang.ico
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1070 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/luavs.bat
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      800 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/min.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1253 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/noparser.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      928 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/etc/strict.lua
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6087 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22708 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lapi.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      262 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lapi.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17417 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lauxlib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5777 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lauxlib.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17045 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lbaselib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21170 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lcode.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2750 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lcode.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10092 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldblib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16840 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldebug.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1061 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldebug.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14892 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldo.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1897 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldo.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3114 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldump.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4618 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lfunc.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1125 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lfunc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20053 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lgc.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3159 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lgc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      765 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/linit.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13466 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/liolib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12501 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/llex.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2177 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/llex.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2349 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/llimits.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5831 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lmathlib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2172 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lmem.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1494 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lmem.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19216 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/loadlib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21481 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/loadlib_rel.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5498 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lobject.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8502 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lobject.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2884 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lopcodes.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8086 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lopcodes.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5992 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/loslib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    36696 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lparser.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2261 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lparser.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5674 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5011 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstate.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3110 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstring.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      814 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstring.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23561 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstrlib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16263 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltable.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1184 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltable.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7343 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltablib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1650 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltm.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1018 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltm.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10163 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2156 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua.def
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11688 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      818 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua.rc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      774 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua_dll.rc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4661 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/luac.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       27 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/luac.rc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21650 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/luaconf.h.in
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22299 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/luaconf.h.orig
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1026 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lualib.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4629 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lundump.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      890 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lundump.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23242 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lvm.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1159 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lvm.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1628 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lzio.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1556 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/lzio.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4944 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/print.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      391 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/src/wmain.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1177 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/README
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      645 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/bisect.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      293 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/cf.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       80 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/echo.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      181 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/env.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      707 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/factorial.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      605 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/fib.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      254 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/fibfor.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      418 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/globals.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       86 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/hello.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2635 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/life.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      234 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/luac.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      169 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/printf.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      260 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/readonly.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      774 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/sieve.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1494 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/sort.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      283 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/table.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      749 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/trace-calls.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      728 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/trace-globals.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      364 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/lua/test/xd.lua
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       72 2022-11-07 20:38:51.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/.git
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       74 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1116 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/.travis.yml
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11387 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/CMakeLists.txt
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2932 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/COPYRIGHT
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5514 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      441 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/README.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/cmake/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4014 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/cmake/FindLua.cmake
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1036 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/cmake/FindReadline.cmake
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13372 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/cmake/dist.cmake
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11725 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/cmake/lua.cmake
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      425 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dist.info
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2514 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/bluequad-print.css
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5575 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/bluequad.css
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    42898 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/changes.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2762 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/contact.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5991 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_c_api.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10285 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21296 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_api.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    53100 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_semantics.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22506 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_tutorial.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5821 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_jit.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15232 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/extensions.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7634 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/faq.html
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/img/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1340 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/img/contact.png
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22841 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/install.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7910 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/luajit.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13567 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/running.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3900 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/status.html
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13423 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_arm.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34483 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_arm.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12200 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_mips.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28080 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_mips.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12110 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_ppc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    37064 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_ppc.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2062 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_proto.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      568 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x64.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15309 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x86.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    58755 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x86.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30989 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dynasm.lua
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/etc/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2339 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/etc/luajit.1
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   105524 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/etc/luajit.ico
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      592 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/etc/luajit.pc
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       84 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21913 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13782 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/Makefile.dep
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       31 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      193 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/README
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12936 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2561 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8263 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_asm.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6473 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_fold.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10654 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_lib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11357 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_peobj.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11962 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/genminilua.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   174364 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/minilua.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       10 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5606 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/bc.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18123 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/bcsave.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19364 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_arm.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13222 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_mips.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      710 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_mipsel.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20319 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_ppc.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      707 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_x64.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    29330 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_x86.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19509 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dump.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5614 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/v.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6006 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lauxlib.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8916 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_aux.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17039 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_base.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1858 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_bit.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9503 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_debug.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22512 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_ffi.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1322 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_init.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13606 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_io.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17654 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_jit.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6190 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_math.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4121 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_os.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17881 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_package.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20010 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_package_rel.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25059 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_string.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7655 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_table.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      383 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj.supp
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    40401 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_alloc.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      330 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_alloc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28933 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_api.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11305 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_arch.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    57315 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      356 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    75575 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm_arm.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    65652 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm_mips.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    70831 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm_ppc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    93623 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm_x86.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      261 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_bc.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8223 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_bc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1936 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_bcdump.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13412 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_bcread.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11396 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_bcwrite.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9958 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_carith.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      674 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_carith.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27435 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ccall.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4125 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ccall.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18816 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ccallback.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      631 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ccallback.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24352 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cconv.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2025 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cconv.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8616 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cdata.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2079 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cdata.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1980 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_char.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1437 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_char.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10343 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_clib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      754 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_clib.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    56601 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cparse.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2187 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cparse.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    53529 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_crecord.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1384 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_crecord.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18135 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ctype.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16925 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ctype.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16801 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_debug.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1794 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_debug.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10277 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_def.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15075 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_dispatch.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4351 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_dispatch.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10779 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_emit_arm.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6087 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_emit_mips.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6999 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_emit_ppc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11905 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_emit_x86.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23531 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_err.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1496 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_err.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7953 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_errmsg.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      364 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ff.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27854 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ffrecord.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      637 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ffrecord.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5811 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_frame.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5689 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_func.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      776 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_func.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    26326 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_gc.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4913 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_gc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21506 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_gdbjit.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      464 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_gdbjit.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13568 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ir.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17621 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ir.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8845 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ircall.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5929 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_iropt.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15241 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_jit.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12685 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_lex.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3082 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_lex.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6275 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_lib.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3613 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_lib.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4093 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_load.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9866 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_mcode.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      691 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_mcode.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14446 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_meta.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1455 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_meta.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      956 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_obj.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30508 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_obj.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1953 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_dce.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    62422 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_fold.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15208 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_loop.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30785 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_mem.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25427 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_narrow.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7060 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_sink.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23291 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_split.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    80370 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_parse.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      417 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_parse.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    74537 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_record.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1578 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_record.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27816 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_snap.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      921 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_snap.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8820 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_state.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1045 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_state.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9720 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_str.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1719 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_str.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15361 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_strscan.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1088 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_strscan.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18063 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_tab.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2370 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_tab.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5953 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7243 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target_arm.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7438 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target_mips.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7517 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target_ppc.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10064 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target_x86.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23430 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_trace.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1505 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_trace.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2103 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_traceerr.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      848 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_udata.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      307 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_udata.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3466 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_vm.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1515 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_vmevent.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1571 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_vmevent.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3212 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_vmmath.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2300 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/ljamalg.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2156 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lua.def
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11964 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lua.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      135 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lua.hpp
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3863 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luaconf.h.in
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4762 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luaconf.h.orig
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14802 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luajit.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2573 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luajit.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      783 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luajit.rc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1113 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lualib.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3591 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/msvcbuild.bat
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3219 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/ps4build.bat
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   122956 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_arm.dasc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   118591 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_mips.dasc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   138458 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_ppc.dasc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   104315 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_ppcspe.dasc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   169692 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_x86.dasc
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      391 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/wmain.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3135 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/luajit/src/xedkbuild.bat
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       73 2022-11-07 20:38:51.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/.git
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      170 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5822 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/Makefile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2105 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/README.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/project/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4878 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/project/modules.mk
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1773 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/project/rules.mk
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6442 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/project/settings.mk
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2945 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/project/test.mk
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      917 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      971 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_aerospike.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      943 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_bytes.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1095 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_config.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      956 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_geojson.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1064 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_iterator.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      936 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_list.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      928 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_map.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      938 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_record.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1138 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_reg.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      913 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_stream.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1639 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_val.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      996 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/internal.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      973 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/internal.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    31971 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6744 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_aerospike.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    40461 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_bytes.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4039 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_geojson.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4074 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_iterator.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10473 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_list.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9484 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_map.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9217 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_record.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2027 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_reg.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5170 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_stream.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8157 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_system.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6496 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_val.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/hash/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6699 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/hash/hash_udf.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/list/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18321 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/list/list_udf.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      898 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/aggr.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      672 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/basics.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      572 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/bytes.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       44 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/errors.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1021 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/integers.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2427 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/lists.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      199 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/logs.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1159 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/maps.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      271 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/raj.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2038 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/records.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      444 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/strings.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5093 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1106 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_bytes.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       82 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_math.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1314 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_unit.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       11 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_1.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       19 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_2.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       33 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_3.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        8 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_4.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       32 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_5.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       47 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_6.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      978 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/mod_lua_test.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/record/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3317 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/record/record_udf.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/stream/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8876 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/stream/stream_udf.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11134 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/test.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9934 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/test.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2031 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/consumer_stream.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1354 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/consumer_stream.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3249 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/map_rec.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1046 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/map_rec.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1989 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/producer_stream.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1342 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/producer_stream.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3216 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_aerospike.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1395 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_aerospike.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1167 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_logger.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      740 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_logger.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/validation/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4520 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/validation/validation_basics.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6199 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/aerospike-mod-lua.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4105 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/aerospike-mod-lua.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6443 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/aerospike-mod-lua-test.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3296 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/aerospike-mod-lua-test.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1561 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua.sln
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/props/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1792 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/props/base.props
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1080 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/props/test.props
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua-test.xcodeproj/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22363 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua-test.xcodeproj/project.pbxproj
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcodeproj/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15468 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcodeproj/project.pbxproj
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      248 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/contents.xcworkspacedata
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      238 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1711 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/aerospike-mod-lua.xcscmblueprint
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1657 2022-11-02 22:15:10.000000 aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/mod-lua.xcscmblueprint
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/pkg/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3107 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/pkg/README.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/pkg/deb/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      248 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/pkg/deb/client-devel.spec
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      245 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/pkg/deb/client.spec
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       86 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/pkg/deb/postinst.client
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     1149 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/pkg/install
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     2404 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/pkg/package
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      849 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/pkg/package_src
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     3579 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/pkg/package_type
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     1215 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/pkg/platform
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/pkg/rpm/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      515 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/pkg/rpm/client-devel.spec
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      466 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/pkg/rpm/client.spec
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      934 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/pkg/set_version
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      181 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/pkg/version
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/project/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   100746 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/project/doxyfile
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6735 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/project/modules.mk
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1809 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/project/rules.mk
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4856 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/project/settings.mk
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3768 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/project/test.mk
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/apidocs/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      447 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/apidocs/footer.html
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1574 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/apidocs/header.html
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/apidocs/html/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14165 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/apidocs/html/aerospike.css
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12830 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/apidocs/html/aerospike_logo.png
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7716 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/apidocs/html/style.css
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5855 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/apidocs/layout.xml
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20950 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/apidocs/old.css
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/include/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11784 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    31849 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_batch.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10825 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_index.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9662 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_info.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25117 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_key.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15106 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_query.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19703 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_scan.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5598 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_stats.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7824 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_udf.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2793 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_address.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12411 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_admin.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8396 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_async.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1421 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_async_proto.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5711 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_batch.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3972 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_bin.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18835 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_bit_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9337 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cdt_ctx.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1949 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cdt_internal.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2118 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cdt_order.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12107 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cluster.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17605 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_command.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    29752 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_config.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3862 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_conn_pool.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2284 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cpu.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8003 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_error.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16841 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_event.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20430 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_event_internal.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   112090 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_exp.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3751 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_exp_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11785 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_hll_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2362 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_host.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3732 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_info.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3999 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_job.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17540 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_key.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    55064 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_list_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4178 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_listener.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2679 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_lookup.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    49603 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_map_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11719 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_node.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22970 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3535 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_partition.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4348 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_partition_filter.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4975 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_partition_tracker.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2049 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_peers.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2137 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_pipe.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    45114 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_policy.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3941 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_poll.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5183 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_proto.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22234 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_query.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2429 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_query_validate.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28254 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_record.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6296 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_record_iterator.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15069 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_scan.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8095 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_shm_cluster.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6151 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_socket.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10213 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_status.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2019 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_tls.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6161 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_udf.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      164 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/include/aerospike/version.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/main/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       10 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4517 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/_bin.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7550 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/_bin.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9621 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    96053 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_batch.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6828 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_index.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4839 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_info.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    37314 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_key.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    63890 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_query.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    40887 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_scan.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6374 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_stats.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10071 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_udf.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2264 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_address.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34722 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_admin.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3223 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_async.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1979 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_batch.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6287 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_bit_operations.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4093 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_cdt_ctx.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3413 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_cdt_internal.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    41876 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_cluster.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    39520 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_command.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7718 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_config.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4877 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_error.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    52102 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23740 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event_ev.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30015 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event_event.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1443 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event_none.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    38081 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event_uv.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11460 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_exp.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2138 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_exp_operations.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4012 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_hll_operations.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1964 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_host.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10580 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_info.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5020 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_job.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6843 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_key.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19919 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_list_operations.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14169 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_lookup.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21378 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_map_operations.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    36389 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_node.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7413 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_operations.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14774 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_partition.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16623 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_partition_tracker.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7875 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_peers.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14327 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_pipe.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2116 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_policy.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3768 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_proto.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6742 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_query.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8178 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_query_validate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12311 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_record.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4152 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_record_hooks.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2697 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_record_iterator.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4163 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_scan.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34140 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_shm_cluster.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12158 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_socket.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    33826 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_tls.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4929 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_udf.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       42 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/main/aerospike/version.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_batch/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20999 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_batch/batch.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11598 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_batch/batch_async.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_bit/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    47496 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_bit/bit.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_geo/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    32114 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_geo/query_geospatial.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    54410 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_geo/starbucks_3k.jpg
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_index/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6562 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_index/index_basics.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_info/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3972 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_info/info_basics.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24384 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/hll_operate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8311 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_apply.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18867 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_apply2.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3994 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_apply_async.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23755 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_basics.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13329 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_basics_async.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10979 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_operate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7165 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_pipeline.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_list/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    86863 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_list/list_basics.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4291 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_list/list_basics_async.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    86671 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_basics.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5146 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_basics_async.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5193 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_index.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21400 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_sort.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5059 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_udf.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_query/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4956 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_query/query_async.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12322 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_query/query_background.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    40582 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_query/query_foreach.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_scan/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      813 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_scan/aerospike_scan_test.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14203 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_scan/scan_async.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    35392 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_scan/scan_basics.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11230 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_test.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      818 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_test.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_udf/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4436 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_udf/udf_basics.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9444 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_udf/udf_record.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12421 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/aerospike_udf/udf_types.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23591 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/exp_operate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    65950 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/filter_exp.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3235 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/client_record_basics.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2428 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/client_record_lists.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4247 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/client_stream_ads.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      900 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/client_stream_simple.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      971 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/key_apply.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1530 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/key_apply2.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      828 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/query_background.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       40 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/udf_basics.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1020 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/udf_record.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1099 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/lua/udf_types.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12885 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/test.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12799 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/test.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1945 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/consumer_stream.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1353 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/consumer_stream.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1142 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/index_util.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      837 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/index_util.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2165 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/info_helper.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1015 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/info_helper.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1699 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/log_helper.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1068 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/log_helper.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3255 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/map_rec.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1045 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/map_rec.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1844 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/producer_stream.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1341 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/producer_stream.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2392 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/test_aerospike.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1053 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/test_aerospike.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4128 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/udf.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1212 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/src/test/util/udf.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1494 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/README.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    33421 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike/aerospike.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34018 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike/aerospike.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5874 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c-libevent.nuspec
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1890 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c-libevent.targets
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5828 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c-libuv.nuspec
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1866 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c-libuv.targets
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4307 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c.nuspec
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1817 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c.targets
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-test/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16219 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-test/aerospike-test.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7295 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-test/aerospike-test.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike-test/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    43293 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/aerospike.sln
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/append/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12529 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/append/append.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1341 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/append/append.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/append/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-batch-get/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12545 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-batch-get/async-batch-get.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1350 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-batch-get/async-batch-get.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-batch-get/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-delay-queue/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12551 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-delay-queue/async-delay-queue.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1352 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-delay-queue/async-delay-queue.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-delay-queue/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-get/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12534 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-get/async-get.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1344 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-get/async-get.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-get/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-query/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12538 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-query/async-query.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1346 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-query/async-query.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-query/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-scan/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12537 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-scan/async-scan.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1345 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-scan/async-scan.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/async-scan/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/batch-get/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12528 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/batch-get/batch-get.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/batch-get/batch-get.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/batch-get/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/expire/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12529 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/expire/expire.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1341 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/expire/expire.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/expire/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/generation/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12537 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/generation/generation.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1345 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/generation/generation.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/generation/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/geo-filter/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12537 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/geo-filter/geo-filter.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1346 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/geo-filter/geo-filter.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/geo-filter/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/geo-simple/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12537 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/geo-simple/geo-simple.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1346 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/geo-simple/geo-simple.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/geo-simple/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/get/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11967 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/get/get.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/get/get.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/get/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/incr/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12717 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/incr/incr.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1339 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/incr/incr.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/incr/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/list/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12525 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/list/list.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1339 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/list/list.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/list/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/map/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12523 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/map/map.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/map/map.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/map/packages.config
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/put/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/put/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12523 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/put/put.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/put/put.vcxproj.filters
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/query/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/query/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12528 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/query/query.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1341 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/query/query.vcxproj.filters
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/query-aggregate/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/query-aggregate/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12540 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/query-aggregate/query-aggregate.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1344 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/query-aggregate/query-aggregate.vcxproj.filters
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/scan/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/scan/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12528 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/scan/scan.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1342 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/scan/scan.vcxproj.filters
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/scan-background/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/scan-background/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12540 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/scan-background/scan-background.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1344 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/scan-background/scan-background.vcxproj.filters
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/touch/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/touch/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12527 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/touch/touch.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1340 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/touch/touch.vcxproj.filters
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/udf/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/udf/packages.config
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12523 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/udf/udf.vcxproj
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/examples/udf/udf.vcxproj.filters
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2434 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/icon.png
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/vs/props/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1450 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/props/base.props
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      979 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/props/example.props
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      580 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/props/libevent.props
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      566 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/props/libuv.props
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      676 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/vs/props/nodejs.props
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/xcode/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/xcode/aerospike-test.xcodeproj/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    42615 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/xcode/aerospike-test.xcodeproj/project.pbxproj
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/xcode/aerospike.xcodeproj/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    95445 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/xcode/aerospike.xcodeproj/project.pbxproj
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/xcode/client.xcworkspace/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      303 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/xcode/client.xcworkspace/contents.xcworkspacedata
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/xcode/client.xcworkspace/xcshareddata/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      238 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/xcode/client.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2685 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/xcode/client.xcworkspace/xcshareddata/client.xcscmblueprint
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike-client-c/xcode/examples.xcodeproj/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   123173 2022-11-18 21:59:38.000000 aerospike-8.0.0/aerospike-client-c/xcode/examples.xcodeproj/project.pbxproj
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      525 2022-11-02 22:15:07.000000 aerospike-8.0.0/aerospike-client-c/xcode/prepare_xcode
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike.egg-info/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4962 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike.egg-info/PKG-INFO
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    65351 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike.egg-info/SOURCES.txt
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        1 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike.egg-info/dependency_links.txt
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        1 2022-10-24 19:47:51.000000 aerospike-8.0.0/aerospike.egg-info/not-zip-safe
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       28 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike.egg-info/top_level.txt
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike_helpers/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      734 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/__init__.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike_helpers/awaitable/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      734 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/awaitable/__init__.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3924 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/awaitable/io.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike_helpers/batch/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      734 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/batch/__init__.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12118 2022-11-18 21:52:58.000000 aerospike-8.0.0/aerospike_helpers/batch/records.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9292 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/cdt_ctx.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike_helpers/expressions/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1314 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/expressions/__init__.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13243 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/expressions/arithmetic.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    29487 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/expressions/base.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27441 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/expressions/bitwise.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8403 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/expressions/bitwise_operators.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11051 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/expressions/hll.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    45732 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/expressions/list.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    52855 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/expressions/map.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6237 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/expressions/resources.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/aerospike_helpers/operations/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      734 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/operations/__init__.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22701 2022-11-18 19:38:45.000000 aerospike-8.0.0/aerospike_helpers/operations/bitwise_operations.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4141 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/operations/expression_operations.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11877 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/operations/hll_operations.py
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)    43876 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/operations/list_operations.py
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)    44530 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/operations/map_operations.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4299 2022-11-18 19:38:44.000000 aerospike-8.0.0/aerospike_helpers/operations/operations.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      181 2022-10-18 16:08:06.000000 aerospike-8.0.0/api-changes.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/benchmarks/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1664 2022-10-10 17:42:29.000000 aerospike-8.0.0/benchmarks/README.rst
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4563 2022-11-07 23:19:07.000000 aerospike-8.0.0/benchmarks/keygen.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11901 2022-11-07 23:19:07.000000 aerospike-8.0.0/benchmarks/kvs.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/doc/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       19 2022-11-18 19:38:44.000000 aerospike-8.0.0/doc/.gitignore
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      652 2022-11-18 19:38:44.000000 aerospike-8.0.0/doc/README.md
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/doc/_static/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      374 2022-10-10 17:42:29.000000 aerospike-8.0.0/doc/_static/theme_overrides.css
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    43304 2022-11-18 21:52:58.000000 aerospike-8.0.0/doc/aerospike.rst
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      464 2022-11-18 19:38:44.000000 aerospike-8.0.0/doc/aerospike_helpers.batch.rst
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      275 2022-10-10 17:42:29.000000 aerospike-8.0.0/doc/aerospike_helpers.cdt_ctx.rst
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7618 2022-11-18 19:38:44.000000 aerospike-8.0.0/doc/aerospike_helpers.expressions.rst
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     1511 2022-10-14 17:17:55.000000 aerospike-8.0.0/doc/aerospike_helpers.operations.rst
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      709 2022-10-14 18:08:50.000000 aerospike-8.0.0/doc/aerospike_helpers.rst
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)   102000 2022-11-18 21:52:58.000000 aerospike-8.0.0/doc/client.rst
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     8111 2022-11-18 19:38:44.000000 aerospike-8.0.0/doc/conf.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5280 2022-10-14 18:08:50.000000 aerospike-8.0.0/doc/data_mapping.rst
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/doc/examples/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      321 2022-10-14 18:08:50.000000 aerospike-8.0.0/doc/examples/batch_apply.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      903 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/batch_apply.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      627 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/batch_get_ops.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1187 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/batch_operate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      733 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/batch_remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1754 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/batch_write.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      463 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/boilerplate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      337 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/exists.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      602 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/exists_many.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/doc/examples/expressions/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1737 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/expressions/top.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      422 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/get.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1091 2022-11-18 19:35:41.000000 aerospike-8.0.0/doc/examples/get_cdtctx_base64.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      196 2022-10-17 21:20:29.000000 aerospike-8.0.0/doc/examples/get_expression_base64.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      117 2022-10-14 18:08:50.000000 aerospike-8.0.0/doc/examples/get_key_digest.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      735 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/get_many.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1438 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/keyordereddict.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/doc/examples/lua/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1655 2022-10-14 18:08:50.000000 aerospike-8.0.0/doc/examples/lua/example.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1157 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/lua/lua.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      760 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/operate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      658 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/operate_ordered.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      316 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/put.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/doc/examples/query/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1098 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/query/boilerplate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      465 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/query/foreach.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      513 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/query/foreachfalse.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      256 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/query/results.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      378 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      224 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/remove_bin.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      499 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/select.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      891 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/select_many.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2056 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/serializer.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      353 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/touch.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      447 2022-11-07 23:19:07.000000 aerospike-8.0.0/doc/examples/truncate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12584 2022-11-18 19:38:44.000000 aerospike-8.0.0/doc/exception.rst
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     3447 2022-10-14 18:08:50.000000 aerospike-8.0.0/doc/geojson.rst
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     2828 2022-11-10 18:17:46.000000 aerospike-8.0.0/doc/index.rst
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      670 2022-10-14 18:08:50.000000 aerospike-8.0.0/doc/key_ordered_dict.rst
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12176 2022-10-14 18:08:50.000000 aerospike-8.0.0/doc/predicates.rst
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)    22480 2022-11-18 19:38:44.000000 aerospike-8.0.0/doc/query.rst
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      113 2022-11-18 19:38:44.000000 aerospike-8.0.0/doc/requirements.txt
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)    23184 2022-11-18 19:38:44.000000 aerospike-8.0.0/doc/scan.rst
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/examples/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/examples/admin/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4216 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/change_password.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3867 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/create_role.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3880 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/admin/create_user.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3756 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/drop_role.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3756 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/drop_user.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3931 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/grant_privileges.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3922 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/grant_roles.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3922 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/admin/query_role.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3772 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/query_roles.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3877 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/admin/query_user.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3883 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/admin/query_user_info.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3778 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/admin/query_users.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3783 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/admin/query_users_info.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3928 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/revoke_privileges.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3931 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/revoke_roles.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3877 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/admin/set_password.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/examples/client/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6255 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/aggregate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4982 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/append.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4762 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/apply.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      329 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/client/bin_lua.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5141 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/bin_ops.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14832 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/client_big_list.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4957 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/delete.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      343 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/client/example.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4319 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/exists.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4614 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/exists_many.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5216 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/get.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5607 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/get_async.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4335 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/get_key_digest.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4616 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/get_many.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3660 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/get_nodes.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5082 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/increment.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4520 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/index_create.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3893 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/index_remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4640 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/info.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3710 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/info_node.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4278 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/is_connected.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5371 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/kvs.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4924 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/multi_thread.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5367 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/operate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4891 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/prepend.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5161 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/put.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6105 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/put_async.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7258 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/query.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7351 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/query_apply.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4296 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4429 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/remove_bin.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      289 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/client/sample.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4691 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/scan.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5442 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/scan_apply.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5056 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/scan_info.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5826 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/scan_partition.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4631 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/select_many.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4885 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/select_record.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1005 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/client/simple.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       38 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/client/simple_udf.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1282 2022-10-18 23:45:02.000000 aerospike-8.0.0/examples/client/stream_example.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5095 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/touch.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11947 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/ttl.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3792 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/udf_get.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3523 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/udf_list.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3703 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/udf_put.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3627 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/udf_remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7519 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/client/unicode_smiles.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/examples/deprecated/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3067 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/deprecated/exists.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3089 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/deprecated/get.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3770 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/deprecated/put.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2920 2022-11-07 23:19:07.000000 aerospike-8.0.0/examples/deprecated/remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      878 2022-11-18 21:52:58.000000 aerospike-8.0.0/pyproject.toml
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/scripts/
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      625 2022-11-18 19:38:44.000000 aerospike-8.0.0/scripts/manylinux2014build.sh
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      493 2022-10-10 17:42:29.000000 aerospike-8.0.0/scripts/manylinuxbuild.sh
--rwxr-xr-x   0 jnguyen   (1001) jnguyen   (1001)     4543 2022-10-10 17:42:29.000000 aerospike-8.0.0/scripts/os_version
--rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     1055 2022-10-10 17:42:29.000000 aerospike-8.0.0/scripts/wait-for-node.sh
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       38 2022-11-18 23:36:09.000000 aerospike-8.0.0/setup.cfg
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12234 2022-11-18 23:08:32.000000 aerospike-8.0.0/setup.py
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/include/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6478 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/admin.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1255 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/bit_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1223 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/cdt_list_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1218 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/cdt_map_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2827 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/cdt_operation_utils.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      994 2022-10-14 18:08:50.000000 aerospike-8.0.0/src/include/cdt_types.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28201 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/client.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10104 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/conversions.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4750 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/exception_types.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      915 2022-10-14 18:08:50.000000 aerospike-8.0.0/src/include/exceptions.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1151 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/expression_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2215 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/geo.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      943 2022-10-14 18:08:50.000000 aerospike-8.0.0/src/include/global_hosts.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1218 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/hll_operations.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1092 2022-10-14 18:08:50.000000 aerospike-8.0.0/src/include/key_ordered_dict.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1791 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/log.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2934 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/macros.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1546 2022-10-14 18:08:50.000000 aerospike-8.0.0/src/include/module_functions.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      914 2022-10-14 18:08:50.000000 aerospike-8.0.0/src/include/nullobject.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1198 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/operate.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11909 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/policy.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2604 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/policy_config.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1539 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/pool.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      836 2022-10-14 18:08:50.000000 aerospike-8.0.0/src/include/predicates.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4149 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/query.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3710 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/scan.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2531 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/serializer.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      914 2022-10-14 18:08:50.000000 aerospike-8.0.0/src/include/tls_config.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1129 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/tls_info_host.h
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2591 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/include/types.h
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/main/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9253 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/aerospike.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4601 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/calc_digest.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/main/cdt_types/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6639 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/cdt_types/type.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/main/client/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    68407 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/admin.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8078 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/apply.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12209 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/batch_apply.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8964 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/batch_get_ops.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12363 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/batch_operate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10965 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/batch_remove.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21805 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/batch_write.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    33885 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/bit_operate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    63986 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/cdt_list_operate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12527 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/cdt_map_operate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6831 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/cdt_operation_utils.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5399 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/close.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9281 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/connect.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6152 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/exists.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12598 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/exists_many.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4684 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/expression_operations.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6262 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/get.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9137 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/get_async.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4094 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/get_cdtctx_base64.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3377 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/get_expression_base64.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4564 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/get_key_digest.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5173 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/get_key_partition_id.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8863 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/get_many.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12232 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/get_nodes.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18261 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/hll_operate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20058 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/info.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9073 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/info_node.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5243 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/info_random_node.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6187 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/info_single_node.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    54373 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/operate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    32955 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/operate_list.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    50339 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/operate_map.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6913 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/put.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8894 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/put_async.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21747 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/query.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6539 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/remove.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9061 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/remove_bin.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12901 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/scan.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21795 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/sec_index.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8183 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/select.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10407 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/select_many.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5893 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/set_xdr_filter.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2351 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/tls_info_host.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6959 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/truncate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    70532 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/type.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19738 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/client/udf.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    93577 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/conversions.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    69491 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/convert_expressions.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11037 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/convert_partition_filter.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27578 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/exception.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/main/geospatial/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2859 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/geospatial/dumps.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3659 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/geospatial/loads.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12738 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/geospatial/type.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1948 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/geospatial/unwrap.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2085 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/geospatial/wrap.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/main/global_hosts/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3818 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/global_hosts/type.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/main/key_ordered_dict/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2628 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/key_ordered_dict/type.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6293 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/log.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/main/nullobject/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3573 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/nullobject/type.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    52882 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/policy.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21544 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/policy_config.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12517 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/predicates.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/main/query/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3673 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/add_ops.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7041 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/apply.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2893 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/execute_background.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7808 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/foreach.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1654 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/get_parts.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2635 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/paginate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5123 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/results.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3003 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/select.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12774 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/type.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13603 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/query/where.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/src/main/scan/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3377 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/scan/add_ops.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7003 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/scan/apply.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2921 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/scan/execute_background.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8156 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/scan/foreach.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1649 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/scan/get_parts.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2854 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/scan/paginate.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5964 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/scan/results.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3091 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/scan/select.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8840 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/scan/type.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23618 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/serializer.c
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6257 2022-11-18 21:52:58.000000 aerospike-8.0.0/src/main/tls_config.c
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/test/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3186 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/README.md
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      563 2022-11-18 01:37:01.000000 aerospike-8.0.0/test/bin_lua.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       90 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/config.conf
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6265 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/counter26.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        0 2022-10-10 17:42:29.000000 aerospike-8.0.0/test/empty.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      342 2022-11-18 01:38:47.000000 aerospike-8.0.0/test/example.lua
-drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2022-11-18 23:36:09.000000 aerospike-8.0.0/test/new_tests/
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        0 2022-10-10 17:42:29.000000 aerospike-8.0.0/test/new_tests/__init__.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8800 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/as_errors.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      724 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/as_status_codes.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9115 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/conftest.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      686 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/index_helpers.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      358 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/invalid_data.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5343 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_change_password.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12754 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_create_role.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10052 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_create_user.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5023 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_drop_role.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7026 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_drop_user.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2992 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_get_role.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2434 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_get_roles.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6841 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_grant_privileges.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5165 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_grant_roles.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2766 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_query_role.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2200 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_query_roles.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4386 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_query_user.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4538 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_query_user_info.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3253 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_query_users.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3311 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_query_users_info.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8743 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_revoke_privileges.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5972 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_revoke_roles.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3622 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_set_password.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5696 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_set_quotas.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6648 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_admin_set_whitelist.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11624 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_aggregate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15202 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_append.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14128 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_apply.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23970 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_arithmetic_expressions.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7645 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_base_class.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10758 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_batch_apply.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5773 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_batch_get_ops.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8729 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_batch_operate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      779 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_batch_records.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6966 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_batch_remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16455 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_batch_write.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    58814 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_bitwise_operations.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2344 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_bool_config.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2643 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_calc_digest.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4208 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_cdt_compators.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24128 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_cdt_index.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2165 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_close.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3949 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_compress.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6614 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_connect.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1574 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_connect_memleak.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3459 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_data.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2094 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_error_codes.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6034 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_exists.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9563 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_exists_many.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5620 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_expression_operations.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11852 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_expressions_base.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11441 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_expressions_bit.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11009 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_expressions_bitwise_operators.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27036 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_expressions_everywhere.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9473 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_expressions_hll.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    26449 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_expressions_list.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18979 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_expressions_map.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    38095 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_geospatial.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8485 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_get_async.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4233 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_get_cdtctx_base64.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3784 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_get_expression_base64r.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3086 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_get_key_digest.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8406 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_get_many.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1556 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_get_node_names.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1675 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_get_nodes.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28897 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_get_put.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5366 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_get_udf.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16574 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_hll.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16777 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_increment.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19127 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_index.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4910 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_info.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3026 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_info_all.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5547 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_info_random_node.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6955 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_info_single_node.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6845 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_invalid_conf.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8602 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_inverted_map_operations.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2013 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_is_connected.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5281 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_job_info.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3606 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_key_digest.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3516 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_key_ordered_dict_get_by_value.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7480 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_kv.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7807 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_append.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1123 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_basics.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5212 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_clear.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7115 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_extend.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5514 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_get.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6789 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_get_range.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13954 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_index.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8546 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_insert.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9194 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_insert_items.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6144 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_pop.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6928 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_pop_range.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6553 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7364 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_remove_range.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8690 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_set.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5241 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_size.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6754 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_list_trim.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1954 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_log.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22871 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_map_basics.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16677 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_map_operation_helpers.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6726 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_map_write_flags.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3393 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_map_write_mode.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14639 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_mapkeys_index.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13620 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_mapvalues_index.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   185860 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_nested_cdt_ctx.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3406 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_new_constructor.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17566 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_new_list_operation_helpers.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24974 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_new_list_operations.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    43725 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_operate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    31672 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_operate_helpers.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    36122 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_operate_map.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    33960 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_operate_ordered.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      518 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_predicates.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16465 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_prepend.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    26644 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_put_async.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34463 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_query.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17650 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_query_apply.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13129 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_query_execute_background.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15415 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_query_expressions.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5173 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_query_get_partitions_status.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9757 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_query_pagination.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21455 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_query_partition.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14418 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_relative_cdt_operations.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10969 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14665 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_remove_bin.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13228 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_scan.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14839 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_scan_apply.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12500 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_scan_execute_background.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4973 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_scan_get_partitions_status.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11861 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_scan_pagination.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12626 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_scan_partition.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8188 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_select.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12743 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_select_many.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4720 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_set_xdr_filter.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9566 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_touch.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7938 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_truncate.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3511 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_udf_list.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6793 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_udf_put.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6818 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_udf_remove.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11177 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_user_serializer.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14877 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/test_zserializers.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1903 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/new_tests/udf_helpers.py
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       56 2022-10-17 21:26:04.000000 aerospike-8.0.0/test/pytest.ini
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      380 2022-11-18 01:35:24.000000 aerospike-8.0.0/test/query_apply.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      290 2022-11-18 01:35:09.000000 aerospike-8.0.0/test/query_apply_parameters.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       29 2022-10-20 22:44:49.000000 aerospike-8.0.0/test/requirements.txt
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      289 2022-11-18 01:30:51.000000 aerospike-8.0.0/test/sample.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1282 2022-11-18 01:30:28.000000 aerospike-8.0.0/test/stream_example.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3296 2022-11-18 01:30:53.000000 aerospike-8.0.0/test/test_record_udf.lua
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      437 2022-11-18 21:52:58.000000 aerospike-8.0.0/test/tox.ini
--rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       84 2022-11-18 01:30:55.000000 aerospike-8.0.0/test/udf_basic_ops.lua
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.151525 aerospike-9.0.0/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      434 2022-12-17 00:32:42.000000 aerospike-9.0.0/.build.yml
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4734 2022-12-17 00:32:42.000000 aerospike-9.0.0/.clang-format
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/.github/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.995526 aerospike-9.0.0/.github/workflows/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5311 2023-01-04 00:50:37.000000 aerospike-9.0.0/.github/workflows/tests.yml
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3077 2023-01-03 18:24:51.000000 aerospike-9.0.0/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      193 2022-12-17 00:32:42.000000 aerospike-9.0.0/.gitmodules
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4773 2023-01-03 18:18:07.000000 aerospike-9.0.0/BUILD.md
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11357 2022-09-19 18:31:26.000000 aerospike-9.0.0/LICENSE
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      187 2022-12-15 01:59:21.000000 aerospike-9.0.0/MANIFEST.in
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4962 2023-01-04 00:50:47.151525 aerospike-9.0.0/PKG-INFO
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4227 2022-12-17 00:32:42.000000 aerospike-9.0.0/README.rst
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5604 2022-12-17 00:32:42.000000 aerospike-9.0.0/Releases.md
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        6 2023-01-04 00:50:40.000000 aerospike-9.0.0/VERSION
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1122 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/.build.yml
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       43 2022-11-07 20:38:50.000000 aerospike-9.0.0/aerospike-client-c/.git
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/.github/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/.github/workflows/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      787 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/.github/workflows/build.yml
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2872 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/.github/workflows/codeql.yml
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      809 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      466 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/.gitmodules
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    51706 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/LICENSE.md
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11774 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6275 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/README.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      217 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8913 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/README.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      175 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_batch_get/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_batch_get/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_batch_get/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_batch_get/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8088 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_batch_get/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5704 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_get/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_get/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_get/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_get/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5487 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_get/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_query/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_query/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_query/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_query/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7695 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_query/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_scan/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_scan/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_scan/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_scan/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5911 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_scan/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      241 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/append/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/append/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/append/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/append/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4968 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/append/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/expire/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/expire/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/expire/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/expire/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3846 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/expire/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/generation/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/generation/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/generation/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/generation/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6580 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/generation/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/get/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/get/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/get/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/get/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6015 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/get/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/incr/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/incr/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/incr/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/incr/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6231 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/incr/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/list/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/list/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/list/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/list/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3845 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/list/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/map/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/map/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/map/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/map/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5646 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/map/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/put/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/put/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/put/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/put/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5941 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/put/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/touch/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/touch/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/touch/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/touch/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3818 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/touch/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/udf/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/udf/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.983527 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/udf/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.999526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/udf/src/lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      569 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/udf/src/lua/basic_udf.lua
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/udf/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5663 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/basic_examples/udf/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/batch_examples/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       52 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/batch_examples/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/batch_examples/get/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/batch_examples/get/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/examples/batch_examples/get/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/batch_examples/get/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24403 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/examples/batch_examples/get/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       77 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   296047 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/geospatial_simple.png
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      291 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/lua/geo_filter_amen.lua
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6792 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/simple/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/simple/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   296047 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/simple/geospatial_simple.png
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/simple/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/simple/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5893 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/simple/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/project/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5789 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/examples/project/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/query_examples/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       80 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/query_examples/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/query_examples/aggregate/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/query_examples/aggregate/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/examples/query_examples/aggregate/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/query_examples/aggregate/src/lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2260 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/query_examples/aggregate/src/lua/query_udf.lua
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/query_examples/aggregate/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10504 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/query_examples/aggregate/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/query_examples/simple/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/query_examples/simple/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/examples/query_examples/simple/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/query_examples/simple/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10407 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/examples/query_examples/simple/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       83 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/background/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/background/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/background/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/background/src/lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      232 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/background/src/lua/bg_scan_udf.lua
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/background/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5591 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/background/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/standard/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       78 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/standard/Makefile
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/standard/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/standard/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14104 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/examples/scan_examples/standard/src/main/example.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/examples/utils/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/examples/utils/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/utils/src/include/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3723 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/examples/utils/src/include/example_utils.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/examples/utils/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25877 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/examples/utils/src/main/example_utils.c
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      297 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/install_libev
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      343 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/install_libevent
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      312 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/install_libuv
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/modules/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/modules/common/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       72 2022-11-07 20:38:51.000000 aerospike-9.0.0/aerospike-client-c/modules/common/.git
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      177 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5469 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      382 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/README.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.003526 aerospike-9.0.0/aerospike-client-c/modules/common/project/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1293 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/project/rules.mk
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6371 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/project/settings.mk
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2379 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/project/test.mk
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/modules/common/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.011526 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3631 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_aerospike.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1094 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arch.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30555 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arraylist.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4983 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arraylist_iterator.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4471 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19937 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic_gcc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21016 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic_win.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5129 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_boolean.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1624 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_buffer.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4278 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_buffer_pool.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25884 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_bytes.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2398 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_dir.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6037 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_double.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8041 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_geojson.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3038 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_hashmap.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2146 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_hashmap_iterator.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6383 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_integer.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3093 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_iterator.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    41289 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_list.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1153 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_list_iterator.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4878 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_log.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2434 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_log_macros.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11807 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_map.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1140 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_map_iterator.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6909 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_module.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1690 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_monitor.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7740 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1745 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack_ext.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1251 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack_serializer.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1717 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_nil.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10358 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_orderedmap.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4157 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_pair.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2263 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_password.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4866 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_queue.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5402 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_queue_mt.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3547 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_random.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20805 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_rec.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2014 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_result.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3307 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_serializer.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      864 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_sleep.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1168 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_std.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5935 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_stream.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9270 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_string.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3928 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_string_builder.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6804 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_stringmap.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1390 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_thread.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2259 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_thread_pool.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2544 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_timer.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1325 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_types.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1137 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_udf_context.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1535 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_util.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5016 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_val.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4588 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_vector.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      873 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/ssl_util.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.011526 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2443 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/alloc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2081 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_b64.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3749 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_byte_order.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10776 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_clock.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2074 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_crypto.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2920 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_digest.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7770 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_hash_math.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6994 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_ll.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5020 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_queue.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1129 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_random.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.015526 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1446 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_aerospike.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12643 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10838 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_hooks.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2564 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_iterator.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2035 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_iterator_hooks.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2670 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_boolean.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1183 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_buffer.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3660 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_buffer_pool.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14188 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_bytes.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2222 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_double.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4041 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_geojson.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2171 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_integer.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1415 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_iterator.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3838 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_list.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1166 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_log.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3742 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_map.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2469 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_module.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    64367 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1699 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack_ext.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5208 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack_serializer.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1378 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_nil.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14070 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_orderedmap.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2322 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_pair.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3348 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_password.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5196 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_queue.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3249 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_queue_mt.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2677 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_random.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1948 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_rec.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2910 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_result.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1640 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_serializer.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1152 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_stream.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5303 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_string.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4878 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_string_builder.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3492 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_thread_pool.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2098 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_timer.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6169 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_val.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2748 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_vector.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    31923 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/crypt_blowfish.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1009 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/crypt_blowfish.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11607 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/ssl_util.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.019526 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2514 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_alloc.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9521 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_b64.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1516 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_clock.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18498 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_crypto.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      787 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_digest.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7281 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_ll.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14585 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_queue.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3868 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_random.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.019526 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      573 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/common.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.019526 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/msgpack/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15140 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/msgpack/msgpack_direct.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4937 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/msgpack/msgpack_rountrip.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10169 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/test.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10446 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/test.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2792 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/test_common.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1187 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/test_common.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.019526 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1295 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/password.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1942 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/random.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4142 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/string_builder.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14955 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_arraylist.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3410 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_boolean.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5926 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_bytes.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1369 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_double.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11516 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_hashmap.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1652 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_integer.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1106 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_nil.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13133 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_orderedmap.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4845 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_queue.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5054 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_queue_mt.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1115 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_string.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.019526 aerospike-9.0.0/aerospike-client-c/modules/common/vs/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.019526 aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13044 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common/aerospike-common.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16004 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common/aerospike-common.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.019526 aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6869 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/aerospike-common-test.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3692 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/aerospike-common-test.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1555 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common.sln
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.023526 aerospike-9.0.0/aerospike-client-c/modules/common/vs/props/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1668 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/vs/props/base.props
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      784 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/vs/props/test.props
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/modules/common/xcode/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.023526 aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common-test.xcodeproj/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20945 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common-test.xcodeproj/project.pbxproj
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.023526 aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcodeproj/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    32074 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcodeproj/project.pbxproj
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.023526 aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcworkspace/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      246 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcworkspace/contents.xcworkspacedata
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.023526 aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcworkspace/xcshareddata/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      238 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.023526 aerospike-9.0.0/aerospike-client-c/modules/lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       69 2022-11-07 20:38:51.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/.git
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       52 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1086 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/.travis.yml
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7495 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/CMakeLists.txt
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1528 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/COPYRIGHT
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7907 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/HISTORY
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3868 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/INSTALL
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3695 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1478 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/README.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.023526 aerospike-9.0.0/aerospike-client-c/modules/lua/cmake/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4014 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/cmake/FindLua.cmake
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1036 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/cmake/FindReadline.cmake
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13372 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/cmake/dist.cmake
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11671 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/cmake/lua.cmake
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      307 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/dist.info
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.023526 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22482 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/contents.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3305 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/cover.png
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4232 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/logo.gif
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3619 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/lua.1
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1306 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/lua.css
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3951 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/lua.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3617 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/luac.1
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3896 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/luac.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      341 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/manual.css
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   254745 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/manual.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      834 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/doc/readme.html
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.027526 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      912 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      972 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/README
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      678 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/all.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      191 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/lua.hpp
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   116114 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/lua.ico
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      658 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/lua.pc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   119793 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/lua_lang.ico
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1070 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/luavs.bat
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      800 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/min.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1253 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/noparser.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      928 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/etc/strict.lua
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.031526 aerospike-9.0.0/aerospike-client-c/modules/lua/src/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6087 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22708 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lapi.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      262 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lapi.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17417 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lauxlib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5777 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lauxlib.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17045 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lbaselib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21170 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lcode.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2750 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lcode.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10092 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldblib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16840 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldebug.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1061 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldebug.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14892 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldo.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1897 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldo.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3114 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldump.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4618 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lfunc.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1125 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lfunc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20053 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lgc.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3159 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lgc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      765 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/linit.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13466 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/liolib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12501 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/llex.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2177 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/llex.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2349 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/llimits.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5831 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lmathlib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2172 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lmem.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1494 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lmem.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19216 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/loadlib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21481 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/loadlib_rel.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5498 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lobject.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8502 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lobject.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2884 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lopcodes.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8086 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lopcodes.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5992 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/loslib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    36696 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lparser.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2261 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lparser.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5674 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5011 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstate.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3110 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstring.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      814 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstring.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23561 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstrlib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16263 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltable.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1184 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltable.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7343 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltablib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1650 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltm.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1018 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltm.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10163 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2156 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua.def
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11688 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      818 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua.rc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      774 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua_dll.rc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4661 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/luac.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       27 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/luac.rc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21650 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/luaconf.h.in
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22299 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/luaconf.h.orig
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1026 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lualib.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4629 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lundump.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      890 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lundump.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23242 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lvm.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1159 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lvm.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1628 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lzio.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1556 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/lzio.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4944 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/print.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      391 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/src/wmain.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.035526 aerospike-9.0.0/aerospike-client-c/modules/lua/test/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1177 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/README
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      645 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/bisect.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      293 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/cf.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       80 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/echo.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      181 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/env.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      707 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/factorial.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      605 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/fib.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      254 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/fibfor.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      418 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/globals.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       86 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/hello.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2635 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/life.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      234 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/luac.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      169 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/printf.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      260 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/readonly.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      774 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/sieve.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1494 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/sort.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      283 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/table.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      749 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/trace-calls.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      728 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/trace-globals.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      364 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/lua/test/xd.lua
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.035526 aerospike-9.0.0/aerospike-client-c/modules/luajit/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       72 2022-11-07 20:38:51.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/.git
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       74 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1116 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/.travis.yml
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11387 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/CMakeLists.txt
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2932 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/COPYRIGHT
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5514 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      441 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/README.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.035526 aerospike-9.0.0/aerospike-client-c/modules/luajit/cmake/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4014 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/cmake/FindLua.cmake
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1036 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/cmake/FindReadline.cmake
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13372 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/cmake/dist.cmake
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11725 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/cmake/lua.cmake
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      425 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dist.info
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.039526 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2514 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/bluequad-print.css
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5575 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/bluequad.css
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    42898 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/changes.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2762 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/contact.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5991 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_c_api.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10285 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21296 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_api.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    53100 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_semantics.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22506 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_tutorial.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5821 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_jit.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15232 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/extensions.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7634 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/faq.html
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.039526 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/img/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1340 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/img/contact.png
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22841 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/install.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7910 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/luajit.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13567 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/running.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3900 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/status.html
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.039526 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13423 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_arm.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34483 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_arm.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12200 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_mips.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28080 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_mips.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12110 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_ppc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    37064 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_ppc.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2062 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_proto.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      568 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x64.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15309 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x86.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    58755 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x86.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30989 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dynasm.lua
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.039526 aerospike-9.0.0/aerospike-client-c/modules/luajit/etc/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2339 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/etc/luajit.1
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   105524 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/etc/luajit.ico
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      592 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/etc/luajit.pc
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.059526 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       84 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21913 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13782 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/Makefile.dep
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.059526 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       31 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      193 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/README
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12936 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2561 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8263 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_asm.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6473 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_fold.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10654 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_lib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11357 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_peobj.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11962 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/genminilua.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   174364 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/minilua.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.059526 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       10 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5606 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/bc.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18123 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/bcsave.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19364 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_arm.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13222 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_mips.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      710 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_mipsel.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20319 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_ppc.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      707 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_x64.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    29330 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_x86.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19509 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dump.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5614 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/v.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6006 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lauxlib.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8916 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_aux.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17039 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_base.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1858 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_bit.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9503 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_debug.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22512 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_ffi.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1322 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_init.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13606 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_io.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17654 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_jit.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6190 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_math.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4121 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_os.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17881 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_package.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20010 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_package_rel.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25059 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_string.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7655 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_table.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      383 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj.supp
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    40401 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_alloc.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      330 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_alloc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28933 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_api.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11305 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_arch.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    57315 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      356 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    75575 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm_arm.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    65652 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm_mips.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    70831 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm_ppc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    93623 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm_x86.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      261 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_bc.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8223 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_bc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1936 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_bcdump.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13412 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_bcread.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11396 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_bcwrite.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9958 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_carith.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      674 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_carith.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27435 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ccall.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4125 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ccall.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18816 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ccallback.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      631 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ccallback.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24352 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cconv.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2025 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cconv.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8616 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cdata.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2079 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cdata.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1980 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_char.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1437 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_char.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10343 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_clib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      754 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_clib.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    56601 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cparse.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2187 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cparse.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    53529 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_crecord.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1384 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_crecord.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18135 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ctype.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16925 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ctype.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16801 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_debug.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1794 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_debug.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10277 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_def.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15075 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_dispatch.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4351 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_dispatch.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10779 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_emit_arm.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6087 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_emit_mips.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6999 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_emit_ppc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11905 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_emit_x86.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23531 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_err.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1496 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_err.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7953 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_errmsg.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      364 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ff.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27854 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ffrecord.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      637 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ffrecord.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5811 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_frame.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5689 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_func.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      776 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_func.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    26326 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_gc.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4913 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_gc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21506 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_gdbjit.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      464 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_gdbjit.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13568 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ir.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17621 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ir.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8845 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ircall.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5929 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_iropt.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15241 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_jit.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12685 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_lex.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3082 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_lex.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6275 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_lib.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3613 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_lib.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4093 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_load.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9866 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_mcode.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      691 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_mcode.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14446 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_meta.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1455 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_meta.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      956 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_obj.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30508 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_obj.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1953 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_dce.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    62422 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_fold.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15208 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_loop.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30785 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_mem.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25427 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_narrow.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7060 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_sink.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23291 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_split.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    80370 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_parse.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      417 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_parse.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    74537 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_record.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1578 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_record.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27816 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_snap.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      921 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_snap.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8820 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_state.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1045 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_state.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9720 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_str.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1719 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_str.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15361 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_strscan.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1088 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_strscan.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18063 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_tab.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2370 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_tab.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5953 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7243 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target_arm.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7438 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target_mips.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7517 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target_ppc.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10064 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target_x86.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23430 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_trace.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1505 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_trace.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2103 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_traceerr.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      848 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_udata.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      307 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_udata.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3466 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_vm.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1515 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_vmevent.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1571 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_vmevent.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3212 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_vmmath.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2300 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/ljamalg.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2156 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lua.def
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11964 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lua.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      135 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lua.hpp
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3863 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luaconf.h.in
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4762 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luaconf.h.orig
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14802 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luajit.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2573 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luajit.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      783 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luajit.rc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1113 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lualib.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3591 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/msvcbuild.bat
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3219 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/ps4build.bat
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   122956 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_arm.dasc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   118591 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_mips.dasc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   138458 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_ppc.dasc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   104315 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_ppcspe.dasc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   169692 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_x86.dasc
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      391 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/wmain.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3135 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/luajit/src/xedkbuild.bat
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.059526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       73 2022-11-07 20:38:51.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/.git
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      170 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5822 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/Makefile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2105 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/README.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.059526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/project/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4878 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/project/modules.mk
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1773 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/project/rules.mk
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6442 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/project/settings.mk
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2945 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/project/test.mk
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.987527 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.063526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      917 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      971 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_aerospike.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      943 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_bytes.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1095 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_config.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      956 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_geojson.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1064 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_iterator.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      936 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_list.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      928 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_map.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      938 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_record.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1138 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_reg.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      913 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_stream.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1639 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_val.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.063526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      996 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/internal.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      973 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/internal.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    31971 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6744 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_aerospike.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    40461 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_bytes.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4039 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_geojson.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4074 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_iterator.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10473 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_list.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9484 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_map.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9217 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_record.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2027 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_reg.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5170 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_stream.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8157 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_system.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6496 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_val.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.063526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.063526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/hash/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6699 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/hash/hash_udf.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.063526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/list/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18321 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/list/list_udf.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.067526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      898 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/aggr.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      672 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/basics.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      572 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/bytes.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       44 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/errors.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1021 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/integers.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2427 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/lists.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      199 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/logs.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1159 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/maps.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      271 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/raj.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2038 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/records.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      444 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/strings.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5093 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1106 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_bytes.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       82 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_math.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1314 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_unit.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       11 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_1.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       19 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_2.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       33 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_3.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        8 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_4.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       32 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_5.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       47 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/validate_6.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      978 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/mod_lua_test.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.067526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/record/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3317 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/record/record_udf.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.067526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/stream/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8876 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/stream/stream_udf.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11134 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/test.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9934 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/test.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.067526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2031 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/consumer_stream.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1354 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/consumer_stream.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3249 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/map_rec.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1046 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/map_rec.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1989 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/producer_stream.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1342 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/producer_stream.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3216 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_aerospike.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1395 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_aerospike.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1167 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_logger.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      740 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_logger.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.067526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/validation/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4520 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/validation/validation_basics.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.067526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.067526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6199 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/aerospike-mod-lua.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4105 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/aerospike-mod-lua.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6443 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/aerospike-mod-lua-test.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3296 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/aerospike-mod-lua-test.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1561 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua.sln
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/props/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1792 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/props/base.props
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1080 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/props/test.props
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.991526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua-test.xcodeproj/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22363 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua-test.xcodeproj/project.pbxproj
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcodeproj/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15468 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcodeproj/project.pbxproj
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      248 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/contents.xcworkspacedata
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      238 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1711 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/aerospike-mod-lua.xcscmblueprint
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1657 2022-11-02 22:15:10.000000 aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/mod-lua.xcscmblueprint
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/pkg/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3107 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/pkg/README.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/pkg/deb/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      248 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/pkg/deb/client-devel.spec
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      245 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/pkg/deb/client.spec
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       86 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/pkg/deb/postinst.client
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     1149 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/pkg/install
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     2404 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/pkg/package
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      849 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/pkg/package_src
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     3579 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/pkg/package_type
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     1215 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/pkg/platform
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/pkg/rpm/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      515 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/pkg/rpm/client-devel.spec
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      466 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/pkg/rpm/client.spec
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      934 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/pkg/set_version
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      181 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/pkg/version
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/project/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   100746 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/project/doxyfile
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6735 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/project/modules.mk
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1809 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/project/rules.mk
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4856 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/project/settings.mk
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3768 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/project/test.mk
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.991526 aerospike-9.0.0/aerospike-client-c/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/src/apidocs/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      447 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/apidocs/footer.html
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1574 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/apidocs/header.html
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.071526 aerospike-9.0.0/aerospike-client-c/src/apidocs/html/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14165 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/apidocs/html/aerospike.css
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12830 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/apidocs/html/aerospike_logo.png
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7716 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/apidocs/html/style.css
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5855 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/apidocs/layout.xml
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20950 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/apidocs/old.css
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.991526 aerospike-9.0.0/aerospike-client-c/src/include/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.079526 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11784 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    31849 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_batch.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10825 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_index.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9662 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_info.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    25117 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_key.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15106 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_query.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19703 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_scan.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5598 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_stats.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7824 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_udf.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2793 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_address.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12411 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_admin.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8396 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_async.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1421 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_async_proto.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5711 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_batch.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3972 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_bin.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18835 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_bit_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9337 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cdt_ctx.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1949 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cdt_internal.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2118 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cdt_order.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12107 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cluster.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17605 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_command.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    29752 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_config.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3862 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_conn_pool.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2284 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cpu.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8003 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_error.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16841 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_event.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20430 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_event_internal.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   112090 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_exp.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3751 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_exp_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11785 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_hll_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2362 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_host.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3732 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_info.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3999 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_job.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17540 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_key.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    55064 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_list_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4178 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_listener.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2679 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_lookup.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    49603 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_map_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11719 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_node.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22970 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3535 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_partition.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4348 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_partition_filter.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4975 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_partition_tracker.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2049 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_peers.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2137 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_pipe.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    45114 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_policy.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3941 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_poll.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5183 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_proto.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22234 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_query.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2429 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_query_validate.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28254 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_record.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6296 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_record_iterator.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15069 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_scan.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8095 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_shm_cluster.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6151 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_socket.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10213 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_status.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2019 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_tls.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6161 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_udf.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      164 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/src/include/aerospike/version.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.991526 aerospike-9.0.0/aerospike-client-c/src/main/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       10 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4517 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/_bin.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7550 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/_bin.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9621 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    96053 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_batch.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6828 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_index.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4839 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_info.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    37314 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_key.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    63890 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_query.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    40887 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_scan.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6374 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_stats.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10071 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_udf.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2264 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_address.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34722 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_admin.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3223 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_async.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1979 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_batch.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6287 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_bit_operations.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4093 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_cdt_ctx.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3413 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_cdt_internal.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    41876 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_cluster.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    39520 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_command.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7718 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_config.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4877 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_error.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    52102 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23740 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event_ev.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    30015 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event_event.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1443 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event_none.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    38081 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event_uv.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11460 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_exp.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2138 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_exp_operations.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4012 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_hll_operations.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1964 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_host.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10580 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_info.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5020 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_job.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6843 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_key.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19919 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_list_operations.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14169 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_lookup.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21378 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_map_operations.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    36389 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_node.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7413 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_operations.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14774 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_partition.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16623 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_partition_tracker.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7875 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_peers.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14327 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_pipe.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2116 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_policy.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3768 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_proto.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6742 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_query.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8178 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_query_validate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12311 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_record.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4152 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_record_hooks.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2697 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_record_iterator.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4163 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_scan.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34140 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_shm_cluster.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12158 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_socket.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    33826 2022-12-02 21:48:57.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_tls.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4929 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_udf.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       42 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/src/main/aerospike/version.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_batch/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20999 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_batch/batch.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11598 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_batch/batch_async.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_bit/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    47496 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_bit/bit.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_geo/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    32114 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_geo/query_geospatial.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    54410 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_geo/starbucks_3k.jpg
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_index/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6562 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_index/index_basics.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_info/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3972 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_info/info_basics.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24384 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/hll_operate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8311 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_apply.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18867 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_apply2.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3994 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_apply_async.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23755 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_basics.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13329 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_basics_async.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10979 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_operate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7165 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_pipeline.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_list/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    86863 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_list/list_basics.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4291 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_list/list_basics_async.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    86671 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_basics.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5146 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_basics_async.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5193 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_index.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21400 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_sort.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5059 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_udf.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_query/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4956 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_query/query_async.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12322 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_query/query_background.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    40582 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_query/query_foreach.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.087526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_scan/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      813 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_scan/aerospike_scan_test.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14203 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_scan/scan_async.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    35392 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_scan/scan_basics.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11230 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_test.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      818 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_test.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.091526 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_udf/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4436 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_udf/udf_basics.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9444 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_udf/udf_record.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12421 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/aerospike_udf/udf_types.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23591 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/exp_operate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    65950 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/filter_exp.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.091526 aerospike-9.0.0/aerospike-client-c/src/test/lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3235 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/client_record_basics.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2428 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/client_record_lists.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4247 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/client_stream_ads.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      900 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/client_stream_simple.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      971 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/key_apply.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1530 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/key_apply2.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      828 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/query_background.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       40 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/udf_basics.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1020 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/udf_record.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1099 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/lua/udf_types.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12885 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/test.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12799 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/test.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.091526 aerospike-9.0.0/aerospike-client-c/src/test/util/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1945 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/consumer_stream.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1353 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/consumer_stream.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1142 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/index_util.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      837 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/index_util.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2165 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/info_helper.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1015 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/info_helper.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1699 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/log_helper.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1068 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/log_helper.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3255 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/map_rec.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1045 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/map_rec.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1844 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/producer_stream.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1341 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/producer_stream.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2392 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/test_aerospike.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1053 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/test_aerospike.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4128 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/udf.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1212 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/src/test/util/udf.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.091526 aerospike-9.0.0/aerospike-client-c/vs/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1494 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/README.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/aerospike/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    33421 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike/aerospike.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34018 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike/aerospike.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5874 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c-libevent.nuspec
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1890 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c-libevent.targets
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5828 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c-libuv.nuspec
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1866 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c-libuv.targets
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4307 2022-12-15 02:04:35.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c.nuspec
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1817 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c.targets
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/aerospike-test/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16219 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike-test/aerospike-test.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7295 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike-test/aerospike-test.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike-test/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    43293 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/aerospike.sln
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.991526 aerospike-9.0.0/aerospike-client-c/vs/examples/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/append/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12529 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/append/append.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1341 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/append/append.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/append/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/async-batch-get/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12545 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-batch-get/async-batch-get.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1350 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-batch-get/async-batch-get.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-batch-get/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/async-delay-queue/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12551 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-delay-queue/async-delay-queue.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1352 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-delay-queue/async-delay-queue.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-delay-queue/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/async-get/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12534 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-get/async-get.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1344 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-get/async-get.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-get/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/async-query/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12538 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-query/async-query.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1346 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-query/async-query.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-query/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/async-scan/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12537 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-scan/async-scan.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1345 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-scan/async-scan.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/async-scan/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/batch-get/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12528 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/batch-get/batch-get.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/batch-get/batch-get.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/batch-get/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/expire/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12529 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/expire/expire.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1341 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/expire/expire.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/expire/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/generation/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12537 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/generation/generation.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1345 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/generation/generation.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/generation/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/geo-filter/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12537 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/geo-filter/geo-filter.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1346 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/geo-filter/geo-filter.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/geo-filter/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.095526 aerospike-9.0.0/aerospike-client-c/vs/examples/geo-simple/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12537 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/geo-simple/geo-simple.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1346 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/geo-simple/geo-simple.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/geo-simple/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/get/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11967 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/get/get.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/get/get.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/get/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/incr/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12717 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/incr/incr.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1339 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/incr/incr.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/incr/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/list/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12525 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/list/list.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1339 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/list/list.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/list/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/map/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12523 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/map/map.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/map/map.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/map/packages.config
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/put/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/put/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12523 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/put/put.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/put/put.vcxproj.filters
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/query/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/query/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12528 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/query/query.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1341 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/query/query.vcxproj.filters
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/query-aggregate/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/query-aggregate/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12540 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/query-aggregate/query-aggregate.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1344 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/query-aggregate/query-aggregate.vcxproj.filters
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/scan/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/scan/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12528 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/scan/scan.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1342 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/scan/scan.vcxproj.filters
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/scan-background/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/scan-background/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12540 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/scan-background/scan-background.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1344 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/scan-background/scan-background.vcxproj.filters
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/touch/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/touch/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12527 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/touch/touch.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1340 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/touch/touch.vcxproj.filters
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/examples/udf/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      156 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/udf/packages.config
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12523 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/udf/udf.vcxproj
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1338 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/examples/udf/udf.vcxproj.filters
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2434 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/icon.png
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/vs/props/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1450 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/props/base.props
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      979 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/props/example.props
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      580 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/props/libevent.props
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      566 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/props/libuv.props
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      676 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/vs/props/nodejs.props
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/xcode/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.099526 aerospike-9.0.0/aerospike-client-c/xcode/aerospike-test.xcodeproj/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    42615 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/xcode/aerospike-test.xcodeproj/project.pbxproj
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.103526 aerospike-9.0.0/aerospike-client-c/xcode/aerospike.xcodeproj/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    95445 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/xcode/aerospike.xcodeproj/project.pbxproj
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.103526 aerospike-9.0.0/aerospike-client-c/xcode/client.xcworkspace/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      303 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/xcode/client.xcworkspace/contents.xcworkspacedata
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.103526 aerospike-9.0.0/aerospike-client-c/xcode/client.xcworkspace/xcshareddata/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      238 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/xcode/client.xcworkspace/xcshareddata/IDEWorkspaceChecks.plist
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2685 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/xcode/client.xcworkspace/xcshareddata/client.xcscmblueprint
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.103526 aerospike-9.0.0/aerospike-client-c/xcode/examples.xcodeproj/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   123173 2022-11-29 22:02:55.000000 aerospike-9.0.0/aerospike-client-c/xcode/examples.xcodeproj/project.pbxproj
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      525 2022-11-02 22:15:07.000000 aerospike-9.0.0/aerospike-client-c/xcode/prepare_xcode
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.103526 aerospike-9.0.0/aerospike.egg-info/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4962 2023-01-04 00:50:46.000000 aerospike-9.0.0/aerospike.egg-info/PKG-INFO
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    65351 2023-01-04 00:50:46.000000 aerospike-9.0.0/aerospike.egg-info/SOURCES.txt
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        1 2023-01-04 00:50:46.000000 aerospike-9.0.0/aerospike.egg-info/dependency_links.txt
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        1 2022-10-24 19:47:51.000000 aerospike-9.0.0/aerospike.egg-info/not-zip-safe
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       28 2023-01-04 00:50:46.000000 aerospike-9.0.0/aerospike.egg-info/top_level.txt
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.103526 aerospike-9.0.0/aerospike_helpers/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      734 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/__init__.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.103526 aerospike-9.0.0/aerospike_helpers/awaitable/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      734 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/awaitable/__init__.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3924 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/awaitable/io.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.103526 aerospike-9.0.0/aerospike_helpers/batch/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      734 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/batch/__init__.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12118 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/batch/records.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9292 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/cdt_ctx.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.107526 aerospike-9.0.0/aerospike_helpers/expressions/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1314 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/expressions/__init__.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13243 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/expressions/arithmetic.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    29487 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/expressions/base.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27441 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/expressions/bitwise.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8403 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/expressions/bitwise_operators.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11051 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/expressions/hll.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    45732 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/expressions/list.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    52855 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/expressions/map.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6237 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/expressions/resources.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.107526 aerospike-9.0.0/aerospike_helpers/operations/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      734 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/operations/__init__.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22701 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/operations/bitwise_operations.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4141 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/operations/expression_operations.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11877 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/operations/hll_operations.py
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)    43876 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/operations/list_operations.py
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)    44530 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/operations/map_operations.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4299 2022-12-17 00:32:42.000000 aerospike-9.0.0/aerospike_helpers/operations/operations.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      181 2022-10-18 16:08:06.000000 aerospike-9.0.0/api-changes.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.107526 aerospike-9.0.0/benchmarks/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1664 2022-10-10 17:42:29.000000 aerospike-9.0.0/benchmarks/README.rst
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4563 2022-12-15 01:59:21.000000 aerospike-9.0.0/benchmarks/keygen.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11901 2022-12-15 01:59:21.000000 aerospike-9.0.0/benchmarks/kvs.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.107526 aerospike-9.0.0/doc/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       19 2022-12-17 00:32:42.000000 aerospike-9.0.0/doc/.gitignore
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      652 2022-12-17 00:32:42.000000 aerospike-9.0.0/doc/README.md
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.107526 aerospike-9.0.0/doc/_static/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      374 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/_static/theme_overrides.css
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    43343 2023-01-03 18:24:47.000000 aerospike-9.0.0/doc/aerospike.rst
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      464 2022-12-17 00:32:42.000000 aerospike-9.0.0/doc/aerospike_helpers.batch.rst
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      275 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/aerospike_helpers.cdt_ctx.rst
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7618 2022-12-17 00:32:42.000000 aerospike-9.0.0/doc/aerospike_helpers.expressions.rst
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     1511 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/aerospike_helpers.operations.rst
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      709 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/aerospike_helpers.rst
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)   103621 2023-01-03 18:18:07.000000 aerospike-9.0.0/doc/client.rst
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     8111 2022-12-17 00:32:42.000000 aerospike-9.0.0/doc/conf.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5280 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/data_mapping.rst
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.111526 aerospike-9.0.0/doc/examples/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      321 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/batch_apply.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      903 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/batch_apply.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      627 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/batch_get_ops.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1187 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/batch_operate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      733 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/batch_remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1754 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/batch_write.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      463 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/boilerplate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      337 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/exists.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      602 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/exists_many.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.111526 aerospike-9.0.0/doc/examples/expressions/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1737 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/expressions/top.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      422 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/get.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1091 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/get_cdtctx_base64.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      196 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/get_expression_base64.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      117 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/get_key_digest.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      735 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/get_many.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1438 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/keyordereddict.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.111526 aerospike-9.0.0/doc/examples/lua/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1655 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/lua/example.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1157 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/lua/lua.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      760 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/operate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      658 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/operate_ordered.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      316 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/put.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.111526 aerospike-9.0.0/doc/examples/query/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1098 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/query/boilerplate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      465 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/query/foreach.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      513 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/query/foreachfalse.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      256 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/query/results.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      378 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      224 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/remove_bin.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      499 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/select.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      891 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/select_many.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2056 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/serializer.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      353 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/touch.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      447 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/examples/truncate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12584 2022-12-17 00:32:42.000000 aerospike-9.0.0/doc/exception.rst
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     3447 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/geojson.rst
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     2828 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/index.rst
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      670 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/key_ordered_dict.rst
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12176 2022-12-15 01:59:21.000000 aerospike-9.0.0/doc/predicates.rst
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)    22480 2022-12-17 00:32:42.000000 aerospike-9.0.0/doc/query.rst
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      113 2022-12-17 00:32:42.000000 aerospike-9.0.0/doc/requirements.txt
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)    23184 2022-12-17 00:32:42.000000 aerospike-9.0.0/doc/scan.rst
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.995526 aerospike-9.0.0/examples/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.115526 aerospike-9.0.0/examples/admin/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4216 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/change_password.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3867 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/create_role.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3880 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/create_user.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3756 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/drop_role.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3756 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/drop_user.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3931 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/grant_privileges.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3922 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/grant_roles.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3922 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/query_role.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3772 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/query_roles.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3877 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/query_user.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3883 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/query_user_info.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3778 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/query_users.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3783 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/query_users_info.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3928 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/revoke_privileges.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3931 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/revoke_roles.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3877 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/admin/set_password.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.119526 aerospike-9.0.0/examples/client/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6255 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/aggregate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4982 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/append.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4762 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/apply.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      329 2022-10-18 23:45:02.000000 aerospike-9.0.0/examples/client/bin_lua.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5141 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/bin_ops.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14832 2022-11-07 23:19:07.000000 aerospike-9.0.0/examples/client/client_big_list.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4957 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/delete.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      343 2022-10-18 23:45:02.000000 aerospike-9.0.0/examples/client/example.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4319 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/exists.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4614 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/exists_many.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5216 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/get.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5607 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/get_async.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4335 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/get_key_digest.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4616 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/get_many.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3660 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/get_nodes.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5082 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/increment.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4520 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/index_create.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3893 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/index_remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4640 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/info.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3710 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/info_node.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4278 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/is_connected.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5371 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/kvs.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4924 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/multi_thread.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5367 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/operate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4891 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/prepend.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5161 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/put.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6105 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/put_async.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7258 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/query.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7351 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/query_apply.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4296 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4429 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/remove_bin.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      289 2022-10-18 23:45:02.000000 aerospike-9.0.0/examples/client/sample.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4691 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/scan.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5442 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/scan_apply.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5056 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/scan_info.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5826 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/scan_partition.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4631 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/select_many.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4885 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/select_record.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1005 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/simple.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       38 2022-10-18 23:45:02.000000 aerospike-9.0.0/examples/client/simple_udf.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1282 2022-10-18 23:45:02.000000 aerospike-9.0.0/examples/client/stream_example.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5095 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/touch.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11947 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/ttl.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3792 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/udf_get.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3523 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/udf_list.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3703 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/udf_put.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3627 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/udf_remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7519 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/client/unicode_smiles.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.119526 aerospike-9.0.0/examples/deprecated/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3067 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/deprecated/exists.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3089 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/deprecated/get.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3770 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/deprecated/put.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2920 2022-12-15 01:59:21.000000 aerospike-9.0.0/examples/deprecated/remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      878 2022-12-17 00:32:42.000000 aerospike-9.0.0/pyproject.toml
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.119526 aerospike-9.0.0/scripts/
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      625 2022-12-17 00:32:42.000000 aerospike-9.0.0/scripts/manylinux2014build.sh
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)      493 2022-12-15 01:59:21.000000 aerospike-9.0.0/scripts/manylinuxbuild.sh
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     4543 2022-12-15 01:59:21.000000 aerospike-9.0.0/scripts/os_version
+-rwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)     1055 2022-12-15 01:59:21.000000 aerospike-9.0.0/scripts/wait-for-node.sh
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       38 2023-01-04 00:50:47.151525 aerospike-9.0.0/setup.cfg
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12234 2022-12-17 00:32:42.000000 aerospike-9.0.0/setup.py
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:46.995526 aerospike-9.0.0/src/
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.123525 aerospike-9.0.0/src/include/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6478 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/admin.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1255 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/bit_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1223 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/cdt_list_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1218 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/cdt_map_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2827 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/cdt_operation_utils.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      994 2022-12-15 01:59:21.000000 aerospike-9.0.0/src/include/cdt_types.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28201 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/client.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10104 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/conversions.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4750 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/exception_types.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      915 2022-12-15 01:59:21.000000 aerospike-9.0.0/src/include/exceptions.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1151 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/expression_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2215 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/geo.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      943 2022-12-15 01:59:21.000000 aerospike-9.0.0/src/include/global_hosts.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1218 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/hll_operations.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1092 2022-12-15 01:59:21.000000 aerospike-9.0.0/src/include/key_ordered_dict.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1791 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/log.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2934 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/macros.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1546 2022-12-15 01:59:21.000000 aerospike-9.0.0/src/include/module_functions.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      914 2022-12-15 01:59:21.000000 aerospike-9.0.0/src/include/nullobject.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1198 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/operate.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11909 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/policy.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2604 2023-01-03 18:24:47.000000 aerospike-9.0.0/src/include/policy_config.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1539 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/pool.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      836 2022-12-15 01:59:21.000000 aerospike-9.0.0/src/include/predicates.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4149 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/query.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3710 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/scan.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2531 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/serializer.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      914 2022-12-15 01:59:21.000000 aerospike-9.0.0/src/include/tls_config.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1129 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/tls_info_host.h
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2591 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/include/types.h
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.123525 aerospike-9.0.0/src/main/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9253 2023-01-04 00:50:40.000000 aerospike-9.0.0/src/main/aerospike.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4601 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/calc_digest.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.123525 aerospike-9.0.0/src/main/cdt_types/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6639 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/cdt_types/type.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.131525 aerospike-9.0.0/src/main/client/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    68407 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/admin.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8078 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/apply.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12209 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/batch_apply.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8655 2023-01-03 18:24:47.000000 aerospike-9.0.0/src/main/client/batch_get_ops.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12363 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/batch_operate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10965 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/batch_remove.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21805 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/batch_write.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    33885 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/bit_operate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    63986 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/cdt_list_operate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12527 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/cdt_map_operate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6831 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/cdt_operation_utils.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5399 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/close.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9281 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/connect.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6152 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/exists.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12598 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/exists_many.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4684 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/expression_operations.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6262 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/get.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9137 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/get_async.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4094 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/get_cdtctx_base64.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3377 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/get_expression_base64.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4564 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/get_key_digest.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5173 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/get_key_partition_id.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8863 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/get_many.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12232 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/get_nodes.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18261 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/hll_operate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    20058 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/info.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9073 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/info_node.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5243 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/info_random_node.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6187 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/info_single_node.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    54373 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/operate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    32955 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/operate_list.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    50339 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/operate_map.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6913 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/put.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8894 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/put_async.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21747 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/query.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6539 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/remove.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9061 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/remove_bin.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12808 2023-01-03 18:14:07.000000 aerospike-9.0.0/src/main/client/scan.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21795 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/sec_index.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8183 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/select.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10407 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/select_many.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5893 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/set_xdr_filter.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2351 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/tls_info_host.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6959 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/truncate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    70531 2023-01-03 18:18:07.000000 aerospike-9.0.0/src/main/client/type.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19738 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/client/udf.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    93577 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/conversions.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    69491 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/convert_expressions.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11037 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/convert_partition_filter.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27578 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/exception.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.131525 aerospike-9.0.0/src/main/geospatial/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2859 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/geospatial/dumps.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3659 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/geospatial/loads.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12738 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/geospatial/type.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1948 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/geospatial/unwrap.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2085 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/geospatial/wrap.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.131525 aerospike-9.0.0/src/main/global_hosts/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3818 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/global_hosts/type.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.131525 aerospike-9.0.0/src/main/key_ordered_dict/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2628 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/key_ordered_dict/type.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6293 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/log.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.131525 aerospike-9.0.0/src/main/nullobject/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3573 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/nullobject/type.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    52920 2023-01-03 18:14:07.000000 aerospike-9.0.0/src/main/policy.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21544 2023-01-03 18:24:47.000000 aerospike-9.0.0/src/main/policy_config.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12517 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/predicates.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.131525 aerospike-9.0.0/src/main/query/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3673 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/add_ops.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7041 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/apply.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2893 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/execute_background.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7808 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/foreach.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1654 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/get_parts.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2635 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/paginate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5123 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/results.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3003 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/select.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12774 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/type.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13603 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/query/where.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.135525 aerospike-9.0.0/src/main/scan/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3377 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/scan/add_ops.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7003 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/scan/apply.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2921 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/scan/execute_background.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8156 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/scan/foreach.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1649 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/scan/get_parts.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2854 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/scan/paginate.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5964 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/scan/results.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3091 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/scan/select.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8840 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/scan/type.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23618 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/serializer.c
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6257 2022-12-17 00:32:42.000000 aerospike-9.0.0/src/main/tls_config.c
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.135525 aerospike-9.0.0/test/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3186 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/README.md
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      563 2022-12-15 01:59:21.000000 aerospike-9.0.0/test/bin_lua.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       90 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/config.conf
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6265 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/counter26.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        0 2022-10-10 17:42:29.000000 aerospike-9.0.0/test/empty.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      342 2022-12-06 23:57:48.000000 aerospike-9.0.0/test/example.lua
+drwxrwxr-x   0 jnguyen   (1001) jnguyen   (1001)        0 2023-01-04 00:50:47.151525 aerospike-9.0.0/test/new_tests/
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)        0 2022-10-10 17:42:29.000000 aerospike-9.0.0/test/new_tests/__init__.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8800 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/as_errors.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      724 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/as_status_codes.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9129 2023-01-03 18:14:07.000000 aerospike-9.0.0/test/new_tests/conftest.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      686 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/index_helpers.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      358 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/invalid_data.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5343 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_change_password.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12754 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_create_role.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10177 2023-01-03 20:37:57.000000 aerospike-9.0.0/test/new_tests/test_admin_create_user.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5023 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_drop_role.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7026 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_drop_user.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2992 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_get_role.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2434 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_get_roles.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6841 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_grant_privileges.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5165 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_grant_roles.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2766 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_query_role.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2200 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_query_roles.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4386 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_query_user.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4538 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_query_user_info.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3253 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_query_users.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3311 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_query_users_info.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8743 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_revoke_privileges.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5972 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_revoke_roles.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3622 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_set_password.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5696 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_set_quotas.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6648 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_admin_set_whitelist.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11624 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_aggregate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15202 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_append.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14128 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_apply.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    23970 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_arithmetic_expressions.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7645 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_base_class.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10758 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_batch_apply.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5741 2023-01-03 18:18:07.000000 aerospike-9.0.0/test/new_tests/test_batch_get_ops.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8729 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_batch_operate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      779 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_batch_records.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6966 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_batch_remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16455 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_batch_write.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    58814 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_bitwise_operations.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2344 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_bool_config.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2643 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_calc_digest.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4208 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_cdt_compators.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24128 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_cdt_index.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2165 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_close.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3949 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_compress.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6614 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_connect.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1574 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_connect_memleak.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3459 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_data.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2094 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_error_codes.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6034 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_exists.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9563 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_exists_many.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5620 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_expression_operations.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12896 2023-01-03 18:14:07.000000 aerospike-9.0.0/test/new_tests/test_expressions_base.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11441 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_expressions_bit.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11009 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_expressions_bitwise_operators.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    27036 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_expressions_everywhere.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9473 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_expressions_hll.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    26449 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_expressions_list.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    18979 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_expressions_map.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    38095 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_geospatial.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8485 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_get_async.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4233 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_get_cdtctx_base64.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3784 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_get_expression_base64r.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3086 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_get_key_digest.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8406 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_get_many.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1556 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_get_node_names.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1675 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_get_nodes.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    28897 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_get_put.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5366 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_get_udf.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16574 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_hll.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16777 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_increment.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    19127 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_index.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4910 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_info.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3026 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_info_all.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5547 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_info_random_node.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6955 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_info_single_node.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6845 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_invalid_conf.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8602 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_inverted_map_operations.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     2013 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_is_connected.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5281 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_job_info.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3606 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_key_digest.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3516 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_key_ordered_dict_get_by_value.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7480 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_kv.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7807 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_append.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1123 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_basics.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5212 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_clear.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7115 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_extend.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5514 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_get.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6789 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_get_range.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13954 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_index.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8546 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_insert.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9194 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_insert_items.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6144 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_pop.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6928 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_pop_range.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6553 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7364 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_remove_range.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8690 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_set.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5241 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_size.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6754 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_list_trim.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1954 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_log.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    22871 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_map_basics.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16881 2023-01-03 18:18:07.000000 aerospike-9.0.0/test/new_tests/test_map_operation_helpers.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6726 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_map_write_flags.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3393 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_map_write_mode.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14639 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_mapkeys_index.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13620 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_mapvalues_index.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)   185860 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_nested_cdt_ctx.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3406 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_new_constructor.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17566 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_new_list_operation_helpers.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    24974 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_new_list_operations.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    43725 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_operate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    31672 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_operate_helpers.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    36122 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_operate_map.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    33960 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_operate_ordered.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      518 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_predicates.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    16465 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_prepend.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    26644 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_put_async.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    34463 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_query.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    17650 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_query_apply.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13129 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_query_execute_background.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    15415 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_query_expressions.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     5173 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_query_get_partitions_status.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9757 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_query_pagination.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    21455 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_query_partition.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14418 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_relative_cdt_operations.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    10969 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14665 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_remove_bin.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    13228 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_scan.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14839 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_scan_apply.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12500 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_scan_execute_background.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4973 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_scan_get_partitions_status.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11861 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_scan_pagination.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12626 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_scan_partition.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     8188 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_select.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    12743 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_select_many.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     4720 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_set_xdr_filter.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     9566 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_touch.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     7938 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_truncate.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3511 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_udf_list.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6793 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_udf_put.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     6818 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_udf_remove.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    11177 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_user_serializer.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)    14877 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/test_zserializers.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1903 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/new_tests/udf_helpers.py
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       56 2022-12-15 01:59:21.000000 aerospike-9.0.0/test/pytest.ini
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      380 2022-12-06 23:54:23.000000 aerospike-9.0.0/test/query_apply.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      290 2022-12-15 01:59:21.000000 aerospike-9.0.0/test/query_apply_parameters.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       29 2022-12-15 01:59:21.000000 aerospike-9.0.0/test/requirements.txt
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      289 2022-12-06 23:49:50.000000 aerospike-9.0.0/test/sample.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     1282 2022-12-06 23:49:25.000000 aerospike-9.0.0/test/stream_example.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)     3296 2022-12-15 01:59:21.000000 aerospike-9.0.0/test/test_record_udf.lua
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)      437 2022-12-17 00:32:42.000000 aerospike-9.0.0/test/tox.ini
+-rw-rw-r--   0 jnguyen   (1001) jnguyen   (1001)       84 2022-12-06 23:49:54.000000 aerospike-9.0.0/test/udf_basic_ops.lua
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `aerospike-8.0.0/.clang-format` & `aerospike-9.0.0/.clang-format`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/BUILD.md` & `aerospike-9.0.0/BUILD.md`

 * *Files 7% similar despite different names*

```diff
@@ -79,16 +79,26 @@
 ## Build
 
     export STATIC_SSL=1
     # substitute the paths to your OpenSSL 1.1 library
     export SSL_LIB_PATH=/usr/local/Cellar/openssl@1.1/1.1.1l/lib/
     export CPATH=/usr/local/Cellar/openssl@1.1/1.1.1l/include/
 
-    pip install build
-    python3 -m build
+Before building the wheel, it is recommended to manually clean the C client build:
+```
+python3 setup.py clean
+```
+Sometimes the C client will not rebuild if you switch branches and update the C client submodule, and you will end up
+using the wrong version of the C client. This can causes strange issues when building or testing the Python client.
+
+Then build the source distribution and wheel:
+```
+pip install build
+python3 -m build
+```
 
 ### Troubleshooting macOS
 
 In some versions of macOS, Python 2.7 is installed as ``python`` with
 ``pip`` as its associated package manager, and Python 3 is installed as ``python3``
 with ``pip3`` as the associated package manager. Make sure to use the ones that
 map to Python 3.
```

### Comparing `aerospike-8.0.0/LICENSE` & `aerospike-9.0.0/LICENSE`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/PKG-INFO` & `aerospike-9.0.0/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerospike
-Version: 8.0.0
+Version: 9.0.0
 Summary: Aerospike Client Library for Python
 Author-email: "Aerospike, Inc." <info@aerospike.com>
 License: Apache Software License
 Project-URL: Homepage, https://aerospike.com
 Keywords: aerospike,nosql,database
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `aerospike-8.0.0/README.rst` & `aerospike-9.0.0/README.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/Releases.md` & `aerospike-9.0.0/Releases.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/.build.yml` & `aerospike-9.0.0/aerospike-client-c/.build.yml`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/.github/workflows/build.yml` & `aerospike-9.0.0/aerospike-client-c/.github/workflows/build.yml`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/.github/workflows/codeql.yml` & `aerospike-9.0.0/aerospike-client-c/.github/workflows/codeql.yml`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/.gitignore` & `aerospike-9.0.0/aerospike-client-c/.gitignore`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/LICENSE.md` & `aerospike-9.0.0/aerospike-client-c/LICENSE.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/Makefile` & `aerospike-9.0.0/aerospike-client-c/Makefile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/README.md` & `aerospike-9.0.0/aerospike-client-c/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/README.md` & `aerospike-9.0.0/aerospike-client-c/examples/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_batch_get/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_batch_get/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_delay_queue/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_get/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_get/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_query/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_query/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/async_examples/async_scan/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/async_examples/async_scan/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/append/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/append/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/expire/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/expire/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/generation/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/generation/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/get/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/get/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/incr/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/incr/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/list/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/list/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/map/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/map/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/put/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/put/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/touch/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/touch/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/udf/src/lua/basic_udf.lua` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/udf/src/lua/basic_udf.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/basic_examples/udf/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/basic_examples/udf/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/batch_examples/get/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/batch_examples/get/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/geospatial_simple.png` & `aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/geospatial_simple.png`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/filter/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/simple/geospatial_simple.png` & `aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/simple/geospatial_simple.png`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/geospatial_examples/simple/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/geospatial_examples/simple/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/project/Makefile` & `aerospike-9.0.0/aerospike-client-c/examples/project/Makefile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/query_examples/aggregate/src/lua/query_udf.lua` & `aerospike-9.0.0/aerospike-client-c/examples/query_examples/aggregate/src/lua/query_udf.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/query_examples/aggregate/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/query_examples/aggregate/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/query_examples/simple/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/query_examples/simple/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/scan_examples/background/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/scan_examples/background/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/scan_examples/standard/src/main/example.c` & `aerospike-9.0.0/aerospike-client-c/examples/scan_examples/standard/src/main/example.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/utils/src/include/example_utils.h` & `aerospike-9.0.0/aerospike-client-c/examples/utils/src/include/example_utils.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/examples/utils/src/main/example_utils.c` & `aerospike-9.0.0/aerospike-client-c/examples/utils/src/main/example_utils.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/Makefile` & `aerospike-9.0.0/aerospike-client-c/modules/common/Makefile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/project/rules.mk` & `aerospike-9.0.0/aerospike-client-c/modules/common/project/rules.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/project/settings.mk` & `aerospike-9.0.0/aerospike-client-c/modules/common/project/settings.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/project/test.mk` & `aerospike-9.0.0/aerospike-client-c/modules/common/project/test.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_aerospike.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_aerospike.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arch.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arch.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arraylist.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arraylist.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arraylist_iterator.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_arraylist_iterator.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic_gcc.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic_gcc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic_win.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_atomic_win.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_boolean.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_boolean.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_buffer.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_buffer.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_buffer_pool.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_buffer_pool.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_bytes.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_bytes.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_dir.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_dir.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_double.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_double.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_geojson.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_geojson.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_hashmap.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_hashmap.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_hashmap_iterator.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_hashmap_iterator.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_integer.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_integer.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_iterator.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_iterator.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_list.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_list.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_list_iterator.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_list_iterator.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_log.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_log.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_log_macros.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_log_macros.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_map.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_map.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_map_iterator.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_map_iterator.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_module.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_module.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_monitor.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_monitor.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack_ext.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack_ext.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack_serializer.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_msgpack_serializer.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_nil.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_nil.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_orderedmap.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_orderedmap.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_pair.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_pair.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_password.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_password.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_queue.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_queue.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_queue_mt.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_queue_mt.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_random.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_random.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_rec.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_rec.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_result.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_result.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_serializer.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_serializer.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_sleep.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_sleep.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_std.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_std.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_stream.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_stream.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_string.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_string.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_string_builder.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_string_builder.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_stringmap.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_stringmap.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_thread.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_thread.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_thread_pool.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_thread_pool.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_timer.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_timer.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_types.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_types.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_udf_context.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_udf_context.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_util.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_util.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_val.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_val.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_vector.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/as_vector.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/aerospike/ssl_util.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/aerospike/ssl_util.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/alloc.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/alloc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_b64.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_b64.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_byte_order.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_byte_order.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_clock.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_clock.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_crypto.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_crypto.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_digest.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_digest.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_hash_math.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_hash_math.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_ll.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_ll.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_queue.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_queue.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_random.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/include/citrusleaf/cf_random.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_aerospike.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_aerospike.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_hooks.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_hooks.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_iterator.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_iterator.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_iterator_hooks.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_arraylist_iterator_hooks.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_boolean.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_boolean.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_buffer.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_buffer.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_buffer_pool.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_buffer_pool.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_bytes.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_bytes.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_double.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_double.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_geojson.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_geojson.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_integer.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_integer.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_iterator.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_iterator.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_list.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_list.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_log.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_log.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_map.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_map.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_module.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_module.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack_ext.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack_ext.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack_serializer.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_msgpack_serializer.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_nil.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_nil.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_orderedmap.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_orderedmap.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_pair.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_pair.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_password.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_password.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_queue.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_queue.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_queue_mt.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_queue_mt.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_random.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_random.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_rec.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_rec.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_result.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_result.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_serializer.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_serializer.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_stream.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_stream.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_string.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_string.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_string_builder.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_string_builder.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_thread_pool.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_thread_pool.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_timer.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_timer.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_val.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_val.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_vector.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/as_vector.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/crypt_blowfish.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/crypt_blowfish.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/crypt_blowfish.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/crypt_blowfish.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/aerospike/ssl_util.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/aerospike/ssl_util.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_alloc.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_alloc.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_b64.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_b64.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_clock.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_clock.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_crypto.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_crypto.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_digest.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_digest.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_ll.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_ll.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_queue.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_queue.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_random.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/main/citrusleaf/cf_random.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/common.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/common.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/msgpack/msgpack_direct.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/msgpack/msgpack_direct.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/msgpack/msgpack_rountrip.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/msgpack/msgpack_rountrip.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/test.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/test.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/test.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/test.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/test_common.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/test_common.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/test_common.h` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/test_common.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/password.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/password.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/random.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/random.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/string_builder.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/string_builder.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_arraylist.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_arraylist.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_boolean.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_boolean.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_bytes.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_bytes.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_double.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_double.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_hashmap.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_hashmap.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_integer.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_integer.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_nil.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_nil.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_orderedmap.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_orderedmap.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_queue.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_queue.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_queue_mt.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_queue_mt.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/src/test/types/types_string.c` & `aerospike-9.0.0/aerospike-client-c/modules/common/src/test/types/types_string.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common/aerospike-common.vcxproj` & `aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common/aerospike-common.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common/aerospike-common.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common/aerospike-common.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/aerospike-common-test.vcxproj` & `aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/aerospike-common-test.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/aerospike-common-test.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common-test/aerospike-common-test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/vs/aerospike-common.sln` & `aerospike-9.0.0/aerospike-client-c/modules/common/vs/aerospike-common.sln`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/vs/props/base.props` & `aerospike-9.0.0/aerospike-client-c/modules/common/vs/props/base.props`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/vs/props/test.props` & `aerospike-9.0.0/aerospike-client-c/modules/common/vs/props/test.props`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common-test.xcodeproj/project.pbxproj` & `aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common-test.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcodeproj/project.pbxproj` & `aerospike-9.0.0/aerospike-client-c/modules/common/xcode/aerospike-common.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/.travis.yml` & `aerospike-9.0.0/aerospike-client-c/modules/lua/.travis.yml`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/CMakeLists.txt` & `aerospike-9.0.0/aerospike-client-c/modules/lua/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/COPYRIGHT` & `aerospike-9.0.0/aerospike-client-c/modules/lua/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/HISTORY` & `aerospike-9.0.0/aerospike-client-c/modules/lua/HISTORY`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/INSTALL` & `aerospike-9.0.0/aerospike-client-c/modules/lua/INSTALL`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/Makefile` & `aerospike-9.0.0/aerospike-client-c/modules/lua/Makefile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/README.md` & `aerospike-9.0.0/aerospike-client-c/modules/lua/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/cmake/FindLua.cmake` & `aerospike-9.0.0/aerospike-client-c/modules/lua/cmake/FindLua.cmake`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/cmake/FindReadline.cmake` & `aerospike-9.0.0/aerospike-client-c/modules/lua/cmake/FindReadline.cmake`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/cmake/dist.cmake` & `aerospike-9.0.0/aerospike-client-c/modules/lua/cmake/dist.cmake`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/cmake/lua.cmake` & `aerospike-9.0.0/aerospike-client-c/modules/lua/cmake/lua.cmake`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/contents.html` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/contents.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/cover.png` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/cover.png`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/logo.gif` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/logo.gif`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/lua.1` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/lua.1`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/lua.css` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/lua.css`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/lua.html` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/lua.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/luac.1` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/luac.1`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/luac.html` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/luac.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/manual.html` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/manual.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/doc/readme.html` & `aerospike-9.0.0/aerospike-client-c/modules/lua/doc/readme.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/Makefile` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/Makefile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/README` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/README`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/all.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/all.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/lua.ico` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/lua.ico`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/lua.pc` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/lua.pc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/lua_lang.ico` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/lua_lang.ico`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/luavs.bat` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/luavs.bat`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/min.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/min.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/noparser.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/noparser.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/etc/strict.lua` & `aerospike-9.0.0/aerospike-client-c/modules/lua/etc/strict.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/Makefile` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/Makefile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lapi.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lapi.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lauxlib.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lauxlib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lauxlib.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lauxlib.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lbaselib.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lbaselib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lcode.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lcode.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lcode.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lcode.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldblib.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldblib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldebug.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldebug.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldebug.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldebug.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldo.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldo.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldo.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldo.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ldump.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ldump.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lfunc.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lfunc.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lfunc.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lfunc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lgc.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lgc.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lgc.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lgc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/linit.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/linit.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/liolib.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/liolib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/llex.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/llex.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/llex.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/llex.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/llimits.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/llimits.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lmathlib.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lmathlib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lmem.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lmem.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lmem.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lmem.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/loadlib.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/loadlib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/loadlib_rel.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/loadlib_rel.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lobject.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lobject.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lobject.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lobject.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lopcodes.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lopcodes.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lopcodes.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lopcodes.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/loslib.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/loslib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lparser.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lparser.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lparser.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lparser.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstate.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstate.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstate.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstring.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstring.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstring.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstring.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lstrlib.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lstrlib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltable.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltable.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltable.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltable.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltablib.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltablib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltm.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltm.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/ltm.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/ltm.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua.def` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua.def`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua.rc` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua.rc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lua_dll.rc` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lua_dll.rc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/luac.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/luac.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/luaconf.h.in` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/luaconf.h.in`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/luaconf.h.orig` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/luaconf.h.orig`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lualib.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lualib.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lundump.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lundump.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lundump.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lundump.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lvm.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lvm.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lvm.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lvm.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lzio.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lzio.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/lzio.h` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/lzio.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/src/print.c` & `aerospike-9.0.0/aerospike-client-c/modules/lua/src/print.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/test/README` & `aerospike-9.0.0/aerospike-client-c/modules/lua/test/README`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/test/bisect.lua` & `aerospike-9.0.0/aerospike-client-c/modules/lua/test/bisect.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/test/factorial.lua` & `aerospike-9.0.0/aerospike-client-c/modules/lua/test/factorial.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/test/fib.lua` & `aerospike-9.0.0/aerospike-client-c/modules/lua/test/fib.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/test/life.lua` & `aerospike-9.0.0/aerospike-client-c/modules/lua/test/life.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/test/sieve.lua` & `aerospike-9.0.0/aerospike-client-c/modules/lua/test/sieve.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/test/sort.lua` & `aerospike-9.0.0/aerospike-client-c/modules/lua/test/sort.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/test/trace-calls.lua` & `aerospike-9.0.0/aerospike-client-c/modules/lua/test/trace-calls.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/lua/test/trace-globals.lua` & `aerospike-9.0.0/aerospike-client-c/modules/lua/test/trace-globals.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/.travis.yml` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/.travis.yml`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/CMakeLists.txt` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/CMakeLists.txt`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/COPYRIGHT` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/COPYRIGHT`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/Makefile` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/Makefile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/cmake/FindLua.cmake` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/cmake/FindLua.cmake`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/cmake/FindReadline.cmake` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/cmake/FindReadline.cmake`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/cmake/dist.cmake` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/cmake/dist.cmake`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/cmake/lua.cmake` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/cmake/lua.cmake`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/bluequad-print.css` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/bluequad-print.css`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/bluequad.css` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/bluequad.css`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/changes.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/changes.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/contact.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/contact.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_c_api.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_c_api.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_api.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_api.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_semantics.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_semantics.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_tutorial.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_ffi_tutorial.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/ext_jit.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/ext_jit.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/extensions.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/extensions.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/faq.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/faq.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/img/contact.png` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/img/contact.png`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/install.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/install.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/luajit.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/luajit.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/running.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/running.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/doc/status.html` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/doc/status.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_arm.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_arm.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_arm.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_arm.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_mips.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_mips.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_mips.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_mips.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_ppc.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_ppc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_ppc.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_ppc.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_proto.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_proto.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x64.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x64.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x86.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x86.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x86.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dasm_x86.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/dynasm/dynasm.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/dynasm/dynasm.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/etc/luajit.1` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/etc/luajit.1`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/etc/luajit.ico` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/etc/luajit.ico`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/etc/luajit.pc` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/etc/luajit.pc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/Makefile` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/Makefile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/Makefile.dep` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/Makefile.dep`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_asm.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_asm.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_fold.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_fold.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_lib.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_lib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_peobj.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/buildvm_peobj.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/genminilua.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/genminilua.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/host/minilua.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/host/minilua.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/bc.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/bc.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/bcsave.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/bcsave.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_arm.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_arm.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_mips.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_mips.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_mipsel.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_mipsel.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_ppc.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_ppc.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_x64.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_x64.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dis_x86.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dis_x86.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/dump.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/dump.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/jit/v.lua` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/jit/v.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lauxlib.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lauxlib.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_aux.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_aux.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_base.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_base.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_bit.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_bit.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_debug.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_debug.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_ffi.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_ffi.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_init.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_init.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_io.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_io.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_jit.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_jit.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_math.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_math.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_os.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_os.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_package.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_package.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_package_rel.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_package_rel.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_string.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_string.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lib_table.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lib_table.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_alloc.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_alloc.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_api.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_api.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_arch.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_arch.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm_arm.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm_arm.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm_mips.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm_mips.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm_ppc.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm_ppc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_asm_x86.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_asm_x86.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_bc.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_bc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_bcdump.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_bcdump.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_bcread.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_bcread.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_bcwrite.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_bcwrite.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_carith.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_carith.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_carith.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_carith.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ccall.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ccall.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ccall.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ccall.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ccallback.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ccallback.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ccallback.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ccallback.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cconv.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cconv.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cconv.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cconv.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cdata.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cdata.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cdata.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cdata.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_char.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_char.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_char.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_char.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_clib.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_clib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_clib.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_clib.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cparse.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cparse.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_cparse.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_cparse.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_crecord.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_crecord.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_crecord.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_crecord.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ctype.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ctype.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ctype.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ctype.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_debug.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_debug.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_debug.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_debug.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_def.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_def.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_dispatch.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_dispatch.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_dispatch.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_dispatch.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_emit_arm.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_emit_arm.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_emit_mips.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_emit_mips.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_emit_ppc.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_emit_ppc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_emit_x86.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_emit_x86.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_err.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_err.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_err.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_err.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_errmsg.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_errmsg.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ffrecord.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ffrecord.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ffrecord.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ffrecord.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_frame.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_frame.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_func.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_func.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_func.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_func.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_gc.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_gc.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_gc.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_gc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_gdbjit.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_gdbjit.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ir.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ir.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ir.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ir.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_ircall.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_ircall.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_iropt.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_iropt.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_jit.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_jit.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_lex.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_lex.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_lex.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_lex.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_lib.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_lib.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_lib.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_lib.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_load.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_load.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_mcode.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_mcode.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_mcode.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_mcode.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_meta.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_meta.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_meta.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_meta.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_obj.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_obj.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_obj.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_obj.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_dce.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_dce.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_fold.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_fold.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_loop.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_loop.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_mem.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_mem.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_narrow.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_narrow.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_sink.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_sink.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_opt_split.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_opt_split.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_parse.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_parse.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_record.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_record.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_record.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_record.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_snap.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_snap.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_snap.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_snap.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_state.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_state.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_state.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_state.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_str.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_str.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_str.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_str.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_strscan.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_strscan.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_strscan.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_strscan.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_tab.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_tab.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_tab.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_tab.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target_arm.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target_arm.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target_mips.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target_mips.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target_ppc.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target_ppc.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_target_x86.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_target_x86.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_trace.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_trace.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_trace.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_trace.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_traceerr.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_traceerr.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_udata.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_udata.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_vm.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_vm.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_vmevent.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_vmevent.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_vmevent.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_vmevent.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lj_vmmath.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lj_vmmath.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/ljamalg.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/ljamalg.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lua.def` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lua.def`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lua.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lua.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luaconf.h.in` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luaconf.h.in`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luaconf.h.orig` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luaconf.h.orig`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luajit.c` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luajit.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luajit.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luajit.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/luajit.rc` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/luajit.rc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/lualib.h` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/lualib.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/msvcbuild.bat` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/msvcbuild.bat`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/ps4build.bat` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/ps4build.bat`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_arm.dasc` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_arm.dasc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_mips.dasc` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_mips.dasc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_ppc.dasc` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_ppc.dasc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_ppcspe.dasc` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_ppcspe.dasc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/vm_x86.dasc` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/vm_x86.dasc`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/luajit/src/xedkbuild.bat` & `aerospike-9.0.0/aerospike-client-c/modules/luajit/src/xedkbuild.bat`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/Makefile` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/Makefile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/README.md` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/project/modules.mk` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/project/modules.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/project/rules.mk` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/project/rules.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/project/settings.mk` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/project/settings.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/project/test.mk` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/project/test.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_aerospike.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_aerospike.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_bytes.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_bytes.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_config.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_config.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_geojson.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_geojson.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_iterator.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_iterator.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_list.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_list.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_map.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_map.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_record.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_record.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_reg.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_reg.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_stream.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_stream.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_val.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/include/aerospike/mod_lua_val.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/internal.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/internal.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/internal.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/internal.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_aerospike.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_aerospike.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_bytes.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_bytes.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_geojson.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_geojson.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_iterator.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_iterator.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_list.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_list.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_map.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_map.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_record.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_record.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_reg.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_reg.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_stream.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_stream.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_system.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_system.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_val.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/main/mod_lua_val.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/hash/hash_udf.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/hash/hash_udf.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/list/list_udf.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/list/list_udf.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/aggr.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/aggr.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/basics.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/basics.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/bytes.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/bytes.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/integers.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/integers.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/lists.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/lists.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/maps.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/maps.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/records.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/records.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_bytes.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_bytes.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_unit.lua` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/lua/test_unit.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/mod_lua_test.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/mod_lua_test.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/record/record_udf.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/record/record_udf.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/stream/stream_udf.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/stream/stream_udf.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/test.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/test.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/test.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/test.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/consumer_stream.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/consumer_stream.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/consumer_stream.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/consumer_stream.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/map_rec.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/map_rec.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/map_rec.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/map_rec.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/producer_stream.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/producer_stream.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/producer_stream.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/producer_stream.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_aerospike.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_aerospike.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_aerospike.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_aerospike.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_logger.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_logger.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_logger.h` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/util/test_logger.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/src/test/validation/validation_basics.c` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/src/test/validation/validation_basics.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/aerospike-mod-lua.vcxproj` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/aerospike-mod-lua.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/aerospike-mod-lua.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua/aerospike-mod-lua.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/aerospike-mod-lua-test.vcxproj` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/aerospike-mod-lua-test.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/aerospike-mod-lua-test.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua-test/aerospike-mod-lua-test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua.sln` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/aerospike-mod-lua.sln`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/props/base.props` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/props/base.props`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/vs/props/test.props` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/vs/props/test.props`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua-test.xcodeproj/project.pbxproj` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua-test.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcodeproj/project.pbxproj` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/aerospike-mod-lua.xcscmblueprint` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/aerospike-mod-lua.xcscmblueprint`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/mod-lua.xcscmblueprint` & `aerospike-9.0.0/aerospike-client-c/modules/mod-lua/xcode/aerospike-mod-lua.xcworkspace/xcshareddata/mod-lua.xcscmblueprint`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/pkg/README.md` & `aerospike-9.0.0/aerospike-client-c/pkg/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/pkg/install` & `aerospike-9.0.0/aerospike-client-c/pkg/install`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/pkg/package` & `aerospike-9.0.0/aerospike-client-c/pkg/package`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/pkg/package_src` & `aerospike-9.0.0/aerospike-client-c/pkg/package_src`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/pkg/package_type` & `aerospike-9.0.0/aerospike-client-c/pkg/package_type`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/pkg/platform` & `aerospike-9.0.0/aerospike-client-c/pkg/platform`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/pkg/rpm/client-devel.spec` & `aerospike-9.0.0/aerospike-client-c/pkg/rpm/client-devel.spec`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/pkg/set_version` & `aerospike-9.0.0/aerospike-client-c/pkg/set_version`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/project/doxyfile` & `aerospike-9.0.0/aerospike-client-c/project/doxyfile`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/project/modules.mk` & `aerospike-9.0.0/aerospike-client-c/project/modules.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/project/rules.mk` & `aerospike-9.0.0/aerospike-client-c/project/rules.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/project/settings.mk` & `aerospike-9.0.0/aerospike-client-c/project/settings.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/project/test.mk` & `aerospike-9.0.0/aerospike-client-c/project/test.mk`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/apidocs/header.html` & `aerospike-9.0.0/aerospike-client-c/src/apidocs/header.html`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/apidocs/html/aerospike.css` & `aerospike-9.0.0/aerospike-client-c/src/apidocs/html/aerospike.css`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/apidocs/html/aerospike_logo.png` & `aerospike-9.0.0/aerospike-client-c/src/apidocs/html/aerospike_logo.png`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/apidocs/html/style.css` & `aerospike-9.0.0/aerospike-client-c/src/apidocs/html/style.css`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/apidocs/layout.xml` & `aerospike-9.0.0/aerospike-client-c/src/apidocs/layout.xml`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/apidocs/old.css` & `aerospike-9.0.0/aerospike-client-c/src/apidocs/old.css`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_batch.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_batch.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_index.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_index.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_info.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_info.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_key.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_key.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_query.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_query.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_scan.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_scan.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_stats.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_stats.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/aerospike_udf.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/aerospike_udf.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_address.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_address.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_admin.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_admin.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_async.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_async.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_async_proto.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_async_proto.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_batch.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_batch.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_bin.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_bin.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_bit_operations.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_bit_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cdt_ctx.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cdt_ctx.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cdt_internal.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cdt_internal.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cdt_order.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cdt_order.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cluster.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cluster.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_command.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_command.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_config.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_config.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_conn_pool.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_conn_pool.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_cpu.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_cpu.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_error.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_error.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_event.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_event.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_event_internal.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_event_internal.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_exp.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_exp.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_exp_operations.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_exp_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_hll_operations.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_hll_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_host.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_host.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_info.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_info.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_job.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_job.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_key.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_key.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_list_operations.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_list_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_listener.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_listener.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_lookup.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_lookup.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_map_operations.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_map_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_node.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_node.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_operations.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_partition.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_partition.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_partition_filter.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_partition_filter.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_partition_tracker.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_partition_tracker.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_peers.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_peers.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_pipe.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_pipe.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_policy.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_policy.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_poll.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_poll.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_proto.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_proto.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_query.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_query.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_query_validate.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_query_validate.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_record.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_record.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_record_iterator.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_record_iterator.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_scan.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_scan.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_shm_cluster.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_shm_cluster.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_socket.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_socket.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_status.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_status.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_tls.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_tls.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/include/aerospike/as_udf.h` & `aerospike-9.0.0/aerospike-client-c/src/include/aerospike/as_udf.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/_bin.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/_bin.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/_bin.h` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/_bin.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_batch.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_batch.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_index.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_index.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_info.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_info.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_key.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_key.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_query.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_query.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_scan.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_scan.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_stats.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_stats.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/aerospike_udf.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/aerospike_udf.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_address.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_address.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_admin.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_admin.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_async.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_batch.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_batch.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_bit_operations.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_bit_operations.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_cdt_ctx.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_cdt_ctx.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_cdt_internal.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_cdt_internal.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_cluster.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_cluster.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_command.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_command.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_config.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_config.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_error.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_error.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event_ev.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event_ev.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event_event.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event_event.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event_none.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event_none.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_event_uv.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_event_uv.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_exp.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_exp.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_exp_operations.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_exp_operations.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_hll_operations.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_hll_operations.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_host.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_host.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_info.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_info.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_job.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_job.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_key.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_key.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_list_operations.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_list_operations.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_lookup.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_lookup.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_map_operations.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_map_operations.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_node.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_node.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_operations.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_operations.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_partition.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_partition.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_partition_tracker.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_partition_tracker.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_peers.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_peers.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_pipe.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_pipe.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_policy.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_policy.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_proto.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_proto.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_query.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_query.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_query_validate.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_query_validate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_record.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_record.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_record_hooks.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_record_hooks.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_record_iterator.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_record_iterator.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_scan.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_scan.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_shm_cluster.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_shm_cluster.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_socket.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_socket.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_tls.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_tls.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/main/aerospike/as_udf.c` & `aerospike-9.0.0/aerospike-client-c/src/main/aerospike/as_udf.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_batch/batch.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_batch/batch.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_batch/batch_async.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_batch/batch_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_bit/bit.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_bit/bit.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_geo/query_geospatial.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_geo/query_geospatial.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_geo/starbucks_3k.jpg` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_geo/starbucks_3k.jpg`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_index/index_basics.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_index/index_basics.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_info/info_basics.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_info/info_basics.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/hll_operate.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/hll_operate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_apply.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_apply.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_apply2.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_apply2.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_apply_async.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_apply_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_basics.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_basics.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_basics_async.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_basics_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_operate.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_operate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_key/key_pipeline.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_key/key_pipeline.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_list/list_basics.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_list/list_basics.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_list/list_basics_async.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_list/list_basics_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_basics.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_basics.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_basics_async.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_basics_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_index.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_index.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_sort.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_sort.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_map/map_udf.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_map/map_udf.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_query/query_async.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_query/query_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_query/query_background.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_query/query_background.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_query/query_foreach.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_query/query_foreach.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_scan/aerospike_scan_test.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_scan/aerospike_scan_test.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_scan/scan_async.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_scan/scan_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_scan/scan_basics.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_scan/scan_basics.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_test.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_test.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_test.h` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_test.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_udf/udf_basics.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_udf/udf_basics.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_udf/udf_record.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_udf/udf_record.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/aerospike_udf/udf_types.c` & `aerospike-9.0.0/aerospike-client-c/src/test/aerospike_udf/udf_types.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/exp_operate.c` & `aerospike-9.0.0/aerospike-client-c/src/test/exp_operate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/filter_exp.c` & `aerospike-9.0.0/aerospike-client-c/src/test/filter_exp.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/lua/client_record_basics.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/lua/client_record_basics.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/lua/client_record_lists.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/lua/client_record_lists.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/lua/client_stream_ads.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/lua/client_stream_ads.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/lua/client_stream_simple.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/lua/client_stream_simple.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/lua/key_apply.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/lua/key_apply.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/lua/key_apply2.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/lua/key_apply2.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/lua/query_background.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/lua/query_background.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/lua/udf_record.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/lua/udf_record.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/lua/udf_types.lua` & `aerospike-9.0.0/aerospike-client-c/src/test/lua/udf_types.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/test.c` & `aerospike-9.0.0/aerospike-client-c/src/test/test.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/test.h` & `aerospike-9.0.0/aerospike-client-c/src/test/test.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/consumer_stream.c` & `aerospike-9.0.0/aerospike-client-c/src/test/util/consumer_stream.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/consumer_stream.h` & `aerospike-9.0.0/aerospike-client-c/src/test/util/consumer_stream.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/index_util.c` & `aerospike-9.0.0/aerospike-client-c/src/test/util/index_util.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/index_util.h` & `aerospike-9.0.0/aerospike-client-c/src/test/util/index_util.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/info_helper.c` & `aerospike-9.0.0/aerospike-client-c/src/test/util/info_helper.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/info_helper.h` & `aerospike-9.0.0/aerospike-client-c/src/test/util/info_helper.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/log_helper.c` & `aerospike-9.0.0/aerospike-client-c/src/test/util/log_helper.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/log_helper.h` & `aerospike-9.0.0/aerospike-client-c/src/test/util/log_helper.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/map_rec.c` & `aerospike-9.0.0/aerospike-client-c/src/test/util/map_rec.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/map_rec.h` & `aerospike-9.0.0/aerospike-client-c/src/test/util/map_rec.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/producer_stream.c` & `aerospike-9.0.0/aerospike-client-c/src/test/util/producer_stream.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/producer_stream.h` & `aerospike-9.0.0/aerospike-client-c/src/test/util/producer_stream.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/test_aerospike.c` & `aerospike-9.0.0/aerospike-client-c/src/test/util/test_aerospike.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/test_aerospike.h` & `aerospike-9.0.0/aerospike-client-c/src/test/util/test_aerospike.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/udf.c` & `aerospike-9.0.0/aerospike-client-c/src/test/util/udf.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/src/test/util/udf.h` & `aerospike-9.0.0/aerospike-client-c/src/test/util/udf.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/README.md` & `aerospike-9.0.0/aerospike-client-c/vs/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike/aerospike.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike/aerospike.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike/aerospike.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike/aerospike.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c-libevent.nuspec` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c-libevent.nuspec`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c-libevent.targets` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c-libevent.targets`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c-libuv.nuspec` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c-libuv.nuspec`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c-libuv.targets` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c-libuv.targets`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c.nuspec` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c.nuspec`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike-client-c.targets` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike-client-c.targets`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike-test/aerospike-test.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike-test/aerospike-test.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike-test/aerospike-test.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike-test/aerospike-test.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/aerospike.sln` & `aerospike-9.0.0/aerospike-client-c/vs/aerospike.sln`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/append/append.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/append/append.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/append/append.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/append/append.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-batch-get/async-batch-get.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-batch-get/async-batch-get.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-batch-get/async-batch-get.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-batch-get/async-batch-get.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-delay-queue/async-delay-queue.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-delay-queue/async-delay-queue.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-delay-queue/async-delay-queue.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-delay-queue/async-delay-queue.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-get/async-get.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-get/async-get.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-get/async-get.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-get/async-get.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-query/async-query.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-query/async-query.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-query/async-query.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-query/async-query.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-scan/async-scan.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-scan/async-scan.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/async-scan/async-scan.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/async-scan/async-scan.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/batch-get/batch-get.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/batch-get/batch-get.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/batch-get/batch-get.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/batch-get/batch-get.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/expire/expire.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/expire/expire.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/expire/expire.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/expire/expire.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/generation/generation.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/generation/generation.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/generation/generation.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/generation/generation.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/geo-filter/geo-filter.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/geo-filter/geo-filter.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/geo-filter/geo-filter.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/geo-filter/geo-filter.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/geo-simple/geo-simple.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/geo-simple/geo-simple.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/geo-simple/geo-simple.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/geo-simple/geo-simple.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/get/get.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/get/get.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/get/get.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/get/get.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/incr/incr.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/incr/incr.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/incr/incr.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/incr/incr.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/list/list.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/list/list.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/list/list.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/list/list.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/map/map.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/map/map.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/map/map.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/map/map.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/put/put.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/put/put.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/put/put.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/put/put.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/query/query.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/query/query.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/query/query.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/query/query.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/query-aggregate/query-aggregate.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/query-aggregate/query-aggregate.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/query-aggregate/query-aggregate.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/query-aggregate/query-aggregate.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/scan/scan.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/scan/scan.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/scan/scan.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/scan/scan.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/scan-background/scan-background.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/scan-background/scan-background.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/scan-background/scan-background.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/scan-background/scan-background.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/touch/touch.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/touch/touch.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/touch/touch.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/touch/touch.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/udf/udf.vcxproj` & `aerospike-9.0.0/aerospike-client-c/vs/examples/udf/udf.vcxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/examples/udf/udf.vcxproj.filters` & `aerospike-9.0.0/aerospike-client-c/vs/examples/udf/udf.vcxproj.filters`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/icon.png` & `aerospike-9.0.0/aerospike-client-c/vs/icon.png`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/props/base.props` & `aerospike-9.0.0/aerospike-client-c/vs/props/base.props`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/props/example.props` & `aerospike-9.0.0/aerospike-client-c/vs/props/example.props`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/props/libevent.props` & `aerospike-9.0.0/aerospike-client-c/vs/props/libevent.props`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/props/libuv.props` & `aerospike-9.0.0/aerospike-client-c/vs/props/libuv.props`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/vs/props/nodejs.props` & `aerospike-9.0.0/aerospike-client-c/vs/props/nodejs.props`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/xcode/aerospike-test.xcodeproj/project.pbxproj` & `aerospike-9.0.0/aerospike-client-c/xcode/aerospike-test.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/xcode/aerospike.xcodeproj/project.pbxproj` & `aerospike-9.0.0/aerospike-client-c/xcode/aerospike.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/xcode/client.xcworkspace/xcshareddata/client.xcscmblueprint` & `aerospike-9.0.0/aerospike-client-c/xcode/client.xcworkspace/xcshareddata/client.xcscmblueprint`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/xcode/examples.xcodeproj/project.pbxproj` & `aerospike-9.0.0/aerospike-client-c/xcode/examples.xcodeproj/project.pbxproj`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike-client-c/xcode/prepare_xcode` & `aerospike-9.0.0/aerospike-client-c/xcode/prepare_xcode`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike.egg-info/PKG-INFO` & `aerospike-9.0.0/aerospike.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: aerospike
-Version: 8.0.0
+Version: 9.0.0
 Summary: Aerospike Client Library for Python
 Author-email: "Aerospike, Inc." <info@aerospike.com>
 License: Apache Software License
 Project-URL: Homepage, https://aerospike.com
 Keywords: aerospike,nosql,database
 Classifier: License :: OSI Approved :: Apache Software License
 Classifier: Operating System :: POSIX :: Linux
```

### Comparing `aerospike-8.0.0/aerospike.egg-info/SOURCES.txt` & `aerospike-9.0.0/aerospike.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/__init__.py` & `aerospike-9.0.0/aerospike_helpers/__init__.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/awaitable/__init__.py` & `aerospike-9.0.0/aerospike_helpers/awaitable/__init__.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/awaitable/io.py` & `aerospike-9.0.0/aerospike_helpers/awaitable/io.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/batch/__init__.py` & `aerospike-9.0.0/aerospike_helpers/batch/__init__.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/batch/records.py` & `aerospike-9.0.0/aerospike_helpers/batch/records.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/cdt_ctx.py` & `aerospike-9.0.0/aerospike_helpers/cdt_ctx.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/expressions/__init__.py` & `aerospike-9.0.0/aerospike_helpers/expressions/__init__.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/expressions/arithmetic.py` & `aerospike-9.0.0/aerospike_helpers/expressions/arithmetic.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/expressions/base.py` & `aerospike-9.0.0/aerospike_helpers/expressions/base.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/expressions/bitwise.py` & `aerospike-9.0.0/aerospike_helpers/expressions/bitwise.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/expressions/bitwise_operators.py` & `aerospike-9.0.0/aerospike_helpers/expressions/bitwise_operators.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/expressions/hll.py` & `aerospike-9.0.0/aerospike_helpers/expressions/hll.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/expressions/list.py` & `aerospike-9.0.0/aerospike_helpers/expressions/list.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/expressions/map.py` & `aerospike-9.0.0/aerospike_helpers/expressions/map.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/expressions/resources.py` & `aerospike-9.0.0/aerospike_helpers/expressions/resources.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/operations/__init__.py` & `aerospike-9.0.0/aerospike_helpers/operations/__init__.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/operations/bitwise_operations.py` & `aerospike-9.0.0/aerospike_helpers/operations/bitwise_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/operations/expression_operations.py` & `aerospike-9.0.0/aerospike_helpers/operations/expression_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/operations/hll_operations.py` & `aerospike-9.0.0/aerospike_helpers/operations/hll_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/operations/list_operations.py` & `aerospike-9.0.0/aerospike_helpers/operations/list_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/operations/map_operations.py` & `aerospike-9.0.0/aerospike_helpers/operations/map_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/aerospike_helpers/operations/operations.py` & `aerospike-9.0.0/aerospike_helpers/operations/operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/benchmarks/README.rst` & `aerospike-9.0.0/benchmarks/README.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/benchmarks/keygen.py` & `aerospike-9.0.0/benchmarks/keygen.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/benchmarks/kvs.py` & `aerospike-9.0.0/benchmarks/kvs.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/README.md` & `aerospike-9.0.0/doc/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/aerospike.rst` & `aerospike-9.0.0/doc/aerospike.rst`

 * *Files 0% similar despite different names*

```diff
@@ -563,15 +563,15 @@
         * **send_bool_as** (:class:`int`)
             Configures the client to encode Python booleans as the native Python boolean type, an integer, or the server boolean type.
 
             Use one of the :ref:`send_bool_as_constants` constant values.
 
             See :ref:`Data_Mapping` for more information.
 
-            Default: :data:`aerospike.PY_BYTES`
+            Default: :data:`aerospike.AS_BOOL`
         * **serialization** (:class:`tuple`)
             An optional instance-level `tuple` of ``(serializer, deserializer)``.
 
             Takes precedence over a class serializer registered with :func:`~aerospike.set_serializer`.
         * **thread_pool_size** (:class:`int`)
             Number of threads in the pool that is used in batch/scan/query commands.
 
@@ -1377,14 +1377,18 @@
 
     (int): 11
 
 .. data:: AS_BYTES_ERLANG
 
     (int): 12
 
+.. data:: AS_BYTES_BOOL
+
+    (int): 17
+
 .. data:: AS_BYTES_HLL
 
     (int): 18
 
 .. data:: AS_BYTES_MAP
 
     (int): 19
```

### Comparing `aerospike-8.0.0/doc/aerospike_helpers.expressions.rst` & `aerospike-9.0.0/doc/aerospike_helpers.expressions.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/aerospike_helpers.operations.rst` & `aerospike-9.0.0/doc/aerospike_helpers.operations.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/aerospike_helpers.rst` & `aerospike-9.0.0/doc/aerospike_helpers.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/client.rst` & `aerospike-9.0.0/doc/client.rst`

 * *Files 1% similar despite different names*

```diff
@@ -283,15 +283,15 @@
         :param dict policy: see :ref:`aerospike_batch_policies`.
 
         :return: a :class:`list` of :ref:`aerospike_record_tuple`.
 
         .. include:: examples/select_many.py
             :code: python
 
-    .. method:: batch_get_ops(keys, ops, meta, policy: dict) -> [ (key, meta, bins)]
+    .. method:: batch_get_ops(keys, ops, policy: dict) -> [ (key, meta, bins)]
 
         Batch-read multiple records, and return them as a :class:`list`.
         
         Any record that does not exist will have a exception type value as metadata \
         and :py:obj:`None` value as bins in the record tuple.
 
         :param list keys: a list of :ref:`aerospike_key_tuple`.
@@ -1985,14 +1985,23 @@
             | Determine if batch commands to each server are run in parallel threads. 
             | 
             | Default ``False``
         * **allow_inline** (:class:`bool`)
             | Allow batch to be processed immediately in the server's receiving thread when the server deems it to be appropriate.  If `False`, the batch will always be processed in separate transaction threads.  This field is only relevant for the new batch index protocol. 
             | 
             | Default ``True``
+        * **allow_inline_ssd** (:class:`bool`)
+            Allow batch to be processed immediately in the server's receiving thread for SSD namespaces.
+            If false, the batch will always be processed in separate service threads. Server versions < 6.0 ignore this field.
+
+            Inline processing can introduce the possibility of unfairness because the server can process the entire
+            batch before moving onto the next command.
+
+            Default: ``False``
+
         * **send_set_name** (:class:`bool`) 
             |
             |   .. deprecated:: in client version 7.0.0, the client ignores this policy and always sends set name to the server.
             |
             | Send set name field to server for every key in the batch for batch index protocol. This is only necessary when authentication is enabled and security roles are defined on a per set basis. 
             | 
             | Default: ``False``
@@ -2002,14 +2011,31 @@
             | Default: ``True``
         * **expressions** :class:`list`
             | Compiled aerospike expressions :mod:`aerospike_helpers` used for filtering records within a transaction.
             |
             | Default: None
 
             .. note:: Requires Aerospike server version >= 5.2.
+        * **respond_all_keys** :class:`bool`
+            Should all batch keys be attempted regardless of errors. This field is used on both the client and server.
+            The client handles node specific errors and the server handles key specific errors.
+
+            If ``True``, every batch key is attempted regardless of previous key specific errors.
+            Node specific errors such as timeouts stop keys to that node, but keys directed at other nodes will continue
+            to be processed.
+
+            If ``False``, the server will stop the batch to its node on most key specific errors. The exceptions are
+            ``AEROSPIKE_ERR_RECORD_NOT_FOUND`` and ``AEROSPIKE_FILTERED_OUT`` which never stop the batch. The client
+            will stop the entire batch on node specific errors for sync commands that are run in sequence
+            (``concurrent`` == false).
+            The client will not stop the entire batch for async commands or sync commands run in parallel.
+
+            Server versions < 6.0 do not support this field and treat this value as false for key specific errors.
+
+            Default: ``True``
 
 .. _aerospike_batch_write_policies:
 
 Batch Write Policies
 --------------------
 
 .. object:: policy
```

### Comparing `aerospike-8.0.0/doc/conf.py` & `aerospike-9.0.0/doc/conf.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/data_mapping.rst` & `aerospike-9.0.0/doc/data_mapping.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/batch_apply.py` & `aerospike-9.0.0/doc/examples/batch_apply.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/batch_get_ops.py` & `aerospike-9.0.0/doc/examples/batch_get_ops.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/batch_operate.py` & `aerospike-9.0.0/doc/examples/batch_operate.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/batch_remove.py` & `aerospike-9.0.0/doc/examples/batch_remove.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/batch_write.py` & `aerospike-9.0.0/doc/examples/batch_write.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/exists_many.py` & `aerospike-9.0.0/doc/examples/exists_many.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/expressions/top.py` & `aerospike-9.0.0/doc/examples/expressions/top.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/get_cdtctx_base64.py` & `aerospike-9.0.0/doc/examples/get_cdtctx_base64.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/get_many.py` & `aerospike-9.0.0/doc/examples/get_many.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/keyordereddict.py` & `aerospike-9.0.0/doc/examples/keyordereddict.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/lua/example.lua` & `aerospike-9.0.0/doc/examples/lua/example.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/lua/lua.py` & `aerospike-9.0.0/doc/examples/lua/lua.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/operate.py` & `aerospike-9.0.0/doc/examples/operate.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/operate_ordered.py` & `aerospike-9.0.0/doc/examples/operate_ordered.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/query/boilerplate.py` & `aerospike-9.0.0/doc/examples/query/boilerplate.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/query/foreachfalse.py` & `aerospike-9.0.0/doc/examples/query/foreachfalse.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/select_many.py` & `aerospike-9.0.0/doc/examples/select_many.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/examples/serializer.py` & `aerospike-9.0.0/doc/examples/serializer.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/exception.rst` & `aerospike-9.0.0/doc/exception.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/geojson.rst` & `aerospike-9.0.0/doc/geojson.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/index.rst` & `aerospike-9.0.0/doc/index.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/key_ordered_dict.rst` & `aerospike-9.0.0/doc/key_ordered_dict.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/predicates.rst` & `aerospike-9.0.0/doc/predicates.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/query.rst` & `aerospike-9.0.0/doc/query.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/doc/scan.rst` & `aerospike-9.0.0/doc/scan.rst`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/change_password.py` & `aerospike-9.0.0/examples/admin/change_password.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/create_role.py` & `aerospike-9.0.0/examples/admin/create_role.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/create_user.py` & `aerospike-9.0.0/examples/admin/create_user.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/drop_role.py` & `aerospike-9.0.0/examples/admin/drop_role.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/drop_user.py` & `aerospike-9.0.0/examples/admin/drop_user.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/grant_privileges.py` & `aerospike-9.0.0/examples/admin/grant_privileges.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/grant_roles.py` & `aerospike-9.0.0/examples/admin/grant_roles.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/query_role.py` & `aerospike-9.0.0/examples/admin/query_role.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/query_roles.py` & `aerospike-9.0.0/examples/admin/query_roles.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/query_user.py` & `aerospike-9.0.0/examples/admin/query_user.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/query_user_info.py` & `aerospike-9.0.0/examples/admin/query_user_info.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/query_users.py` & `aerospike-9.0.0/examples/admin/query_users.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/query_users_info.py` & `aerospike-9.0.0/examples/admin/query_users_info.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/revoke_privileges.py` & `aerospike-9.0.0/examples/admin/revoke_privileges.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/revoke_roles.py` & `aerospike-9.0.0/examples/admin/revoke_roles.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/admin/set_password.py` & `aerospike-9.0.0/examples/admin/set_password.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/aggregate.py` & `aerospike-9.0.0/examples/client/aggregate.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/append.py` & `aerospike-9.0.0/examples/client/append.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/apply.py` & `aerospike-9.0.0/examples/client/apply.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/bin_ops.py` & `aerospike-9.0.0/examples/client/bin_ops.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/client_big_list.py` & `aerospike-9.0.0/examples/client/client_big_list.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/delete.py` & `aerospike-9.0.0/examples/client/delete.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/exists.py` & `aerospike-9.0.0/examples/client/exists.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/exists_many.py` & `aerospike-9.0.0/examples/client/exists_many.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/get.py` & `aerospike-9.0.0/examples/client/get.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/get_async.py` & `aerospike-9.0.0/examples/client/get_async.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/get_key_digest.py` & `aerospike-9.0.0/examples/client/get_key_digest.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/get_many.py` & `aerospike-9.0.0/examples/client/get_many.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/get_nodes.py` & `aerospike-9.0.0/examples/client/get_nodes.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/increment.py` & `aerospike-9.0.0/examples/client/increment.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/index_create.py` & `aerospike-9.0.0/examples/client/index_create.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/index_remove.py` & `aerospike-9.0.0/examples/client/index_remove.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/info.py` & `aerospike-9.0.0/examples/client/info.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/info_node.py` & `aerospike-9.0.0/examples/client/info_node.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/is_connected.py` & `aerospike-9.0.0/examples/client/is_connected.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/kvs.py` & `aerospike-9.0.0/examples/client/kvs.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/multi_thread.py` & `aerospike-9.0.0/examples/client/multi_thread.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/operate.py` & `aerospike-9.0.0/examples/client/operate.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/prepend.py` & `aerospike-9.0.0/examples/client/prepend.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/put.py` & `aerospike-9.0.0/examples/client/put.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/put_async.py` & `aerospike-9.0.0/examples/client/put_async.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/query.py` & `aerospike-9.0.0/examples/client/query.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/query_apply.py` & `aerospike-9.0.0/examples/client/query_apply.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/remove.py` & `aerospike-9.0.0/examples/client/remove.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/remove_bin.py` & `aerospike-9.0.0/examples/client/remove_bin.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/scan.py` & `aerospike-9.0.0/examples/client/scan.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/scan_apply.py` & `aerospike-9.0.0/examples/client/scan_apply.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/scan_info.py` & `aerospike-9.0.0/examples/client/scan_info.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/scan_partition.py` & `aerospike-9.0.0/examples/client/scan_partition.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/select_many.py` & `aerospike-9.0.0/examples/client/select_many.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/select_record.py` & `aerospike-9.0.0/examples/client/select_record.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/simple.lua` & `aerospike-9.0.0/examples/client/simple.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/stream_example.lua` & `aerospike-9.0.0/examples/client/stream_example.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/touch.py` & `aerospike-9.0.0/examples/client/touch.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/ttl.py` & `aerospike-9.0.0/examples/client/ttl.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/udf_get.py` & `aerospike-9.0.0/examples/client/udf_get.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/udf_list.py` & `aerospike-9.0.0/examples/client/udf_list.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/udf_put.py` & `aerospike-9.0.0/examples/client/udf_put.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/udf_remove.py` & `aerospike-9.0.0/examples/client/udf_remove.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/client/unicode_smiles.py` & `aerospike-9.0.0/examples/client/unicode_smiles.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/deprecated/exists.py` & `aerospike-9.0.0/examples/deprecated/exists.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/deprecated/get.py` & `aerospike-9.0.0/examples/deprecated/get.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/deprecated/put.py` & `aerospike-9.0.0/examples/deprecated/put.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/examples/deprecated/remove.py` & `aerospike-9.0.0/examples/deprecated/remove.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/pyproject.toml` & `aerospike-9.0.0/pyproject.toml`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/scripts/manylinux2014build.sh` & `aerospike-9.0.0/scripts/manylinux2014build.sh`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/scripts/os_version` & `aerospike-9.0.0/scripts/os_version`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/scripts/wait-for-node.sh` & `aerospike-9.0.0/scripts/wait-for-node.sh`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/setup.py` & `aerospike-9.0.0/setup.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/admin.h` & `aerospike-9.0.0/src/include/admin.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/bit_operations.h` & `aerospike-9.0.0/src/include/bit_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/cdt_list_operations.h` & `aerospike-9.0.0/src/include/cdt_list_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/cdt_map_operations.h` & `aerospike-9.0.0/src/include/cdt_map_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/cdt_operation_utils.h` & `aerospike-9.0.0/src/include/cdt_operation_utils.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/cdt_types.h` & `aerospike-9.0.0/src/include/cdt_types.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/client.h` & `aerospike-9.0.0/src/include/client.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/conversions.h` & `aerospike-9.0.0/src/include/conversions.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/exception_types.h` & `aerospike-9.0.0/src/include/exception_types.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/exceptions.h` & `aerospike-9.0.0/src/include/exceptions.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/expression_operations.h` & `aerospike-9.0.0/src/include/expression_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/geo.h` & `aerospike-9.0.0/src/include/geo.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/global_hosts.h` & `aerospike-9.0.0/src/include/global_hosts.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/hll_operations.h` & `aerospike-9.0.0/src/include/hll_operations.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/key_ordered_dict.h` & `aerospike-9.0.0/src/include/key_ordered_dict.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/log.h` & `aerospike-9.0.0/src/include/log.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/macros.h` & `aerospike-9.0.0/src/include/macros.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/module_functions.h` & `aerospike-9.0.0/src/include/module_functions.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/nullobject.h` & `aerospike-9.0.0/src/include/nullobject.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/operate.h` & `aerospike-9.0.0/src/include/operate.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/policy.h` & `aerospike-9.0.0/src/include/policy.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/policy_config.h` & `aerospike-9.0.0/src/include/policy_config.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/pool.h` & `aerospike-9.0.0/src/include/pool.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/predicates.h` & `aerospike-9.0.0/src/include/predicates.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/query.h` & `aerospike-9.0.0/src/include/query.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/scan.h` & `aerospike-9.0.0/src/include/scan.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/serializer.h` & `aerospike-9.0.0/src/include/serializer.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/tls_config.h` & `aerospike-9.0.0/src/include/tls_config.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/tls_info_host.h` & `aerospike-9.0.0/src/include/tls_info_host.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/include/types.h` & `aerospike-9.0.0/src/include/types.h`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/aerospike.c` & `aerospike-9.0.0/src/main/aerospike.c`

 * *Files 0% similar despite different names*

```diff
@@ -149,15 +149,15 @@
 
     return 0;
 }
 
 MOD_INIT(aerospike)
 {
 
-    const char version[8] = "8.0.0";
+    const char version[8] = "9.0.0";
     // Makes things "thread-safe"
     PyEval_InitThreads();
     int i = 0;
 
     // aerospike Module
     PyObject *aerospike;
```

### Comparing `aerospike-8.0.0/src/main/calc_digest.c` & `aerospike-9.0.0/src/main/calc_digest.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/cdt_types/type.c` & `aerospike-9.0.0/src/main/cdt_types/type.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/admin.c` & `aerospike-9.0.0/src/main/client/admin.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/apply.c` & `aerospike-9.0.0/src/main/client/apply.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/batch_apply.c` & `aerospike-9.0.0/src/main/client/batch_apply.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/batch_get_ops.c` & `aerospike-9.0.0/src/main/client/batch_get_ops.c`

 * *Files 5% similar despite different names*

```diff
@@ -103,22 +103,21 @@
  * This function invokes csdk's API's.
  *
  * @param self                  AerospikeClient object
  * @param err                   The as_error to be populated by the function
  *                              with the encountered error if any.
  * @param py_keys                   The list containing keys.
  * @param py_ops               The list containing op, bin and value.
- * @param py_meta               The metadata for the operation.
  * @param py_policy      		Python dict used to populate the operate_policy or map_policy.
  *******************************************************************************************************
  */
 static PyObject *
 AerospikeClient_Batch_GetOps_Invoke(AerospikeClient *self, as_error *err,
                                     PyObject *py_keys, PyObject *py_ops,
-                                    PyObject *py_meta, PyObject *py_policy)
+                                    PyObject *py_policy)
 {
     long operation;
     long return_type = -1;
     as_policy_batch policy;
     as_policy_batch *batch_policy_p = NULL;
     PyObject *py_results = NULL;
     as_batch batch;
@@ -143,20 +142,14 @@
             goto CLEANUP;
         }
     }
 
     as_static_pool static_pool;
     memset(&static_pool, 0, sizeof(static_pool));
 
-    if (py_meta) {
-        if (check_and_set_meta(py_meta, &ops, err) != AEROSPIKE_OK) {
-            goto CLEANUP;
-        }
-    }
-
     for (int i = 0; i < ops_size; i++) {
         PyObject *py_val = PyList_GetItem(py_ops, i);
 
         if (PyDict_Check(py_val)) {
             if (add_op(self, err, py_val, unicodeStrVector, &static_pool, &ops,
                        &operation, &return_type) != AEROSPIKE_OK) {
                 goto CLEANUP;
@@ -236,37 +229,35 @@
  *******************************************************************************************************
  */
 PyObject *AerospikeClient_Batch_GetOps(AerospikeClient *self, PyObject *args,
                                        PyObject *kwds)
 {
     as_error err;
     PyObject *py_policy = NULL;
-    PyObject *py_meta = NULL;
     PyObject *py_keys = NULL;
     PyObject *py_ops = NULL;
     PyObject *py_results = NULL;
 
     as_error_init(&err);
 
     // Python Function Keyword Arguments
-    static char *kwlist[] = {"keys", "list", "meta", "policy", NULL};
-    if (PyArg_ParseTupleAndKeywords(args, kwds, "OO|OO:batch_getops", kwlist,
-                                    &py_keys, &py_ops, &py_meta,
-                                    &py_policy) == false) {
+    static char *kwlist[] = {"keys", "list", "policy", NULL};
+    if (PyArg_ParseTupleAndKeywords(args, kwds, "OO|O:batch_getops", kwlist,
+                                    &py_keys, &py_ops, &py_policy) == false) {
         return NULL;
     }
 
     if (!py_keys || !PyList_Check(py_keys) || !py_ops ||
         !PyList_Check(py_ops)) {
         as_error_update(&err, AEROSPIKE_ERR_PARAM,
                         "batch_getops keys/ops should be of type list");
     }
 
     py_results = AerospikeClient_Batch_GetOps_Invoke(
-        self, &err, py_keys, py_ops, py_meta, py_policy);
+        self, &err, py_keys, py_ops, py_policy);
 
     if (py_results == NULL) {
         PyObject *py_err = NULL;
         error_to_pyobject(&err, &py_err);
         PyObject *exception_type = raise_exception(&err);
         PyErr_SetObject(exception_type, py_err);
         Py_DECREF(py_err);
```

### Comparing `aerospike-8.0.0/src/main/client/batch_operate.c` & `aerospike-9.0.0/src/main/client/batch_operate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/batch_remove.c` & `aerospike-9.0.0/src/main/client/batch_remove.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/batch_write.c` & `aerospike-9.0.0/src/main/client/batch_write.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/bit_operate.c` & `aerospike-9.0.0/src/main/client/bit_operate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/cdt_list_operate.c` & `aerospike-9.0.0/src/main/client/cdt_list_operate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/cdt_map_operate.c` & `aerospike-9.0.0/src/main/client/cdt_map_operate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/cdt_operation_utils.c` & `aerospike-9.0.0/src/main/client/cdt_operation_utils.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/close.c` & `aerospike-9.0.0/src/main/client/close.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/connect.c` & `aerospike-9.0.0/src/main/client/connect.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/exists.c` & `aerospike-9.0.0/src/main/client/exists.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/exists_many.c` & `aerospike-9.0.0/src/main/client/exists_many.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/expression_operations.c` & `aerospike-9.0.0/src/main/client/expression_operations.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/get.c` & `aerospike-9.0.0/src/main/client/get.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/get_async.c` & `aerospike-9.0.0/src/main/client/get_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/get_cdtctx_base64.c` & `aerospike-9.0.0/src/main/client/get_cdtctx_base64.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/get_expression_base64.c` & `aerospike-9.0.0/src/main/client/get_expression_base64.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/get_key_digest.c` & `aerospike-9.0.0/src/main/client/get_key_digest.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/get_key_partition_id.c` & `aerospike-9.0.0/src/main/client/get_key_partition_id.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/get_many.c` & `aerospike-9.0.0/src/main/client/get_many.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/get_nodes.c` & `aerospike-9.0.0/src/main/client/get_nodes.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/hll_operate.c` & `aerospike-9.0.0/src/main/client/hll_operate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/info.c` & `aerospike-9.0.0/src/main/client/info.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/info_node.c` & `aerospike-9.0.0/src/main/client/info_node.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/info_random_node.c` & `aerospike-9.0.0/src/main/client/info_random_node.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/info_single_node.c` & `aerospike-9.0.0/src/main/client/info_single_node.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/operate.c` & `aerospike-9.0.0/src/main/client/operate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/operate_list.c` & `aerospike-9.0.0/src/main/client/operate_list.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/operate_map.c` & `aerospike-9.0.0/src/main/client/operate_map.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/put.c` & `aerospike-9.0.0/src/main/client/put.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/put_async.c` & `aerospike-9.0.0/src/main/client/put_async.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/query.c` & `aerospike-9.0.0/src/main/client/query.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/remove.c` & `aerospike-9.0.0/src/main/client/remove.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/remove_bin.c` & `aerospike-9.0.0/src/main/client/remove_bin.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/scan.c` & `aerospike-9.0.0/src/main/client/scan.c`

 * *Files 1% similar despite different names*

```diff
@@ -207,23 +207,18 @@
                 if (err.code != AEROSPIKE_OK) {
                     goto CLEANUP;
                 }
             }
             Py_BEGIN_ALLOW_THREADS
             aerospike_scan_wait(self->as, &err, info_policy_p, scan_id, 0);
             Py_END_ALLOW_THREADS
-            if (err.code != AEROSPIKE_OK) {
-                as_error_update(&err, AEROSPIKE_ERR_PARAM,
-                                "Unable to perform scan_wait on the scan");
-            }
+            // We don't need to jump to the cleanup section to handle the code
+            // since it's already directly below this block
         }
     }
-    else {
-        goto CLEANUP;
-    }
 
 CLEANUP:
 
     if (exp_list_p) {
         as_exp_destroy(exp_list_p);
         ;
     }
```

### Comparing `aerospike-8.0.0/src/main/client/sec_index.c` & `aerospike-9.0.0/src/main/client/sec_index.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/select.c` & `aerospike-9.0.0/src/main/client/select.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/select_many.c` & `aerospike-9.0.0/src/main/client/select_many.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/set_xdr_filter.c` & `aerospike-9.0.0/src/main/client/set_xdr_filter.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/tls_info_host.c` & `aerospike-9.0.0/src/main/client/tls_info_host.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/truncate.c` & `aerospike-9.0.0/src/main/client/truncate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/client/type.c` & `aerospike-9.0.0/src/main/client/type.c`

 * *Files 1% similar despite different names*

```diff
@@ -901,15 +901,15 @@
     as_error constructor_err;
     as_error_init(&constructor_err);
     static char *kwlist[] = {"config", NULL};
 
     self->has_connected = false;
     self->use_shared_connection = false;
     self->as = NULL;
-    self->send_bool_as = SEND_BOOL_AS_PY_BYTES;
+    self->send_bool_as = SEND_BOOL_AS_AS_BOOL;
 
     if (PyArg_ParseTupleAndKeywords(args, kwds, "O:client", kwlist,
                                     &py_config) == false) {
         error_code = INIT_NO_CONFIG_ERR;
         goto CONSTRUCTOR_ERROR;
     }
```

### Comparing `aerospike-8.0.0/src/main/client/udf.c` & `aerospike-9.0.0/src/main/client/udf.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/conversions.c` & `aerospike-9.0.0/src/main/conversions.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/convert_expressions.c` & `aerospike-9.0.0/src/main/convert_expressions.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/convert_partition_filter.c` & `aerospike-9.0.0/src/main/convert_partition_filter.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/exception.c` & `aerospike-9.0.0/src/main/exception.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/geospatial/dumps.c` & `aerospike-9.0.0/src/main/geospatial/dumps.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/geospatial/loads.c` & `aerospike-9.0.0/src/main/geospatial/loads.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/geospatial/type.c` & `aerospike-9.0.0/src/main/geospatial/type.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/geospatial/unwrap.c` & `aerospike-9.0.0/src/main/geospatial/unwrap.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/geospatial/wrap.c` & `aerospike-9.0.0/src/main/geospatial/wrap.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/global_hosts/type.c` & `aerospike-9.0.0/src/main/global_hosts/type.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/key_ordered_dict/type.c` & `aerospike-9.0.0/src/main/key_ordered_dict/type.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/log.c` & `aerospike-9.0.0/src/main/log.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/nullobject/type.c` & `aerospike-9.0.0/src/main/nullobject/type.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/policy.c` & `aerospike-9.0.0/src/main/policy.c`

 * *Files 1% similar despite different names*

```diff
@@ -451,14 +451,15 @@
     {AS_BYTES_BLOB, "AS_BYTES_BLOB"},
     {AS_BYTES_JAVA, "AS_BYTES_JAVA"},
     {AS_BYTES_CSHARP, "AS_BYTES_CSHARP"},
     {AS_BYTES_PYTHON, "AS_BYTES_PYTHON"},
     {AS_BYTES_RUBY, "AS_BYTES_RUBY"},
     {AS_BYTES_PHP, "AS_BYTES_PHP"},
     {AS_BYTES_ERLANG, "AS_BYTES_ERLANG"},
+    {AS_BYTES_BOOL, "AS_BYTES_BOOL"},
     {AS_BYTES_HLL, "AS_BYTES_HLL"},
     {AS_BYTES_MAP, "AS_BYTES_MAP"},
     {AS_BYTES_LIST, "AS_BYTES_LIST"},
     {AS_BYTES_GEOJSON, "AS_BYTES_GEOJSON"},
     {AS_BYTES_TYPE_MAX, "AS_BYTES_TYPE_MAX"},
 
     /* Regex constants from predexp, still used by expressions */
```

### Comparing `aerospike-8.0.0/src/main/policy_config.c` & `aerospike-9.0.0/src/main/policy_config.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/predicates.c` & `aerospike-9.0.0/src/main/predicates.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/add_ops.c` & `aerospike-9.0.0/src/main/query/add_ops.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/apply.c` & `aerospike-9.0.0/src/main/query/apply.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/execute_background.c` & `aerospike-9.0.0/src/main/query/execute_background.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/foreach.c` & `aerospike-9.0.0/src/main/query/foreach.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/get_parts.c` & `aerospike-9.0.0/src/main/query/get_parts.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/paginate.c` & `aerospike-9.0.0/src/main/query/paginate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/results.c` & `aerospike-9.0.0/src/main/query/results.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/select.c` & `aerospike-9.0.0/src/main/query/select.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/type.c` & `aerospike-9.0.0/src/main/query/type.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/query/where.c` & `aerospike-9.0.0/src/main/query/where.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/scan/add_ops.c` & `aerospike-9.0.0/src/main/scan/add_ops.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/scan/apply.c` & `aerospike-9.0.0/src/main/scan/apply.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/scan/execute_background.c` & `aerospike-9.0.0/src/main/scan/execute_background.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/scan/foreach.c` & `aerospike-9.0.0/src/main/scan/foreach.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/scan/get_parts.c` & `aerospike-9.0.0/src/main/scan/get_parts.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/scan/paginate.c` & `aerospike-9.0.0/src/main/scan/paginate.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/scan/results.c` & `aerospike-9.0.0/src/main/scan/results.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/scan/select.c` & `aerospike-9.0.0/src/main/scan/select.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/scan/type.c` & `aerospike-9.0.0/src/main/scan/type.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/serializer.c` & `aerospike-9.0.0/src/main/serializer.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/src/main/tls_config.c` & `aerospike-9.0.0/src/main/tls_config.c`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/README.md` & `aerospike-9.0.0/test/README.md`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/bin_lua.lua` & `aerospike-9.0.0/test/bin_lua.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/counter26.py` & `aerospike-9.0.0/test/counter26.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/as_errors.py` & `aerospike-9.0.0/test/new_tests/as_errors.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/as_status_codes.py` & `aerospike-9.0.0/test/new_tests/as_status_codes.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/conftest.py` & `aerospike-9.0.0/test/new_tests/conftest.py`

 * *Files 0% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import socket
 import time
 import os
 import sys
 from distutils.version import LooseVersion
 
 import pytest
-from _pytest.terminal import TerminalReporter
+from _pytest.terminal import TerminalReporter  # noqa: F401
 from collections import namedtuple
 from itertools import groupby
 import tracemalloc
 
 from . import invalid_data
 from .test_base_class import TestBaseClass
```

### Comparing `aerospike-8.0.0/test/new_tests/index_helpers.py` & `aerospike-9.0.0/test/new_tests/index_helpers.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_change_password.py` & `aerospike-9.0.0/test/new_tests/test_admin_change_password.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_create_role.py` & `aerospike-9.0.0/test/new_tests/test_admin_create_role.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_create_user.py` & `aerospike-9.0.0/test/new_tests/test_admin_create_user.py`

 * *Files 2% similar despite different names*

```diff
@@ -319,15 +319,18 @@
         assert status == 0
 
         config = self.connection_config
 
         non_admin_client = None
 
         try:
-            non_admin_client = aerospike.client(config).connect("non_admin_test", "non_admin_test")
+            # Close and reconnect with non_admin_test user
+            non_admin_client = aerospike.client(config)
+            non_admin_client.close()
+            non_admin_client.connect("non_admin_test", "non_admin_test")
             status = non_admin_client.admin_create_user("user78", password, roles, policy)
 
             if non_admin_client:
                 non_admin_client.close()
 
         except e.RoleViolation as exception:
             assert exception.code == 81
```

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_drop_role.py` & `aerospike-9.0.0/test/new_tests/test_admin_drop_role.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_drop_user.py` & `aerospike-9.0.0/test/new_tests/test_admin_drop_user.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_get_role.py` & `aerospike-9.0.0/test/new_tests/test_admin_get_role.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_get_roles.py` & `aerospike-9.0.0/test/new_tests/test_admin_get_roles.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_grant_privileges.py` & `aerospike-9.0.0/test/new_tests/test_admin_grant_privileges.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_grant_roles.py` & `aerospike-9.0.0/test/new_tests/test_admin_grant_roles.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_query_role.py` & `aerospike-9.0.0/test/new_tests/test_admin_query_role.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_query_roles.py` & `aerospike-9.0.0/test/new_tests/test_admin_query_roles.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_query_user.py` & `aerospike-9.0.0/test/new_tests/test_admin_query_user.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_query_user_info.py` & `aerospike-9.0.0/test/new_tests/test_admin_query_user_info.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_query_users.py` & `aerospike-9.0.0/test/new_tests/test_admin_query_users.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_query_users_info.py` & `aerospike-9.0.0/test/new_tests/test_admin_query_users_info.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_revoke_privileges.py` & `aerospike-9.0.0/test/new_tests/test_admin_revoke_privileges.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_revoke_roles.py` & `aerospike-9.0.0/test/new_tests/test_admin_revoke_roles.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_set_password.py` & `aerospike-9.0.0/test/new_tests/test_admin_set_password.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_set_quotas.py` & `aerospike-9.0.0/test/new_tests/test_admin_set_quotas.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_admin_set_whitelist.py` & `aerospike-9.0.0/test/new_tests/test_admin_set_whitelist.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_aggregate.py` & `aerospike-9.0.0/test/new_tests/test_aggregate.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_append.py` & `aerospike-9.0.0/test/new_tests/test_append.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_apply.py` & `aerospike-9.0.0/test/new_tests/test_apply.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_arithmetic_expressions.py` & `aerospike-9.0.0/test/new_tests/test_arithmetic_expressions.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_base_class.py` & `aerospike-9.0.0/test/new_tests/test_base_class.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_batch_apply.py` & `aerospike-9.0.0/test/new_tests/test_batch_apply.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_batch_get_ops.py` & `aerospike-9.0.0/test/new_tests/test_batch_get_ops.py`

 * *Files 1% similar despite different names*

```diff
@@ -82,18 +82,17 @@
         ],
     )
     def test_read_pos(self, expr, flags, name, expected):
         """
         Test expression read operation with correct parameters.
         """
         ops = [expressions.expression_read(name, expr.compile(), flags)]
-        meta = {"gen": 1}
         policy = {"timeout": 1001}
 
-        res = self.as_connection.batch_get_ops(self.keys, ops, meta, policy)
+        res = self.as_connection.batch_get_ops(self.keys, ops, policy)
         """
         res are in the format of (status-tuple, ((meta-dict, result-dict), status-tuple, exception), ...)
         """
         # print(res)
         for i in range(self.rec_count):
             assert res[0][2] == expected
```

### Comparing `aerospike-8.0.0/test/new_tests/test_batch_operate.py` & `aerospike-9.0.0/test/new_tests/test_batch_operate.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_batch_records.py` & `aerospike-9.0.0/test/new_tests/test_batch_records.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_batch_remove.py` & `aerospike-9.0.0/test/new_tests/test_batch_remove.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_batch_write.py` & `aerospike-9.0.0/test/new_tests/test_batch_write.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_bitwise_operations.py` & `aerospike-9.0.0/test/new_tests/test_bitwise_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_bool_config.py` & `aerospike-9.0.0/test/new_tests/test_bool_config.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_calc_digest.py` & `aerospike-9.0.0/test/new_tests/test_calc_digest.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_cdt_compators.py` & `aerospike-9.0.0/test/new_tests/test_cdt_compators.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_cdt_index.py` & `aerospike-9.0.0/test/new_tests/test_cdt_index.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_close.py` & `aerospike-9.0.0/test/new_tests/test_close.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_compress.py` & `aerospike-9.0.0/test/new_tests/test_compress.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_connect.py` & `aerospike-9.0.0/test/new_tests/test_connect.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_connect_memleak.py` & `aerospike-9.0.0/test/new_tests/test_connect_memleak.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_data.py` & `aerospike-9.0.0/test/new_tests/test_data.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_error_codes.py` & `aerospike-9.0.0/test/new_tests/test_error_codes.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_exists.py` & `aerospike-9.0.0/test/new_tests/test_exists.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_exists_many.py` & `aerospike-9.0.0/test/new_tests/test_exists_many.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_expression_operations.py` & `aerospike-9.0.0/test/new_tests/test_expression_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_expressions_base.py` & `aerospike-9.0.0/test/new_tests/test_expressions_base.py`

 * *Files 3% similar despite different names*

```diff
@@ -328,7 +328,33 @@
         if self.server_version < [5, 6]:
             pytest.mark.xfail(reason="Servers older than 5.6 do not support 6.0.0 expressions")
             pytest.xfail()
 
         expr = Cond(GT(IntBin("age"), _NUM_RECORDS), True, Unknown())
         with pytest.raises(e.FilteredOut):
             self.as_connection.get(("test", "demo", _NUM_RECORDS - 1), policy={"expressions": expr.compile()})
+
+    def test_bintype_as_bool(self):
+        if self.server_version < [5, 6]:
+            pytest.mark.xfail(reason="Servers older than 5.6 do not support 6.0.0 expressions")
+            pytest.xfail()
+
+        # Configure client to encode and send booleans as the server boolean type
+        config = TestBaseClass.get_connection_config()
+        config["send_bool_as"] = aerospike.AS_BOOL
+        test_client = aerospike.client(config).connect(config["user"], config["password"])
+
+        # Override record 0's "t" bin to be a server bool instead of a python bool
+        key = ("test", "demo", 0)
+        bins = {"t": True}
+        test_client.put(key, bins)
+
+        # Check that record 0 has a server boolean bin named "t"
+        expr = Eq(BinType("t"), aerospike.AS_BYTES_BOOL).compile()
+        records = test_client.get_many([key], {"expressions": expr})
+
+        # bins would be None if the record was filtered out by the expression
+        record = records[0]
+        bins = record[2]
+        assert bins
+
+        test_client.close()
```

### Comparing `aerospike-8.0.0/test/new_tests/test_expressions_bit.py` & `aerospike-9.0.0/test/new_tests/test_expressions_bit.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_expressions_bitwise_operators.py` & `aerospike-9.0.0/test/new_tests/test_expressions_bitwise_operators.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_expressions_everywhere.py` & `aerospike-9.0.0/test/new_tests/test_expressions_everywhere.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_expressions_hll.py` & `aerospike-9.0.0/test/new_tests/test_expressions_hll.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_expressions_list.py` & `aerospike-9.0.0/test/new_tests/test_expressions_list.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_expressions_map.py` & `aerospike-9.0.0/test/new_tests/test_expressions_map.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_geospatial.py` & `aerospike-9.0.0/test/new_tests/test_geospatial.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_get_async.py` & `aerospike-9.0.0/test/new_tests/test_get_async.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_get_cdtctx_base64.py` & `aerospike-9.0.0/test/new_tests/test_get_cdtctx_base64.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_get_expression_base64r.py` & `aerospike-9.0.0/test/new_tests/test_get_expression_base64r.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_get_key_digest.py` & `aerospike-9.0.0/test/new_tests/test_get_key_digest.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_get_many.py` & `aerospike-9.0.0/test/new_tests/test_get_many.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_get_node_names.py` & `aerospike-9.0.0/test/new_tests/test_get_node_names.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_get_nodes.py` & `aerospike-9.0.0/test/new_tests/test_get_nodes.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_get_put.py` & `aerospike-9.0.0/test/new_tests/test_get_put.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_get_udf.py` & `aerospike-9.0.0/test/new_tests/test_get_udf.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_hll.py` & `aerospike-9.0.0/test/new_tests/test_hll.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_increment.py` & `aerospike-9.0.0/test/new_tests/test_increment.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_index.py` & `aerospike-9.0.0/test/new_tests/test_index.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_info.py` & `aerospike-9.0.0/test/new_tests/test_info.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_info_all.py` & `aerospike-9.0.0/test/new_tests/test_info_all.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_info_random_node.py` & `aerospike-9.0.0/test/new_tests/test_info_random_node.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_info_single_node.py` & `aerospike-9.0.0/test/new_tests/test_info_single_node.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_invalid_conf.py` & `aerospike-9.0.0/test/new_tests/test_invalid_conf.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_inverted_map_operations.py` & `aerospike-9.0.0/test/new_tests/test_inverted_map_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_is_connected.py` & `aerospike-9.0.0/test/new_tests/test_is_connected.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_job_info.py` & `aerospike-9.0.0/test/new_tests/test_job_info.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_key_digest.py` & `aerospike-9.0.0/test/new_tests/test_key_digest.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_key_ordered_dict_get_by_value.py` & `aerospike-9.0.0/test/new_tests/test_key_ordered_dict_get_by_value.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_kv.py` & `aerospike-9.0.0/test/new_tests/test_kv.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_append.py` & `aerospike-9.0.0/test/new_tests/test_list_append.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_basics.py` & `aerospike-9.0.0/test/new_tests/test_list_basics.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_clear.py` & `aerospike-9.0.0/test/new_tests/test_list_clear.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_extend.py` & `aerospike-9.0.0/test/new_tests/test_list_extend.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_get.py` & `aerospike-9.0.0/test/new_tests/test_list_get.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_get_range.py` & `aerospike-9.0.0/test/new_tests/test_list_get_range.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_index.py` & `aerospike-9.0.0/test/new_tests/test_list_index.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_insert.py` & `aerospike-9.0.0/test/new_tests/test_list_insert.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_insert_items.py` & `aerospike-9.0.0/test/new_tests/test_list_insert_items.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_pop.py` & `aerospike-9.0.0/test/new_tests/test_list_pop.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_pop_range.py` & `aerospike-9.0.0/test/new_tests/test_list_pop_range.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_remove.py` & `aerospike-9.0.0/test/new_tests/test_list_remove.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_remove_range.py` & `aerospike-9.0.0/test/new_tests/test_list_remove_range.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_set.py` & `aerospike-9.0.0/test/new_tests/test_list_set.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_size.py` & `aerospike-9.0.0/test/new_tests/test_list_size.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_list_trim.py` & `aerospike-9.0.0/test/new_tests/test_list_trim.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_log.py` & `aerospike-9.0.0/test/new_tests/test_log.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_map_basics.py` & `aerospike-9.0.0/test/new_tests/test_map_basics.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_map_operation_helpers.py` & `aerospike-9.0.0/test/new_tests/test_map_operation_helpers.py`

 * *Files 0% similar despite different names*

```diff
@@ -55,14 +55,16 @@
 class TestNewListOperationsHelpers(object):
     @pytest.fixture(autouse=True)
     def setup(self, request, as_connection):
         """
         Setup Method
         """
         self.keys = []
+        # In a CDT, different types are also ordered from each other
+        # boolean < integer
         self.test_map = {"a": 5, "b": 4, "c": 3, "d": 2, "e": 1, "f": True, "g": False}
 
         self.test_key = "test", "demo", "new_map_op"
         self.test_bin = "map"
         self.as_connection.put(self.test_key, {self.test_bin: self.test_map})
         self.keys.append(self.test_key)
 
@@ -209,25 +211,28 @@
         res_map = self.as_connection.get(self.test_key)[2][self.test_bin]
         assert "b" not in res_map
         assert "c" not in res_map
 
     def test_map_remove_by_rank(self):
         operations = [map_ops.map_remove_by_rank(self.test_bin, 1, return_type=aerospike.MAP_RETURN_KEY)]
         ret_vals = get_map_result_from_operation(self.as_connection, self.test_key, operations, self.test_bin)
-        assert ret_vals == "d"
+        # True > False
+        assert ret_vals == "f"
         res_map = self.as_connection.get(self.test_key)[2][self.test_bin]
-        assert "d" not in res_map
+        assert "f" not in res_map
 
     def test_map_remove_by_rank_range(self):
         operations = [map_ops.map_remove_by_rank_range(self.test_bin, 1, 2, return_type=aerospike.MAP_RETURN_KEY)]
         ret_vals = get_map_result_from_operation(self.as_connection, self.test_key, operations, self.test_bin)
-        assert set(ret_vals) == set(["d", "c"])
+        # f: True, e: 1
+        # Removes 2 items from rank 1 and going up the rank
+        assert set(ret_vals) == set(["e", "f"])
         res_map = self.as_connection.get(self.test_key)[2][self.test_bin]
-        assert "d" not in res_map
-        assert "c" not in res_map
+        assert "e" not in res_map
+        assert "f" not in res_map
 
     def test_map_get_by_key(self):
         operations = [map_ops.map_get_by_key(self.test_bin, "a", return_type=aerospike.MAP_RETURN_VALUE)]
         assert (
             get_map_result_from_operation(self.as_connection, self.test_key, operations, self.test_bin)
             == self.test_map["a"]
         )
@@ -279,21 +284,21 @@
         operations = [map_ops.map_get_by_index_range(self.test_bin, 1, 2, return_type=aerospike.MAP_RETURN_KEY)]
         ret_vals = get_map_result_from_operation(self.as_connection, self.test_key, operations, self.test_bin)
         assert ret_vals == ["b", "c"]
 
     def test_map_get_by_rank(self):
         operations = [map_ops.map_get_by_rank(self.test_bin, 1, return_type=aerospike.MAP_RETURN_KEY)]
         ret_vals = get_map_result_from_operation(self.as_connection, self.test_key, operations, self.test_bin)
-        assert ret_vals == "d"
+        assert ret_vals == "f"
 
     def test_map_get_by_rank_range(self):
         sort_map(self.as_connection, self.test_key, self.test_bin)
         operations = [map_ops.map_get_by_rank_range(self.test_bin, 1, 2, return_type=aerospike.MAP_RETURN_KEY)]
         ret_vals = get_map_result_from_operation(self.as_connection, self.test_key, operations, self.test_bin)
-        assert ret_vals == ["d", "c"]
+        assert ret_vals == ["f", "e"]
 
     def test_map_get_exists_by_key_list(self):
         if not Server61:
             pytest.skip("It only applies to >= 6.1 enterprise edition")
         operations = [
             map_ops.map_get_by_key_list(self.test_bin, ["a", "b", "c"], return_type=aerospike.MAP_RETURN_EXISTS)
         ]
```

### Comparing `aerospike-8.0.0/test/new_tests/test_map_write_flags.py` & `aerospike-9.0.0/test/new_tests/test_map_write_flags.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_map_write_mode.py` & `aerospike-9.0.0/test/new_tests/test_map_write_mode.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_mapkeys_index.py` & `aerospike-9.0.0/test/new_tests/test_mapkeys_index.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_mapvalues_index.py` & `aerospike-9.0.0/test/new_tests/test_mapvalues_index.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_nested_cdt_ctx.py` & `aerospike-9.0.0/test/new_tests/test_nested_cdt_ctx.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_new_constructor.py` & `aerospike-9.0.0/test/new_tests/test_new_constructor.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_new_list_operation_helpers.py` & `aerospike-9.0.0/test/new_tests/test_new_list_operation_helpers.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_new_list_operations.py` & `aerospike-9.0.0/test/new_tests/test_new_list_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_operate.py` & `aerospike-9.0.0/test/new_tests/test_operate.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_operate_helpers.py` & `aerospike-9.0.0/test/new_tests/test_operate_helpers.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_operate_map.py` & `aerospike-9.0.0/test/new_tests/test_operate_map.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_operate_ordered.py` & `aerospike-9.0.0/test/new_tests/test_operate_ordered.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_predicates.py` & `aerospike-9.0.0/test/new_tests/test_predicates.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_prepend.py` & `aerospike-9.0.0/test/new_tests/test_prepend.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_put_async.py` & `aerospike-9.0.0/test/new_tests/test_put_async.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_query.py` & `aerospike-9.0.0/test/new_tests/test_query.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_query_apply.py` & `aerospike-9.0.0/test/new_tests/test_query_apply.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_query_execute_background.py` & `aerospike-9.0.0/test/new_tests/test_query_execute_background.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_query_expressions.py` & `aerospike-9.0.0/test/new_tests/test_query_expressions.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_query_get_partitions_status.py` & `aerospike-9.0.0/test/new_tests/test_query_get_partitions_status.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_query_pagination.py` & `aerospike-9.0.0/test/new_tests/test_query_pagination.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_query_partition.py` & `aerospike-9.0.0/test/new_tests/test_query_partition.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_relative_cdt_operations.py` & `aerospike-9.0.0/test/new_tests/test_relative_cdt_operations.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_remove.py` & `aerospike-9.0.0/test/new_tests/test_remove.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_remove_bin.py` & `aerospike-9.0.0/test/new_tests/test_remove_bin.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_scan.py` & `aerospike-9.0.0/test/new_tests/test_scan.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_scan_apply.py` & `aerospike-9.0.0/test/new_tests/test_scan_apply.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_scan_execute_background.py` & `aerospike-9.0.0/test/new_tests/test_scan_execute_background.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_scan_get_partitions_status.py` & `aerospike-9.0.0/test/new_tests/test_scan_get_partitions_status.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_scan_pagination.py` & `aerospike-9.0.0/test/new_tests/test_scan_pagination.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_scan_partition.py` & `aerospike-9.0.0/test/new_tests/test_scan_partition.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_select.py` & `aerospike-9.0.0/test/new_tests/test_select.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_select_many.py` & `aerospike-9.0.0/test/new_tests/test_select_many.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_set_xdr_filter.py` & `aerospike-9.0.0/test/new_tests/test_set_xdr_filter.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_touch.py` & `aerospike-9.0.0/test/new_tests/test_touch.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_truncate.py` & `aerospike-9.0.0/test/new_tests/test_truncate.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_udf_list.py` & `aerospike-9.0.0/test/new_tests/test_udf_list.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_udf_put.py` & `aerospike-9.0.0/test/new_tests/test_udf_put.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_udf_remove.py` & `aerospike-9.0.0/test/new_tests/test_udf_remove.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_user_serializer.py` & `aerospike-9.0.0/test/new_tests/test_user_serializer.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/test_zserializers.py` & `aerospike-9.0.0/test/new_tests/test_zserializers.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/new_tests/udf_helpers.py` & `aerospike-9.0.0/test/new_tests/udf_helpers.py`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/stream_example.lua` & `aerospike-9.0.0/test/stream_example.lua`

 * *Files identical despite different names*

### Comparing `aerospike-8.0.0/test/test_record_udf.lua` & `aerospike-9.0.0/test/test_record_udf.lua`

 * *Files identical despite different names*

