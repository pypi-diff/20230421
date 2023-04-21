# Comparing `tmp/data-watch-sdk-0.0.1b0.tar.gz` & `tmp/data-watch-sdk-0.0.1b1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data-watch-sdk-0.0.1b0.tar", last modified: Tue Apr 18 15:43:16 2023, max compression
+gzip compressed data, was "data-watch-sdk-0.0.1b1.tar", last modified: Fri Apr 21 19:43:24 2023, max compression
```

## Comparing `data-watch-sdk-0.0.1b0.tar` & `data-watch-sdk-0.0.1b1.tar`

### file list

```diff
@@ -1,104 +1,104 @@
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.935051 data-watch-sdk-0.0.1b0/
--rw-r--r--   0 root         (0) root         (0)      992 2023-04-18 15:43:16.935051 data-watch-sdk-0.0.1b0/PKG-INFO
--rw-rw-rw-   0 root         (0) root         (0)      458 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/README.md
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.912049 data-watch-sdk-0.0.1b0/data_watch/
--rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.912049 data-watch-sdk-0.0.1b0/data_watch/api/
--rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      131 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.912049 data-watch-sdk-0.0.1b0/data_watch/api/service/
--rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.913049 data-watch-sdk-0.0.1b0/data_watch/api/service/auth/
--rw-rw-rw-   0 root         (0) root         (0)      232 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/auth/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1336 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/auth/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2267 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/auth/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1735 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/auth/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.915049 data-watch-sdk-0.0.1b0/data_watch/api/service/group/
--rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1427 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     4316 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      408 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3836 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.917049 data-watch-sdk-0.0.1b0/data_watch/api/service/group/view/
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      257 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      990 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      384 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      894 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/group/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.918049 data-watch-sdk-0.0.1b0/data_watch/api/service/job/
--rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      937 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     2932 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      714 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/model.py
--rw-rw-rw-   0 root         (0) root         (0)     2586 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.920050 data-watch-sdk-0.0.1b0/data_watch/api/service/job/view/
--rw-rw-rw-   0 root         (0) root         (0)      145 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/view/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/view/__util.py
--rw-rw-rw-   0 root         (0) root         (0)      548 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/view/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      476 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/view/model.py
--rw-rw-rw-   0 root         (0) root         (0)      509 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/job/view/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.921050 data-watch-sdk-0.0.1b0/data_watch/api/service/rule/
--rw-rw-rw-   0 root         (0) root         (0)      303 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/rule/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1163 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/rule/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3541 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/rule/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      884 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/rule/model.py
--rw-rw-rw-   0 root         (0) root         (0)     3144 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/api/service/rule/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.923050 data-watch-sdk-0.0.1b0/data_watch/common/
--rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2640 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/base.py
--rw-rw-rw-   0 root         (0) root         (0)      230 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/base_enum.py
--rw-rw-rw-   0 root         (0) root         (0)     2685 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/config.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.923050 data-watch-sdk-0.0.1b0/data_watch/common/date/
--rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/date/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2475 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/date/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.924050 data-watch-sdk-0.0.1b0/data_watch/common/decorators/
--rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.925050 data-watch-sdk-0.0.1b0/data_watch/common/decorators/authorization/
--rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/authorization/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1135 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/authorization/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     3909 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/authorization/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/authorization/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.926050 data-watch-sdk-0.0.1b0/data_watch/common/decorators/data/
--rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/data/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      692 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/data/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1393 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/data/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     1391 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/data/synchronous.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.927050 data-watch-sdk-0.0.1b0/data_watch/common/decorators/serializable/
--rw-rw-rw-   0 root         (0) root         (0)      116 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/serializable/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/serializable/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1902 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/serializable/decorators.py
--rw-rw-rw-   0 root         (0) root         (0)      364 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/decorators/timeit.py
--rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/enum.py
--rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/errors.py
--rw-rw-rw-   0 root         (0) root         (0)     4790 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/function.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.928050 data-watch-sdk-0.0.1b0/data_watch/common/metaclass/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/metaclass/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/metaclass/singleton.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.929050 data-watch-sdk-0.0.1b0/data_watch/common/requests/
--rw-rw-rw-   0 root         (0) root         (0)      395 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/requests/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     4665 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/requests/asynchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     3768 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/requests/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/common/type.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.930050 data-watch-sdk-0.0.1b0/data_watch/pipeline/
--rw-rw-rw-   0 root         (0) root         (0)     4552 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/__init__.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.931050 data-watch-sdk-0.0.1b0/data_watch/pipeline/execution/
--rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/execution/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2558 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/execution/synchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     1655 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/model.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.932051 data-watch-sdk-0.0.1b0/data_watch/pipeline/pandas/
--rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/pandas/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     2518 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/pandas/__util.py
--rw-rw-rw-   0 root         (0) root         (0)     1558 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/pandas/synchronous.py
--rw-rw-rw-   0 root         (0) root         (0)     2659 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/test.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.933051 data-watch-sdk-0.0.1b0/data_watch/pipeline/utils/
--rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/utils/__init__.py
--rw-rw-rw-   0 root         (0) root         (0)     3690 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/utils/asynchronously.py
--rw-rw-rw-   0 root         (0) root         (0)     3547 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/data_watch/pipeline/utils/synchronously.py
-drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-18 15:43:16.934051 data-watch-sdk-0.0.1b0/data_watch_sdk.egg-info/
--rw-r--r--   0 root         (0) root         (0)      992 2023-04-18 15:43:16.000000 data-watch-sdk-0.0.1b0/data_watch_sdk.egg-info/PKG-INFO
--rw-r--r--   0 root         (0) root         (0)     3118 2023-04-18 15:43:16.000000 data-watch-sdk-0.0.1b0/data_watch_sdk.egg-info/SOURCES.txt
--rw-r--r--   0 root         (0) root         (0)        1 2023-04-18 15:43:16.000000 data-watch-sdk-0.0.1b0/data_watch_sdk.egg-info/dependency_links.txt
--rw-r--r--   0 root         (0) root         (0)      212 2023-04-18 15:43:16.000000 data-watch-sdk-0.0.1b0/data_watch_sdk.egg-info/requires.txt
--rw-r--r--   0 root         (0) root         (0)       11 2023-04-18 15:43:16.000000 data-watch-sdk-0.0.1b0/data_watch_sdk.egg-info/top_level.txt
--rw-r--r--   0 root         (0) root         (0)       38 2023-04-18 15:43:16.935051 data-watch-sdk-0.0.1b0/setup.cfg
--rw-rw-rw-   0 root         (0) root         (0)     1348 2023-04-18 15:43:03.000000 data-watch-sdk-0.0.1b0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.583305 data-watch-sdk-0.0.1b1/
+-rw-r--r--   0 root         (0) root         (0)      992 2023-04-21 19:43:24.582305 data-watch-sdk-0.0.1b1/PKG-INFO
+-rw-rw-rw-   0 root         (0) root         (0)      458 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/README.md
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.562303 data-watch-sdk-0.0.1b1/data_watch/
+-rw-rw-rw-   0 root         (0) root         (0)       45 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.562303 data-watch-sdk-0.0.1b1/data_watch/api/
+-rw-rw-rw-   0 root         (0) root         (0)       21 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      275 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.562303 data-watch-sdk-0.0.1b1/data_watch/api/service/
+-rw-rw-rw-   0 root         (0) root         (0)       31 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.564303 data-watch-sdk-0.0.1b1/data_watch/api/service/auth/
+-rw-rw-rw-   0 root         (0) root         (0)      232 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/auth/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1336 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/auth/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2267 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/auth/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1735 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/auth/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.565303 data-watch-sdk-0.0.1b1/data_watch/api/service/group/
+-rw-rw-rw-   0 root         (0) root         (0)      373 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1599 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4820 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      408 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     4295 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.566304 data-watch-sdk-0.0.1b1/data_watch/api/service/group/view/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      257 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      990 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      384 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      894 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/group/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.568304 data-watch-sdk-0.0.1b1/data_watch/api/service/job/
+-rw-rw-rw-   0 root         (0) root         (0)      291 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      937 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     2988 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      842 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     2642 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.569304 data-watch-sdk-0.0.1b1/data_watch/api/service/job/view/
+-rw-rw-rw-   0 root         (0) root         (0)      145 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/view/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)       98 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/view/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)      548 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/view/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      483 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/view/model.py
+-rw-rw-rw-   0 root         (0) root         (0)      509 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/job/view/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.570304 data-watch-sdk-0.0.1b1/data_watch/api/service/rule/
+-rw-rw-rw-   0 root         (0) root         (0)      303 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/rule/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1337 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/rule/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     4046 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/rule/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      812 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/rule/model.py
+-rw-rw-rw-   0 root         (0) root         (0)     3604 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/api/service/rule/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.572304 data-watch-sdk-0.0.1b1/data_watch/common/
+-rw-rw-rw-   0 root         (0) root         (0)       47 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2640 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/base.py
+-rw-rw-rw-   0 root         (0) root         (0)      230 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/base_enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     2685 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/config.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.573304 data-watch-sdk-0.0.1b1/data_watch/common/date/
+-rw-rw-rw-   0 root         (0) root         (0)      202 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/date/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2475 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/date/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.573304 data-watch-sdk-0.0.1b1/data_watch/common/decorators/
+-rw-rw-rw-   0 root         (0) root         (0)      385 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.574304 data-watch-sdk-0.0.1b1/data_watch/common/decorators/authorization/
+-rw-rw-rw-   0 root         (0) root         (0)      236 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/authorization/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1135 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/authorization/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     3909 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/authorization/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3887 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/authorization/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.575304 data-watch-sdk-0.0.1b1/data_watch/common/decorators/data/
+-rw-rw-rw-   0 root         (0) root         (0)      182 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/data/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      692 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/data/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1393 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/data/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     1391 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/data/synchronous.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.576304 data-watch-sdk-0.0.1b1/data_watch/common/decorators/serializable/
+-rw-rw-rw-   0 root         (0) root         (0)      116 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/serializable/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     1001 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/serializable/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1902 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/serializable/decorators.py
+-rw-rw-rw-   0 root         (0) root         (0)      364 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/decorators/timeit.py
+-rw-rw-rw-   0 root         (0) root         (0)      267 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/enum.py
+-rw-rw-rw-   0 root         (0) root         (0)     1299 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/errors.py
+-rw-rw-rw-   0 root         (0) root         (0)     4790 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/function.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.577304 data-watch-sdk-0.0.1b1/data_watch/common/metaclass/
+-rw-rw-rw-   0 root         (0) root         (0)        0 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/metaclass/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)      924 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/metaclass/singleton.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.578304 data-watch-sdk-0.0.1b1/data_watch/common/requests/
+-rw-rw-rw-   0 root         (0) root         (0)      395 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/requests/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4665 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/requests/asynchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     3768 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/requests/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)      241 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/common/type.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.579305 data-watch-sdk-0.0.1b1/data_watch/pipeline/
+-rw-rw-rw-   0 root         (0) root         (0)     4646 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.579305 data-watch-sdk-0.0.1b1/data_watch/pipeline/execution/
+-rw-rw-rw-   0 root         (0) root         (0)       69 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/execution/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2487 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/execution/synchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     1655 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/model.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.580305 data-watch-sdk-0.0.1b1/data_watch/pipeline/pandas/
+-rw-rw-rw-   0 root         (0) root         (0)       73 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/pandas/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     2518 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/pandas/__util.py
+-rw-rw-rw-   0 root         (0) root         (0)     1546 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/pandas/synchronous.py
+-rw-rw-rw-   0 root         (0) root         (0)     2299 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/test.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.581305 data-watch-sdk-0.0.1b1/data_watch/pipeline/utils/
+-rw-rw-rw-   0 root         (0) root         (0)      157 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/utils/__init__.py
+-rw-rw-rw-   0 root         (0) root         (0)     4066 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/utils/asynchronously.py
+-rw-rw-rw-   0 root         (0) root         (0)     3765 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/data_watch/pipeline/utils/synchronously.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 19:43:24.582305 data-watch-sdk-0.0.1b1/data_watch_sdk.egg-info/
+-rw-r--r--   0 root         (0) root         (0)      992 2023-04-21 19:43:24.000000 data-watch-sdk-0.0.1b1/data_watch_sdk.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3118 2023-04-21 19:43:24.000000 data-watch-sdk-0.0.1b1/data_watch_sdk.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 19:43:24.000000 data-watch-sdk-0.0.1b1/data_watch_sdk.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      212 2023-04-21 19:43:24.000000 data-watch-sdk-0.0.1b1/data_watch_sdk.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       11 2023-04-21 19:43:24.000000 data-watch-sdk-0.0.1b1/data_watch_sdk.egg-info/top_level.txt
+-rw-r--r--   0 root         (0) root         (0)       38 2023-04-21 19:43:24.583305 data-watch-sdk-0.0.1b1/setup.cfg
+-rw-rw-rw-   0 root         (0) root         (0)     1348 2023-04-21 19:43:10.000000 data-watch-sdk-0.0.1b1/setup.py
```

### Comparing `data-watch-sdk-0.0.1b0/PKG-INFO` & `data-watch-sdk-0.0.1b1/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-watch-sdk
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: Data Watch Python SDK
 Home-page: https://alpha.dev
 Author: Algora Labs
 Author-email: hello@algoralabs.com
 License: UNKNOWN
 Description: # Data Watch
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/auth/__util.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/auth/__util.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/auth/asynchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/auth/asynchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/auth/synchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/auth/synchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/group/__util.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/group/__util.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from data_watch.api.model import SearchRequest
+from data_watch.api.model import SearchRequest, LookupRequest
 from data_watch.api.service.group.model import GroupRequest
 
 
 def _get_group_request_info(id: str) -> dict:
     return {"endpoint": f"config/datawatch/group/{id}"}
 
 
@@ -10,14 +10,18 @@
     return {"endpoint": f"config/datawatch/group", "params": {"name": name}}
 
 
 def _get_groups_request_info() -> dict:
     return {"endpoint": f"config/datawatch/group"}
 
 
+def _get_groups_by_lookup_request_info(request: LookupRequest) -> dict:
+    return {"endpoint": f"config/datawatch/group", "json": request.request_dict()}
+
+
 def _get_groups_by_rule_id_request_info(rule_id: str) -> dict:
     return {"endpoint": f"config/datawatch/group", "params": {"rule_id": rule_id}}
 
 
 def _search_groups_request_info(request: SearchRequest) -> dict:
     return {"endpoint": f"config/datawatch/group", "json": request.request_dict()}
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/group/asynchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/group/asynchronous.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Dict, Any, List
 
-from data_watch.api.model import SearchRequest
+from data_watch.api.model import SearchRequest, LookupRequest
 from data_watch.api.service.group.__util import (
     _get_group_request_info,
     _get_groups_request_info,
     _create_group_request_info,
     _update_group_request_info,
     _delete_group_request_info,
     _search_groups_request_info,
     _unique_group_name_request_info,
     _get_group_by_name_request_info,
     _get_groups_by_rule_id_request_info,
     _get_group_tags_request_info,
+    _get_groups_by_lookup_request_info,
 )
 from data_watch.api.service.group.model import GroupRequest
 from data_watch.common.decorators import async_data_request
 
 from data_watch.common.requests import (
     __async_get_request,
     __async_post_request,
@@ -56,45 +57,60 @@
 
 @async_data_request
 async def async_get_groups() -> List[Dict[str, Any]]:
     """
     Asynchronously get all groups.
 
     Returns:
-        List[Dict[str, Any]]: List of group response
+        List[Dict[str, Any]]: List of group responses
     """
     request_info = _get_groups_request_info()
     return await __async_get_request(**request_info)
 
 
 @async_data_request
+async def async_get_groups_by_lookup(request: LookupRequest) -> List[Dict[str, Any]]:
+    """
+    Asynchronously get all groups by lookup.
+
+    Args:
+        request (LookupRequest): The group information used in the group look up
+
+    Returns:
+        List[Dict[str, Any]]: List of group responses
+    """
+    request_info = _get_groups_by_lookup_request_info(request)
+    return await __async_post_request(**request_info)
+
+
+@async_data_request
 async def async_get_groups_by_rule_id(rule_id: str) -> List[Dict[str, Any]]:
     """
     Asynchronously get all groups by rule ID.
 
     Args:
         rule_id (str): Rule ID
 
     Returns:
-        List[Dict[str, Any]]: List of group response
+        List[Dict[str, Any]]: List of group responses
     """
     request_info = _get_groups_by_rule_id_request_info(rule_id)
     return await __async_get_request(**request_info)
 
 
 @async_data_request
 async def async_search_groups(request: SearchRequest) -> List[Dict[str, Any]]:
     """
     Asynchronously search all groups.
 
     Parameters:
         request (SearchRequest): A request carrying the search query
 
     Returns:
-        List[Dict[str, Any]]: List of group response
+        List[Dict[str, Any]]: List of group responses
     """
     request_info = _search_groups_request_info(request)
     return await __async_post_request(**request_info)
 
 
 @async_data_request
 async def async_create_group(request: GroupRequest) -> Dict[str, Any]:
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/group/synchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/group/synchronous.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,21 +1,22 @@
 from typing import Dict, Any, List
 
-from data_watch.api.model import SearchRequest
+from data_watch.api.model import SearchRequest, LookupRequest
 from data_watch.api.service.group.__util import (
     _get_group_request_info,
     _get_group_by_name_request_info,
     _get_groups_request_info,
     _get_groups_by_rule_id_request_info,
     _search_groups_request_info,
     _create_group_request_info,
     _update_group_request_info,
     _delete_group_request_info,
     _get_group_tags_request_info,
     _unique_group_name_request_info,
+    _get_groups_by_lookup_request_info,
 )
 from data_watch.api.service.group.model import GroupRequest
 from data_watch.common.decorators import data_request
 
 from data_watch.common.requests import (
     __get_request,
     __post_request,
@@ -56,45 +57,60 @@
 
 @data_request
 def get_groups() -> List[Dict[str, Any]]:
     """
     Get all groups.
 
     Returns:
-        List[Dict[str, Any]]: List of group response
+        List[Dict[str, Any]]: List of group responses
     """
     request_info = _get_groups_request_info()
     return __get_request(**request_info)
 
 
 @data_request
+def get_groups_by_lookup(request: LookupRequest) -> List[Dict[str, Any]]:
+    """
+    Get all groups by lookup.
+
+    Args:
+        request (LookupRequest): The group information used in the group look up
+
+    Returns:
+        List[Dict[str, Any]]: List of group responses
+    """
+    request_info = _get_groups_by_lookup_request_info(request)
+    return __post_request(**request_info)
+
+
+@data_request
 def get_groups_by_rule_id(rule_id: str) -> List[Dict[str, Any]]:
     """
     Get all groups by rule ID.
 
     Args:
         rule_id (str): Rule ID
 
     Returns:
-        List[Dict[str, Any]]: List of group response
+        List[Dict[str, Any]]: List of group responses
     """
     request_info = _get_groups_by_rule_id_request_info(rule_id)
     return __get_request(**request_info)
 
 
 @data_request
 def search_groups(request: SearchRequest) -> List[Dict[str, Any]]:
     """
     Search all groups.
 
     Parameters:
         request (SearchRequest): A request carrying the search query
 
     Returns:
-        List[Dict[str, Any]]: List of group response
+        List[Dict[str, Any]]: List of group responses
     """
     request_info = _search_groups_request_info(request)
     return __post_request(**request_info)
 
 
 @data_request
 def create_group(request: GroupRequest) -> Dict[str, Any]:
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/group/view/asynchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/group/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/group/view/synchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/group/view/synchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/job/__util.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/job/__util.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/job/asynchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/job/asynchronous.py`

 * *Files 2% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 
 
 @async_data_request
 async def async_update_job(id: str, request: JobRequest) -> Dict[str, Any]:
     """
     Asynchronously update job.
 
+    NOTE: Groups associated to the job are not updated
+
     Args:
         id (str): Job ID
         request (JobRequest): Job request
 
     Returns:
         Dict[str, Any]: Job response
     """
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/job/model.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/job/model.py`

 * *Files 17% similar despite different names*

```diff
@@ -5,27 +5,33 @@
 from data_watch.common.base import Base
 from data_watch.common.enum import Status
 
 
 class JobRequest(Base):
     name: str
     status: Status
-    group_id: str
+    group_ids: Optional[List[str]] = Field(default=None)
     start_time: Optional[int] = Field(default=None)
     end_time: Optional[int] = Field(default=None)
     metadata: Optional[dict] = Field(default=None)
     tags: Optional[List[str]] = Field(default=None)
 
 
 class JobResponse(Base):
     id: str
     name: str
     status: Status
-    group_id: str
     start_time: Optional[int]
     end_time: Optional[int]
     metadata: dict
     tags: List[str]
     created_by: str
     created_at: int
     updated_by: Optional[str]
     updated_at: Optional[int]
+
+
+class JobGroupResponse(Base):
+    group_id: str
+    rule_id: str
+    created_by: str
+    created_at: int
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/job/synchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/job/synchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -79,14 +79,16 @@
 
 
 @data_request
 def update_job(id: str, request: JobRequest) -> Dict[str, Any]:
     """
     Update job.
 
+    NOTE: Groups associated to the job are not updated
+
     Args:
         id (str): Job ID
         request (JobRequest): Job request
 
     Returns:
         Dict[str, Any]: Job response
     """
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/job/view/asynchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/job/view/asynchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/rule/__util.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/rule/__util.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,22 +1,26 @@
 import json
 from typing import List
 
-from data_watch.api.model import SearchRequest
+from data_watch.api.model import SearchRequest, LookupRequest
 from data_watch.api.service.rule.model import RuleRequest
 
 
 def _get_rule_request_info(id: str) -> dict:
     return {"endpoint": f"config/datawatch/rule/{id}"}
 
 
 def _get_rules_request_info() -> dict:
     return {"endpoint": f"config/datawatch/rule"}
 
 
+def _get_all_rules_by_groups_request_info(request: LookupRequest) -> dict:
+    return {"endpoint": f"config/datawatch/rule", "json": request.request_dict()}
+
+
 def _search_rules_request_info(request: SearchRequest) -> dict:
     return {"endpoint": f"config/datawatch/rule", "json": request.request_dict()}
 
 
 def _create_rule_request_info(request: RuleRequest) -> dict:
     return {"endpoint": f"config/datawatch/rule", "json": request.request_dict()}
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/rule/asynchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/rule/asynchronous.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Dict, Any, List
 
-from data_watch.api.model import SearchRequest
+from data_watch.api.model import SearchRequest, LookupRequest
 from data_watch.api.service.rule.__util import (
     _get_rule_request_info,
     _get_rules_request_info,
     _create_rule_request_info,
     _update_rule_request_info,
     _delete_rule_request_info,
     _search_rules_request_info,
     _get_rule_tags_request_info,
     _declarative_update_rule_groups_request_info,
+    _get_all_rules_by_groups_request_info,
 )
 from data_watch.api.service.rule.model import RuleRequest
 from data_watch.common.decorators import async_data_request
 
 from data_watch.common.requests import (
     __async_get_request,
     __async_post_request,
@@ -39,30 +40,45 @@
 
 @async_data_request
 async def async_get_rules() -> List[Dict[str, Any]]:
     """
     Asynchronously get all rules.
 
     Returns:
-        List[Dict[str, Any]]: List of rule response
+        List[Dict[str, Any]]: List of rule responses
     """
     request_info = _get_rules_request_info()
     return await __async_get_request(**request_info)
 
 
 @async_data_request
+async def async_get_rules_by_groups(request: LookupRequest) -> List[Dict[str, Any]]:
+    """
+    Asynchronously get all rules by groups.
+
+    Args:
+        request (LookupRequest): The group information used in the rule look up
+
+    Returns:
+        List[Dict[str, Any]]: List of rule responses
+    """
+    request_info = _get_all_rules_by_groups_request_info(request)
+    return await __async_post_request(**request_info)
+
+
+@async_data_request
 async def async_search_rules(request: SearchRequest) -> List[Dict[str, Any]]:
     """
     Asynchronously search all rules.
 
     Parameters:
         request (SearchRequest): A request carrying the search query
 
     Returns:
-        List[Dict[str, Any]]: List of rule response
+        List[Dict[str, Any]]: List of rule responses
     """
     request_info = _search_rules_request_info(request)
     return await __async_post_request(**request_info)
 
 
 @async_data_request
 async def async_create_rule(request: RuleRequest) -> Dict[str, Any]:
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/rule/model.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/rule/model.py`

 * *Files 27% similar despite different names*

```diff
@@ -26,14 +26,11 @@
     created_by: str
     created_at: int
     updated_by: Optional[str]
     updated_at: Optional[int]
 
 
 class RuleGroupResponse(Base):
-    id: str
     group_id: str
     rule_id: str
     created_by: str
     created_at: int
-    updated_by: Optional[str]
-    updated_at: Optional[int]
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/api/service/rule/synchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/api/service/rule/synchronous.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from typing import Dict, Any, List
 
-from data_watch.api.model import SearchRequest
+from data_watch.api.model import SearchRequest, LookupRequest
 from data_watch.api.service.rule.__util import (
     _get_rule_request_info,
     _get_rules_request_info,
     _create_rule_request_info,
     _update_rule_request_info,
     _delete_rule_request_info,
     _search_rules_request_info,
     _get_rule_tags_request_info,
     _declarative_update_rule_groups_request_info,
+    _get_all_rules_by_groups_request_info,
 )
 from data_watch.api.service.rule.model import RuleRequest
 from data_watch.common.decorators import data_request
 from data_watch.common.requests import (
     __get_request,
     __post_request,
     __put_request,
@@ -38,30 +39,45 @@
 
 @data_request
 def get_rules() -> List[Dict[str, Any]]:
     """
     Get all rules.
 
     Returns:
-        List[Dict[str, Any]]: List of rule response
+        List[Dict[str, Any]]: List of rule responses
     """
     request_info = _get_rules_request_info()
     return __get_request(**request_info)
 
 
 @data_request
+def get_rules_by_groups(request: LookupRequest) -> List[Dict[str, Any]]:
+    """
+    Get all rules by groups.
+
+    Args:
+        request (LookupRequest): The group information used in the rule look up
+
+    Returns:
+        List[Dict[str, Any]]: List of rule responses
+    """
+    request_info = _get_all_rules_by_groups_request_info(request)
+    return __post_request(**request_info)
+
+
+@data_request
 def search_rules(request: SearchRequest) -> List[Dict[str, Any]]:
     """
     Search all rules.
 
     Parameters:
         request (SearchRequest): A request carrying the search query
 
     Returns:
-        List[Dict[str, Any]]: List of rule response
+        List[Dict[str, Any]]: List of rule responses
     """
     request_info = _search_rules_request_info(request)
     return __post_request(**request_info)
 
 
 @data_request
 def create_rule(request: RuleRequest) -> Dict[str, Any]:
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/base.py` & `data-watch-sdk-0.0.1b1/data_watch/common/base.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/config.py` & `data-watch-sdk-0.0.1b1/data_watch/common/config.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/date/function.py` & `data-watch-sdk-0.0.1b1/data_watch/common/date/function.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/decorators/authorization/__util.py` & `data-watch-sdk-0.0.1b1/data_watch/common/decorators/authorization/__util.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/decorators/authorization/asynchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/common/decorators/authorization/asynchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/decorators/authorization/synchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/common/decorators/authorization/synchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/decorators/data/__util.py` & `data-watch-sdk-0.0.1b1/data_watch/common/decorators/data/__util.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/decorators/data/asynchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/common/decorators/data/asynchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/decorators/data/synchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/common/decorators/data/synchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/decorators/serializable/__util.py` & `data-watch-sdk-0.0.1b1/data_watch/common/decorators/serializable/__util.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/decorators/serializable/decorators.py` & `data-watch-sdk-0.0.1b1/data_watch/common/decorators/serializable/decorators.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/errors.py` & `data-watch-sdk-0.0.1b1/data_watch/common/errors.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/function.py` & `data-watch-sdk-0.0.1b1/data_watch/common/function.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/metaclass/singleton.py` & `data-watch-sdk-0.0.1b1/data_watch/common/metaclass/singleton.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/requests/asynchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/common/requests/asynchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/common/requests/synchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/common/requests/synchronous.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/pipeline/__init__.py` & `data-watch-sdk-0.0.1b1/data_watch/pipeline/__init__.py`

 * *Files 22% similar despite different names*

```diff
@@ -14,52 +14,52 @@
 logger = logging.getLogger(__name__)
 
 
 def data_quality_pipeline(
     data: Any,
     job_name: str,
     *,
-    group_name: Optional[str] = None,
-    group_id: Optional[str] = None,
+    group_names: Optional[List[str]] = None,
+    group_ids: Optional[List[str]] = None,
     metadata: Optional[dict] = None,
     tags: Optional[List[str]] = None,
     multi_processing: bool = False,
     processes: int = 5,
 ) -> JobResponse:
     """
     Runs data through a data quality pipeline.
 
-    NOTE: You must provide the group name or group id for this method to run.
+    NOTE: You must provide the group names and/or the group ids for this method to run.
     NOTE: The number of rules run in parallel is dependent on the number of processes.
 
     Args:
         data (Any): Data that is run through the pipeline
         job_name (str): Name assigned to the job created from running this pipeline
-        group_name (Optional[str]): The name of group run on the pipeline
-        group_id (Optional[str]): The id of the group run on the pipeline
+        group_names (Optional[List[str]]): List of group names to use with the pipeline
+        group_ids (Optional[List[str]]): List of group ids to use with the pipeline
         metadata (Optional[dict]): Metadata added to the job information
         tags (Optional[List[str]]): Tags added to the job
         multi_processing (bool): Optional flag to run the rules over the data concurrently
         processes (int): Optional number of process to spin up when running the rules concurrently
 
     Returns:
         JobResponse: The job response with all the information from the run
     """
-    job, group = start_job(
+    job, rules = start_job(
         job_name=job_name,
-        group_name=group_name,
-        group_id=group_id,
+        group_names=group_names,
+        group_ids=group_ids,
         metadata=metadata,
         tags=tags,
     )
 
     start_time = current_timestamp()
     logger.info(f"Starting data quality pipeline [{job_name=}, {start_time=}]")
     result = run_pipeline(
-        data, group, multi_processing=multi_processing, processes=processes
+        data, rules, multi_processing=multi_processing, processes=processes
     )
     end_time = current_timestamp()
     logger.debug(f"Data quality pipeline result: {result}")
     logger.info(
         f"Data quality pipeline finished [{job_name=}, {end_time=}]: {result.status}"
     )
 
@@ -74,44 +74,44 @@
     return job
 
 
 async def async_data_quality_pipeline(
     data: Any,
     job_name: str,
     *,
-    group_name: Optional[str] = None,
-    group_id: Optional[str] = None,
+    group_names: Optional[List[str]] = None,
+    group_ids: Optional[List[str]] = None,
     metadata: Optional[dict] = None,
     tags: Optional[List[str]] = None,
     multi_processing: bool = False,
     processes: int = 5,
 ) -> JobResponse:
     """
     Asynchronously runs data through a data quality pipeline.
 
-    NOTE: You must provide the group name or group id for this method to run.
+    NOTE: You must provide the group names and/or the group ids for this method to run.
     NOTE: The number of rules run in parallel is dependent on the number of processes.
 
     Args:
         data (Any): Data that is run through the pipeline
         job_name (str): Name assigned to the job created from running this pipeline
-        group_name (Optional[str]): The name of rule group run on the pipeline
-        group_id (Optional[str]): The id of the rule group run on the pipeline
+        group_names (Optional[List[str]]): List of group names to use with the pipeline
+        group_ids (Optional[List[str]]): List of group ids to use with the pipeline
         metadata (Optional[dict]): Metadata added to the job information
         tags (Optional[List[str]]): Tags added to the job
         multi_processing (bool): Optional flag to run the rules over the data concurrently
         processes (int): Optional number of process to spin up when running the rules concurrently
 
     Returns:
         JobResponse: The job response with all the information from the run
     """
     job, group = await async_start_job(
         job_name=job_name,
-        group_name=group_name,
-        group_id=group_id,
+        group_names=group_names,
+        group_ids=group_ids,
         metadata=metadata,
         tags=tags,
     )
 
     start_time = current_timestamp()
     logger.info(f"Starting data quality pipeline [{job_name=}, {start_time=}]")
     result = run_pipeline(
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/pipeline/execution/synchronously.py` & `data-watch-sdk-0.0.1b1/data_watch/pipeline/execution/synchronously.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,84 +1,82 @@
 import logging
-from typing import Any
+from typing import Any, List
 
 import pandas as pd
 
-from data_watch.api.service.group.view.model import GroupViewResponse
+from data_watch.api.service.rule.model import RuleResponse
 from data_watch.pipeline.model import DataQualityResult
 from data_watch.pipeline.pandas import (
     pipeline as pd_pipeline,
     mp_pipeline as pd_mp_pipeline,
 )
 
 
 logger = logging.getLogger(__name__)
 
 
 def run_pipeline(
     data: Any,
-    rule_group: GroupViewResponse,
+    rules: List[RuleResponse],
     *,
     multi_processing: bool = False,
     processes: int = 5,
 ) -> DataQualityResult:
     """
     Wrapper for the different pipeline types.
 
     Args:
         data (Any): The data being run through the pipeline
-        rule_group (GroupViewResponse): The rule group being run on the data
+        rules (List[RuleResponse]): The rules being run on the data
         multi_processing (bool): Optional flag to run the rules over the data concurrently
         processes (int): Optional number of process to spin up when running the rules concurrently
 
     Returns:
         DataQualityResult: The result of running the pipeline
     """
     if multi_processing:
         logger.debug(f"Running the multiprocessing pipeline with {processes} processes")
-        _multiprocessing_pipeline(data, rule_group, processes)
-    return _synchronous_pipeline(data, rule_group)
+        _multiprocessing_pipeline(data, rules, processes)
+    return _synchronous_pipeline(data, rules)
 
 
-def _synchronous_pipeline(
-    data: Any, rule_group: GroupViewResponse
-) -> DataQualityResult:
+def _synchronous_pipeline(data: Any, rules: List[RuleResponse]) -> DataQualityResult:
     """
     Runs all the rules sequentially over the data.
 
     Args:
         data (Any): The data being run through the pipeline
-        rule_group (GroupViewResponse): The rule group being run on the data
+        rules(List[RuleResponse]): The rules being run on the data
 
     Returns:
         DataQualityResult: The result of running the pipeline
     """
     if isinstance(data, pd.DataFrame):
-        result = pd_pipeline(data, rule_group)
+        result = pd_pipeline(data, rules)
     else:
         raise ValueError(f"Data type {type(data)} is not supported")
 
     return result
 
 
 def _multiprocessing_pipeline(
-    data: Any, rule_group: GroupViewResponse, processes: int
+    data: Any, rules: List[RuleResponse], processes: int
 ) -> DataQualityResult:
     """
     Runs all the rules over the data in parallel.
 
     NOTE: The number of rules run in parallel is dependent on the number of processes.
 
     Args:
         data (Any): The data being run through the pipeline
-        rule_group (GroupViewResponse): The rule group being run on the data
+        rules (List[RuleResponse]): The rules being run on the data
         processes (int): The number of process to spin up when running the rules concurrently
 
     Returns:
         DataQualityResult: The result of running the pipeline
     """
     if isinstance(data, pd.DataFrame):
-        result = pd_mp_pipeline(data, rule_group, processes)
+        result = pd_mp_pipeline(data, rules, processes)
     else:
         raise ValueError(f"Data type {type(data)} is not supported")
 
     return result
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/pipeline/model.py` & `data-watch-sdk-0.0.1b1/data_watch/pipeline/model.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/pipeline/pandas/__util.py` & `data-watch-sdk-0.0.1b1/data_watch/pipeline/pandas/__util.py`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/data_watch/pipeline/pandas/synchronous.py` & `data-watch-sdk-0.0.1b1/data_watch/pipeline/pandas/synchronous.py`

 * *Files 27% similar despite different names*

```diff
@@ -1,43 +1,45 @@
+from typing import List
+
 import pandas as pd
 
-from data_watch.api.service.group.view.model import GroupViewResponse
+from data_watch.api.service.rule.model import RuleResponse
 from data_watch.pipeline.model import DataQualityResult
 from data_watch.pipeline.pandas.__util import apply_rule
 from multiprocessing import Pool
 
 
-def pipeline(data: pd.DataFrame, group: GroupViewResponse) -> DataQualityResult:
+def pipeline(data: pd.DataFrame, rules: List[RuleResponse]) -> DataQualityResult:
     """
     Runs the all the pipeline rules on the provided dataset
 
     Args:
         data (pd.DataFrame): The data being put into the pipeline
-        group (GroupViewResponse): The group of rules applied to the data
+        rules (List[RuleResponse]): The rules applied to the data
 
     Returns:
         DataQualityResult: The result of the pipeline run
     """
-    results = [apply_rule(data, rule) for rule in group.rules]
+    results = [apply_rule(data, rule) for rule in rules]
     return DataQualityResult.from_rule_results(results)
 
 
 def mp_pipeline(
-    data: pd.DataFrame, group: GroupViewResponse, processes: int
+    data: pd.DataFrame, rules: List[RuleResponse], processes: int
 ) -> DataQualityResult:
     """
     Runs the all the pipeline rules on the provided dataset in parallel using multiprocessing.
 
     NOTE: The number of rules run in parallel is dependent on the number of processes.
 
     Args:
         data (pd.DataFrame): The data being put into the pipeline
-        group (GroupViewResponse): The group of rules applied to the data
+        rules (List[RuleResponse]): The rules applied to the data
         processes (int): The number of process to spin up when running the rules concurrently
 
     Returns:
         DataQualityResult: The result of the pipeline run
     """
     # Run pipeline
     with Pool(processes=processes) as pool:
-        results = pool.map(lambda rule: apply_rule(data, rule), group.rules)
+        results = pool.map(lambda rule: apply_rule(data, rule), rules)
     return DataQualityResult.from_rule_results(results)
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/pipeline/test.py` & `data-watch-sdk-0.0.1b1/data_watch/pipeline/test.py`

 * *Files 7% similar despite different names*

```diff
@@ -30,19 +30,19 @@
         rules (List[RuleRequest]): A list of the rules to run on the pipeline
         multi_processing (bool): Optional flag to run the rules over the data concurrently
         processes (int): Optional number of process to spin up when running the rules concurrently
 
     Returns:
         dict: A dict containing the metadata of the test job
     """
-    group = _generate_test_group(rules)
+    rules = [_rule_response_to_request(rule) for rule in rules]
     start_time = current_timestamp()
     logger.info(f"Starting data quality pipeline [{job_name=}, {start_time=}]")
     result = run_pipeline(
-        data, group, multi_processing=multi_processing, processes=processes
+        data, rules, multi_processing=multi_processing, processes=processes
     )
     end_time = current_timestamp()
     logger.debug(f"Data quality pipeline result: {result}")
     logger.info(
         f"Data quality pipeline finished [{job_name=}, {end_time=}]: {result.status}"
     )
 
@@ -50,28 +50,14 @@
         "job_name": job_name,
         "result": result,
         "start_time": start_time,
         "end_time": end_time,
     }
 
 
-def _generate_test_group(rules: List[RuleRequest]) -> GroupViewResponse:
-    return GroupViewResponse(
-        id="0",
-        name="test-group",
-        description=None,
-        tags=["TEST", "LOCAL"],
-        rules=[_rule_response_to_request(rule) for rule in rules],
-        created_by="local-user",
-        created_at=0,
-        updated_by=None,
-        updated_at=None,
-    )
-
-
 def _rule_response_to_request(rule: RuleRequest) -> RuleResponse:
     return RuleResponse(
         id="0",
         name=rule.name,
         description=rule.description,
         predicate=rule.predicate,
         threshold=rule.threshold,
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/pipeline/utils/asynchronously.py` & `data-watch-sdk-0.0.1b1/data_watch/pipeline/utils/synchronously.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,112 +1,110 @@
+import copy
 from typing import Optional, List, Tuple
 
-from data_watch.api.service.group.view.asynchronous import (
-    async_get_group_view_by_name,
-    async_get_group_view,
-)
-from data_watch.api.service.group.view.model import GroupViewResponse
-from data_watch.api.service.job import (
-    async_create_job,
-    async_update_job,
-)
+from data_watch.api.service.group.model import GroupResponse
+from data_watch.api.service.group.synchronous import get_groups_by_lookup
+from data_watch.api.service.job import create_job, update_job
 from data_watch.api.service.job.model import JobRequest, JobResponse
-from data_watch.common.date.function import current_timestamp
+from data_watch.api.service.rule.model import RuleResponse
+from data_watch.api.model import LookupRequest
+from data_watch.api.service.rule.synchronous import get_rules_by_groups
 from data_watch.common.enum import Status
 
 
-async def async_get_group(
-    group_name: Optional[str] = None, group_id: Optional[str] = None
-) -> GroupViewResponse:
+def get_rule_and_group_info(
+    group_names: Optional[List[str]] = None, group_ids: Optional[List[str]] = None
+) -> Tuple[List[GroupResponse], List[RuleResponse]]:
     """
-    Asynchronous helper method for getting the group of rules from the group_id or group_name.
-
-    NOTE: You must provide the group_name or group_id but not both.
+    Helper method for getting rules from the group_ids and group_names.
 
     Args:
-        group_name (Optional[str]): The name of rule group
-        group_id (Optional[str]): The id of the rule group
+        group_names (Optional[List[str]]): The name of rule groups
+        group_ids (Optional[List[str]]): The id of the rule groups
 
     Returns:
-        GroupViewResponse: The view of the group associated with the group_id/group_name
+        Tuple[List[GroupResponse], List[RuleResponse]]: A list of all the groups, and rules associated with the group
+        info passed in
     """
-    if not ((group_name is None) ^ (group_id is None)):
-        raise ValueError(f"You must supply group_id or group_name and only one of them")
-
-    if group_id is not None and group_name is None:
-        response = await async_get_group_view(group_id)
-    else:
-        response = await async_get_group_view_by_name(group_name)
-    return GroupViewResponse(**response)
+    request = LookupRequest(
+        group_names=group_names if group_names else [],
+        group_ids=group_ids if group_ids else [],
+    )
+    rule_response = get_rules_by_groups(request)
+    rules = [RuleResponse(**rule) for rule in rule_response]
+    group_response = get_groups_by_lookup(request)
+    groups = [GroupResponse(**group) for group in group_response]
+    return groups, rules
 
 
-async def async_start_job(
+def start_job(
     job_name: str,
     *,
-    group_name: Optional[str] = None,
-    group_id: Optional[str] = None,
+    group_names: Optional[List[str]] = None,
+    group_ids: Optional[List[str]] = None,
     metadata: Optional[dict] = None,
     tags: Optional[List[str]] = None,
-) -> Tuple[JobResponse, GroupViewResponse]:
+) -> Tuple[JobResponse, List[RuleResponse]]:
     """
-    Asynchronously creates the job with the starting information.
-
-    NOTE: You must provide the group_name or group_id but not both.
+    Creates the job with the starting information.
 
     Args:
         job_name (str): Name assigned to the job created from running this pipeline
-        group_name (Optional[str]): The name of rule group run on the pipeline
-        group_id (Optional[str]): The id of the rule group run on the pipeline
+        group_names (Optional[List[str]]): List of group names to use with the pipeline
+        group_ids (Optional[List[str]]): List of group ids to use with the pipeline
         metadata (Optional[dict]): Metadata added to the job information
         tags (Optional[List[str]]): Tags added to the job
 
     Returns:
-        Tuple[JobResponse, GroupViewResponse]: The created job and the group used in the job
+        Tuple[JobResponse, List[RuleResponse]]: The created job and the rules used in the job
     """
-    group = await async_get_group(group_name=group_name, group_id=group_id)
+    groups, rules = get_rule_and_group_info(
+        group_names=group_names, group_ids=group_ids
+    )
     request = JobRequest(
         name=job_name,
         status=Status.IN_PROGRESS,
-        group_id=group.id,
+        group_ids=[group.id for group in groups],
         metadata=metadata,
         tags=tags,
     )
-    response = await async_create_job(request)
+    response = create_job(request)
     job = JobResponse(**response)
-    return job, group
+    return job, rules
 
 
-async def async_stop_job(
+def stop_job(
     job: JobResponse,
     status: Status,
+    *,
     start_time: int,
     end_time: int,
-    *,
     metadata: Optional[dict] = None,
     tags: Optional[List[str]] = None,
 ) -> JobResponse:
     """
-    Asynchronously stops the job and updates it with all the results.
+    Stops the job and updates it with all the results.
 
     Args:
         job (JobResponse): The job being updated
         status (Status): The status of the job
         start_time (int): The timestamp from when the job started
         end_time (int): The timestamp from when the job ended
         metadata (Optional[dict]): Metadata added to the job information
         tags (Optional[List[str]]): Tags added to the job
 
     Returns:
         JobResponse: The updated job
     """
+    combined_metadata = copy.deepcopy(job.metadata)
+    combined_metadata.update(metadata)
     request = JobRequest(
         name=job.name,
         status=status,
-        group_id=job.group_id,
         start_time=start_time,
         end_time=end_time,
-        metadata=metadata or job.metadata,
+        metadata=combined_metadata,
         tags=tags or job.tags,
     )
-    response = await async_update_job(job.id, request)
+    response = update_job(job.id, request)
     job = JobResponse(**response)
     return job
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch/pipeline/utils/synchronously.py` & `data-watch-sdk-0.0.1b1/data_watch/pipeline/utils/asynchronously.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,111 +1,115 @@
-import copy
 from typing import Optional, List, Tuple
 
+from data_watch.api.service.group.asynchronous import async_get_groups_by_lookup
+from data_watch.api.service.group.model import GroupResponse
+from data_watch.api.service.group.view.asynchronous import (
+    async_get_group_view_by_name,
+    async_get_group_view,
+)
 from data_watch.api.service.group.view.model import GroupViewResponse
-from data_watch.api.service.group.view.synchronous import (
-    get_group_view_by_name,
-    get_group_view,
+from data_watch.api.service.job import (
+    async_create_job,
+    async_update_job,
 )
-from data_watch.api.service.job import create_job, update_job
 from data_watch.api.service.job.model import JobRequest, JobResponse
+from data_watch.api.service.rule.asynchronous import async_get_rules_by_groups
+from data_watch.api.service.rule.model import RuleResponse
+from data_watch.api.model import LookupRequest
+from data_watch.common.date.function import current_timestamp
 from data_watch.common.enum import Status
 
 
-def get_group(
-    group_name: Optional[str] = None, group_id: Optional[str] = None
-) -> GroupViewResponse:
+async def async_get_rule_and_group_info(
+    group_names: Optional[List[str]] = None, group_ids: Optional[List[str]] = None
+) -> Tuple[List[GroupResponse], List[RuleResponse]]:
     """
-    Helper method for getting the group of rules from the group_id or group_name.
-
-    NOTE: You must provide the group_name or group_id but not both.
+    Asynchronous helper method for getting the group of rules from the group_id or group_name.
 
     Args:
-        group_name (Optional[str]): The name of rule group
-        group_id (Optional[str]): The id of the rule group
+        group_names (Optional[List[str]]): The name of rule groups
+        group_ids (Optional[List[str]]): The id of the rule groups
 
     Returns:
-        GroupViewResponse: The view of the group associated with the group_id/group_name
+        Tuple[List[GroupResponse], List[RuleResponse]]: A list of all the groups, and rules associated with the group
+        info passed in
     """
-    if not ((group_name is None) ^ (group_id is None)):
-        raise ValueError(f"You must supply group_id or group_name and only one of them")
-
-    if group_id is not None and group_name is None:
-        response = get_group_view(group_id)
-    else:
-        response = get_group_view_by_name(group_name)
-    return GroupViewResponse(**response)
+    request = LookupRequest(group_names=group_names, group_ids=group_ids)
+    response = await async_get_rules_by_groups(request)
+    rules = [RuleResponse(**rule) for rule in response]
+    group_response = await async_get_groups_by_lookup(request)
+    groups = [GroupResponse(**group) for group in group_response]
+    return groups, rules
 
 
-def start_job(
+async def async_start_job(
     job_name: str,
     *,
-    group_name: Optional[str] = None,
-    group_id: Optional[str] = None,
+    group_names: Optional[List[str]] = None,
+    group_ids: Optional[List[str]] = None,
     metadata: Optional[dict] = None,
     tags: Optional[List[str]] = None,
-) -> Tuple[JobResponse, GroupViewResponse]:
+) -> Tuple[JobResponse, List[RuleResponse]]:
     """
-    Creates the job with the starting information.
+    Asynchronously creates the job with the starting information.
 
     NOTE: You must provide the group_name or group_id but not both.
 
     Args:
         job_name (str): Name assigned to the job created from running this pipeline
-        group_name (Optional[str]): The name of rule group run on the pipeline
-        group_id (Optional[str]): The id of the rule group run on the pipeline
+        group_names (Optional[List[str]]): The name of rule groups
+        group_ids (Optional[List[str]]): The id of the rule groups
         metadata (Optional[dict]): Metadata added to the job information
         tags (Optional[List[str]]): Tags added to the job
 
     Returns:
-        Tuple[JobResponse, GroupViewResponse]: The created job and the group used in the job
+        Tuple[JobResponse, List[RuleResponse]]: The created job and the rules used in the job
     """
-    group = get_group(group_name=group_name, group_id=group_id)
+    groups, rules = await async_get_rule_and_group_info(
+        group_names=group_names, group_ids=group_ids
+    )
     request = JobRequest(
         name=job_name,
         status=Status.IN_PROGRESS,
-        group_id=group.id,
+        group_ids=[group.id for group in groups],
         metadata=metadata,
         tags=tags,
     )
-    response = create_job(request)
+    response = await async_create_job(request)
     job = JobResponse(**response)
-    return job, group
+    return job, rules
 
 
-def stop_job(
+async def async_stop_job(
     job: JobResponse,
     status: Status,
-    *,
     start_time: int,
     end_time: int,
+    *,
     metadata: Optional[dict] = None,
     tags: Optional[List[str]] = None,
 ) -> JobResponse:
     """
-    Stops the job and updates it with all the results.
+    Asynchronously stops the job and updates it with all the results.
 
     Args:
         job (JobResponse): The job being updated
         status (Status): The status of the job
         start_time (int): The timestamp from when the job started
         end_time (int): The timestamp from when the job ended
         metadata (Optional[dict]): Metadata added to the job information
         tags (Optional[List[str]]): Tags added to the job
 
     Returns:
         JobResponse: The updated job
     """
-    combined_metadata = copy.deepcopy(job.metadata)
-    combined_metadata.update(metadata)
     request = JobRequest(
         name=job.name,
         status=status,
-        group_id=job.group_id,
         start_time=start_time,
         end_time=end_time,
-        metadata=combined_metadata,
+        metadata=metadata or job.metadata,
         tags=tags or job.tags,
     )
-    response = update_job(job.id, request)
+    response = await async_update_job(job.id, request)
     job = JobResponse(**response)
     return job
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch_sdk.egg-info/PKG-INFO` & `data-watch-sdk-0.0.1b1/data_watch_sdk.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: data-watch-sdk
-Version: 0.0.1b0
+Version: 0.0.1b1
 Summary: Data Watch Python SDK
 Home-page: https://alpha.dev
 Author: Algora Labs
 Author-email: hello@algoralabs.com
 License: UNKNOWN
 Description: # Data Watch
```

### Comparing `data-watch-sdk-0.0.1b0/data_watch_sdk.egg-info/SOURCES.txt` & `data-watch-sdk-0.0.1b1/data_watch_sdk.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `data-watch-sdk-0.0.1b0/setup.py` & `data-watch-sdk-0.0.1b1/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -14,15 +14,15 @@
     tag = subprocess.getoutput('git tag --sort=version:refname | tail -n1')
     commits = subprocess.getoutput(f'git rev-list {tag}..HEAD --count')
     return f'{tag}.{commits}'
 
 
 setuptools.setup(
     name="data-watch-sdk",
-    version="0.0.1b0",
+    version="0.0.1b1",
     author="Algora Labs",
     author_email="hello@algoralabs.com",
     description="Data Watch Python SDK",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://alpha.dev",
     classifiers=[
```

