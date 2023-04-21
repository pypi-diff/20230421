# Comparing `tmp/libertem-live-0.1.0.tar.gz` & `tmp/libertem-live-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "libertem-live-0.1.0.tar", last modified: Tue Jun 29 11:03:28 2021, max compression
+gzip compressed data, was "libertem-live-0.2.0.tar", last modified: Fri Apr 21 15:26:24 2023, max compression
```

## Comparing `libertem-live-0.1.0.tar` & `libertem-live-0.2.0.tar`

### file list

```diff
@@ -1,41 +1,170 @@
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.351547 libertem-live-0.1.0/
--rw-r--r--   0 vsts      (1001) docker     (121)    35149 2021-06-29 11:03:06.000000 libertem-live-0.1.0/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)       45 2021-06-29 11:03:06.000000 libertem-live-0.1.0/MANIFEST.in
--rw-r--r--   0 vsts      (1001) docker     (121)     4023 2021-06-29 11:03:28.351547 libertem-live-0.1.0/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     2352 2021-06-29 11:03:06.000000 libertem-live-0.1.0/README.rst
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.347546 libertem-live-0.1.0/libertem_live/
--rw-r--r--   0 vsts      (1001) docker     (121)       53 2021-06-29 11:03:28.347546 libertem-live-0.1.0/libertem_live/_baked_revision.py
--rw-r--r--   0 vsts      (1001) docker     (121)       82 2021-06-29 11:03:06.000000 libertem-live-0.1.0/pyproject.toml
--rw-r--r--   0 vsts      (1001) docker     (121)      501 2021-06-29 11:03:28.351547 libertem-live-0.1.0/setup.cfg
--rw-r--r--   0 vsts      (1001) docker     (121)     3955 2021-06-29 11:03:06.000000 libertem-live-0.1.0/setup.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.347546 libertem-live-0.1.0/src/
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.351547 libertem-live-0.1.0/src/libertem_live/
--rw-r--r--   0 vsts      (1001) docker     (121)      323 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)       22 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/__version__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3161 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/api.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.351547 libertem-live-0.1.0/src/libertem_live/detectors/
--rw-r--r--   0 vsts      (1001) docker     (121)     1151 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/LICENSE
--rw-r--r--   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/__init__.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.351547 libertem-live-0.1.0/src/libertem_live/detectors/base/
--rw-r--r--   0 vsts      (1001) docker     (121)      462 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/base/acquisition.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.351547 libertem-live-0.1.0/src/libertem_live/detectors/memory/
--rw-r--r--   0 vsts      (1001) docker     (121)       76 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/memory/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1609 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/memory/acquisition.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.351547 libertem-live-0.1.0/src/libertem_live/detectors/merlin/
--rw-r--r--   0 vsts      (1001) docker     (121)      189 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/merlin/__init__.py
--rw-r--r--   0 vsts      (1001) docker     (121)     8609 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/merlin/acquisition.py
--rw-r--r--   0 vsts      (1001) docker     (121)     3949 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/merlin/control.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24401 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/merlin/data.py
--rw-r--r--   0 vsts      (1001) docker     (121)    24760 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/merlin/sim.py
--rw-r--r--   0 vsts      (1001) docker     (121)     1342 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/detectors/merlin/tango_server.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.351547 libertem-live-0.1.0/src/libertem_live/udf/
--rw-r--r--   0 vsts      (1001) docker     (121)      933 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/udf/monitor.py
--rw-r--r--   0 vsts      (1001) docker     (121)      351 2021-06-29 11:03:06.000000 libertem-live-0.1.0/src/libertem_live/versioning.py
-drwxr-xr-x   0 vsts      (1001) docker     (121)        0 2021-06-29 11:03:28.351547 libertem-live-0.1.0/src/libertem_live.egg-info/
--rw-r--r--   0 vsts      (1001) docker     (121)     4023 2021-06-29 11:03:28.000000 libertem-live-0.1.0/src/libertem_live.egg-info/PKG-INFO
--rw-r--r--   0 vsts      (1001) docker     (121)     1005 2021-06-29 11:03:28.000000 libertem-live-0.1.0/src/libertem_live.egg-info/SOURCES.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-06-29 11:03:28.000000 libertem-live-0.1.0/src/libertem_live.egg-info/dependency_links.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       83 2021-06-29 11:03:28.000000 libertem-live-0.1.0/src/libertem_live.egg-info/entry_points.txt
--rw-r--r--   0 vsts      (1001) docker     (121)        1 2021-06-29 11:03:28.000000 libertem-live-0.1.0/src/libertem_live.egg-info/not-zip-safe
--rw-r--r--   0 vsts      (1001) docker     (121)       77 2021-06-29 11:03:28.000000 libertem-live-0.1.0/src/libertem_live.egg-info/requires.txt
--rw-r--r--   0 vsts      (1001) docker     (121)       14 2021-06-29 11:03:28.000000 libertem-live-0.1.0/src/libertem_live.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/
+-rw-r--r--   0 root         (0) root         (0)    35149 2023-04-19 12:20:22.000000 libertem-live-0.2.0/LICENSE
+-rw-r--r--   0 root         (0) root         (0)       45 2023-04-19 12:20:22.000000 libertem-live-0.2.0/MANIFEST.in
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-04-21 15:26:24.436473 libertem-live-0.2.0/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     3229 2023-04-20 17:12:41.000000 libertem-live-0.2.0/README.rst
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.424473 libertem-live-0.2.0/libertem_live/
+-rw-r--r--   0 root         (0) root         (0)       53 2023-04-21 15:26:24.424473 libertem-live-0.2.0/libertem_live/_baked_revision.py
+-rw-r--r--   0 root         (0) root         (0)       82 2023-04-19 12:20:23.000000 libertem-live-0.2.0/pyproject.toml
+-rw-r--r--   0 root         (0) root         (0)      512 2023-04-21 15:26:24.436473 libertem-live-0.2.0/setup.cfg
+-rw-r--r--   0 root         (0) root         (0)     4315 2023-04-21 14:43:24.000000 libertem-live-0.2.0/setup.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.424473 libertem-live-0.2.0/src/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      353 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      345 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      349 2023-04-19 17:02:51.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      167 2023-04-21 15:24:34.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__version__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      164 2023-04-20 16:50:56.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__version__.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      168 2023-04-20 16:28:19.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/__version__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     7632 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/api.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3882 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/hooks.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/hooks.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     3877 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/hooks.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/versioning.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      503 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/versioning.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      513 2023-04-19 17:02:51.000000 libertem-live-0.2.0/src/libertem_live/__pycache__/versioning.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)       22 2023-04-21 15:18:29.000000 libertem-live-0.2.0/src/libertem_live/__version__.py
+-rw-r--r--   0 root         (0) root         (0)     8951 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/api.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/
+-rw-r--r--   0 root         (0) root         (0)     1151 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/LICENSE
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      153 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      147 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      151 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     5348 2023-04-19 17:20:47.000000 libertem-live-0.2.0/src/libertem_live/detectors/__pycache__/common.cpython-39.pyc
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/
+-rw-r--r--   0 root         (0) root         (0)      291 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      386 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    12360 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/acquisition.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6767 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/connection.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     8174 2023-04-19 17:21:07.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/__pycache__/sim.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    13374 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/acquisition.py
+-rw-r--r--   0 root         (0) root         (0)     5781 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/connection.py
+-rw-r--r--   0 root         (0) root         (0)        0 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/controller.py
+-rw-r--r--   0 root         (0) root         (0)     7768 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/asi_tpx3/sim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/base/
+-rw-r--r--   0 root         (0) root         (0)      139 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      292 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      286 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      290 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     5149 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/acquisition.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4984 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/acquisition.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     5082 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/acquisition.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3257 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/connection.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3268 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/connection.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     3294 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/connection.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      679 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/controller.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      667 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/controller.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      679 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/controller.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     6591 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/acquisition.py
+-rw-r--r--   0 root         (0) root         (0)     2301 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/connection.py
+-rw-r--r--   0 root         (0) root         (0)      243 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/base/controller.py
+-rw-r--r--   0 root         (0) root         (0)     4930 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/common.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/dectris/
+-rw-r--r--   0 root         (0) root         (0)    23292 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/DEigerClient.py
+-rw-r--r--   0 root         (0) root         (0)      304 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)    22269 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/DEigerClient.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    22744 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/DEigerClient.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)    22557 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/DEigerClient.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      387 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      385 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    16048 2023-04-20 15:42:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/acquisition.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    15740 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/acquisition.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)    16015 2023-04-20 15:49:53.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/acquisition.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2021 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/common.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2001 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/common.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     2023 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/common.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    13970 2023-04-20 15:42:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/connection.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    13689 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/connection.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)    13793 2023-04-20 15:49:54.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/connection.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4467 2023-04-19 12:43:18.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/controller.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4306 2023-04-20 15:26:16.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/controller.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     4370 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/controller.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    17448 2023-04-21 14:48:39.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/__pycache__/sim.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    18419 2023-04-20 15:19:45.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/acquisition.py
+-rw-r--r--   0 root         (0) root         (0)     1312 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/common.py
+-rw-r--r--   0 root         (0) root         (0)    14526 2023-04-20 15:19:45.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/connection.py
+-rw-r--r--   0 root         (0) root         (0)     5324 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/controller.py
+-rw-r--r--   0 root         (0) root         (0)    27867 2023-04-20 17:16:36.000000 libertem-live-0.2.0/src/libertem_live/detectors/dectris/sim.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/memory/
+-rw-r--r--   0 root         (0) root         (0)      128 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/memory/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/memory/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      274 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/memory/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4043 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/memory/__pycache__/acquisition.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     3535 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/memory/acquisition.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.432473 libertem-live-0.2.0/src/libertem_live/detectors/merlin/
+-rw-r--r--   0 root         (0) root         (0)      323 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__init__.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)      442 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/__init__.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      442 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/__init__.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      440 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/__init__.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    12638 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/acquisition.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    12356 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/acquisition.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)    12567 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/acquisition.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     9836 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/connection.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     9678 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/connection.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     9747 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/connection.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4657 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/control.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     4610 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/control.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     4635 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/control.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)      681 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/controller.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)      669 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/controller.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)      681 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/controller.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    16680 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/data.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)    16629 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/data.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)    16727 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/data.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     4959 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     5698 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     5183 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    30373 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py310.1.nbc
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py310.nbi
+-rw-r--r--   0 root         (0) root         (0)    30480 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py37m.1.nbc
+-rw-r--r--   0 root         (0) root         (0)     1416 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py37m.nbi
+-rw-r--r--   0 root         (0) root         (0)    20187 2023-04-19 17:22:35.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py39.1.nbc
+-rw-r--r--   0 root         (0) root         (0)     1415 2023-04-19 17:22:35.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_multi_u2-15.py39.nbi
+-rw-r--r--   0 root         (0) root         (0)    26273 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py310.1.nbc
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-19 12:43:22.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py310.nbi
+-rw-r--r--   0 root         (0) root         (0)    26528 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py37m.1.nbc
+-rw-r--r--   0 root         (0) root         (0)     1366 2023-04-20 15:26:19.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py37m.nbi
+-rw-r--r--   0 root         (0) root         (0)    18829 2023-04-19 17:22:35.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py39.1.nbc
+-rw-r--r--   0 root         (0) root         (0)     1365 2023-04-19 17:22:35.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/decoders.decode_u2-4.py39.nbi
+-rw-r--r--   0 root         (0) root         (0)    23266 2023-04-19 17:22:20.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/__pycache__/sim.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)    14317 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/acquisition.py
+-rw-r--r--   0 root         (0) root         (0)     8647 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/connection.py
+-rw-r--r--   0 root         (0) root         (0)     4252 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/control.py
+-rw-r--r--   0 root         (0) root         (0)      258 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/controller.py
+-rw-r--r--   0 root         (0) root         (0)    20418 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/data.py
+-rw-r--r--   0 root         (0) root         (0)     8033 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/decoders.py
+-rw-r--r--   0 root         (0) root         (0)    29504 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/sim.py
+-rw-r--r--   0 root         (0) root         (0)     1342 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/tango_server.py
+-rw-r--r--   0 root         (0) root         (0)     3858 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/detectors/merlin/utils.py
+-rw-r--r--   0 root         (0) root         (0)     3657 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/hooks.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/src/libertem_live/udf/
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/
+-rw-r--r--   0 root         (0) root         (0)     3648 2023-04-19 12:43:04.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/monitor.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     3702 2023-04-20 15:26:09.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/monitor.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     3684 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/monitor.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2194 2023-04-19 12:43:04.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/record.cpython-310.pyc
+-rw-r--r--   0 root         (0) root         (0)     2164 2023-04-20 15:26:09.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/record.cpython-37.pyc
+-rw-r--r--   0 root         (0) root         (0)     2184 2023-04-19 17:02:52.000000 libertem-live-0.2.0/src/libertem_live/udf/__pycache__/record.cpython-39.pyc
+-rw-r--r--   0 root         (0) root         (0)     2848 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/udf/monitor.py
+-rw-r--r--   0 root         (0) root         (0)     1726 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/udf/record.py
+-rw-r--r--   0 root         (0) root         (0)      351 2023-04-19 12:20:23.000000 libertem-live-0.2.0/src/libertem_live/versioning.py
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.428473 libertem-live-0.2.0/src/libertem_live.egg-info/
+-rw-r--r--   0 root         (0) root         (0)     4494 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/PKG-INFO
+-rw-r--r--   0 root         (0) root         (0)     8600 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/SOURCES.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/dependency_links.txt
+-rw-r--r--   0 root         (0) root         (0)      222 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/entry_points.txt
+-rw-r--r--   0 root         (0) root         (0)        1 2023-04-19 12:22:49.000000 libertem-live-0.2.0/src/libertem_live.egg-info/not-zip-safe
+-rw-r--r--   0 root         (0) root         (0)      165 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/requires.txt
+-rw-r--r--   0 root         (0) root         (0)       14 2023-04-21 15:26:24.000000 libertem-live-0.2.0/src/libertem_live.egg-info/top_level.txt
+drwxr-xr-x   0 root         (0) root         (0)        0 2023-04-21 15:26:24.436473 libertem-live-0.2.0/tests/
+-rw-r--r--   0 root         (0) root         (0)     1512 2023-04-19 12:20:23.000000 libertem-live-0.2.0/tests/test_api.py
+-rw-r--r--   0 root         (0) root         (0)      343 2023-04-19 12:20:23.000000 libertem-live-0.2.0/tests/test_smoke.py
```

### Comparing `libertem-live-0.1.0/LICENSE` & `libertem-live-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem-live-0.1.0/PKG-INFO` & `libertem-live-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,119 @@
 Metadata-Version: 2.1
 Name: libertem-live
-Version: 0.1.0
+Version: 0.2.0
 Summary: Live processing with LiberTEM
 Home-page: https://libertem.github.io/LiberTEM-live
 Author: the LiberTEM team
 Author-email: libertem-dev@googlegroups.com
 License: GPL v3
-Description: |gitter|_ |azure|_ |github|_
-        
-        .. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
-        .. _gitter: https://gitter.im/LiberTEM/Lobby
-        
-        .. |azure| image:: https://dev.azure.com/LiberTEM/LiberTEM-live/_apis/build/status/LiberTEM.LiberTEM-live?branchName=master
-        .. _azure: https://dev.azure.com/LiberTEM/LiberTEM-live/_build/latest?definitionId=5&branchName=master
-        
-        .. |github| image:: https://img.shields.io/badge/GitHub-GPL--3.0-informational
-        .. _github: https://github.com/LiberTEM/LiberTEM-live/
-        
-        LiberTEM-live is an extension module for `LiberTEM
-        <https://libertem.github.io/LiberTEM/>`_ that allows live
-        data processing.
-        
-        .. note::
-          LiberTEM-live is still experimental and under active development, including
-          the overall architecture. New releases can include changes that break
-          backwards compatibility until the code and architecture are proven in
-          practical application and stabilized sufficiently.
-        
-          That being said, we encourage early experimental use, are happy to support
-          real-world application and appreciate feedback! You can contact us by
-          `creating or commenting on an Issue on GitHub
-          <https://github.com/LiberTEM/LiberTEM-live/issues>`_ or in the `LiberTEM
-          Gitter chat <https://gitter.im/LiberTEM/Lobby>`_.
-        
-        LiberTEM `user-defined functions (UDFs)
-        <https://libertem.github.io/LiberTEM/udf.html>`_ are designed to work without
-        modification on both offline data and live data streams. That means all
-        `LiberTEM applications <https://libertem.github.io/LiberTEM/applications.html>`_
-        and `LiberTEM-based modules
-        <https://libertem.github.io/LiberTEM/packages.html>`_ can work with all
-        supported detectors in LiberTEM-live.
-        
-        Installation
-        ------------
-        
-        The short version to install into an existing LiberTEM environment:
-        
-        .. code-block:: shell
-        
-            (libertem) $ python -m pip install "libertem-live"
-        
-        See the `LiberTEM installation instructions
-        <https://libertem.github.io/LiberTEM/install.html>`_ for more details on
-        installing LiberTEM.
-        
-        Detectors
-        ---------
-        
-        * `Quantum Detectors Merlin
-          <https://libertem.github.io/LiberTEM-live/reference.html#quantum-detectors-merlin>`_
-        
-        Support for the Gatan K2 IS is currently under development.
-        
-        License
-        -------
-        
-        LiberTEM-live is licensed under GPLv3. The I/O parts are also available under
-        the MIT license, please see LICENSE files in the subdirectories for details.
-        
 Keywords: electron microscopy
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: sim
 Provides-Extra: pymemfd
 Provides-Extra: pytango
+License-File: LICENSE
+
+|gitter|_ |azure|_ |github|_ |precommit|_ |zenodo|_
+
+.. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
+.. _gitter: https://gitter.im/LiberTEM/Lobby
+
+.. |azure| image:: https://dev.azure.com/LiberTEM/LiberTEM-live/_apis/build/status/LiberTEM.LiberTEM-live?branchName=master
+.. _azure: https://dev.azure.com/LiberTEM/LiberTEM-live/_build/latest?definitionId=5&branchName=master
+
+.. |github| image:: https://img.shields.io/badge/GitHub-GPL--3.0-informational
+.. _github: https://github.com/LiberTEM/LiberTEM-live/
+
+.. |precommit| image:: https://results.pre-commit.ci/badge/github/LiberTEM/LiberTEM-live/master.svg
+.. _precommit: https://results.pre-commit.ci/latest/github/LiberTEM/LiberTEM-live/master
+
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4916315.svg
+.. _zenodo: https://doi.org/10.5281/zenodo.4916315
+
+LiberTEM-live is an extension module for `LiberTEM
+<https://libertem.github.io/>`_ that allows live
+data processing.
+
+.. note::
+  LiberTEM-live is still experimental and under active development, including
+  the overall architecture. New releases can include changes that break
+  backwards compatibility until the code and architecture are proven in
+  practical application and stabilized sufficiently.
+
+  That being said, we encourage early experimental use, are happy to support
+  real-world application and appreciate feedback! You can contact us by
+  `creating or commenting on an Issue on GitHub
+  <https://github.com/LiberTEM/LiberTEM-live/issues>`_ or in the `LiberTEM
+  Gitter chat <https://gitter.im/LiberTEM/Lobby>`_.
+
+LiberTEM `user-defined functions (UDFs)
+<https://libertem.github.io/LiberTEM/udf.html>`_ are designed to work without
+modification on both offline data and live data streams. That means all
+`LiberTEM applications <https://libertem.github.io/LiberTEM/applications.html>`_
+and `LiberTEM-based modules
+<https://libertem.github.io/LiberTEM/packages.html>`_ can work with all
+supported detectors in LiberTEM-live.
+
+Installation
+------------
+
+The short version to install into an existing LiberTEM environment:
+
+.. code-block:: shell
+
+    (libertem) $ python -m pip install "libertem-live"
+
+See the `LiberTEM installation instructions
+<https://libertem.github.io/LiberTEM/install.html>`_ for more details on
+installing LiberTEM.
+
+Detectors
+---------
+
+* Quantum Detectors Merlin
+* DECTRIS EIGER2-based
+* Amsterdam Scientific Instruments CheeTah TPX3
+
+See `the documentation <https://libertem.github.io/LiberTEM-live/detectors.html>`_
+for details.
+
+Support for the Gatan K2 IS, ASI MPX3, and X-Spectrum cameras is currently
+under development.
+
+License
+-------
+
+LiberTEM-live is licensed under GPLv3. The I/O parts are also available under
+the MIT license, please see LICENSE files in the subdirectories for details.
+
+Acknowledgements
+----------------
+
+We are very grateful for your continuing support for LiberTEM-live!
+
+See `the acknowledgement page
+<https://libertem.github.io/acknowledgements.html#libertem-live>`_ for a list of
+authors and contributors to LiberTEM-live and other LiberTEM projects. See also
+our info on `funding <https://libertem.github.io/#funding>`_ and `industry
+partners <https://libertem.github.io/#industry-partners>`_.
+
+
```

### Comparing `libertem-live-0.1.0/README.rst` & `libertem-live-0.2.0/README.rst`

 * *Files 24% similar despite different names*

```diff
@@ -1,20 +1,26 @@
-|gitter|_ |azure|_ |github|_
+|gitter|_ |azure|_ |github|_ |precommit|_ |zenodo|_
 
 .. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
 .. _gitter: https://gitter.im/LiberTEM/Lobby
 
 .. |azure| image:: https://dev.azure.com/LiberTEM/LiberTEM-live/_apis/build/status/LiberTEM.LiberTEM-live?branchName=master
 .. _azure: https://dev.azure.com/LiberTEM/LiberTEM-live/_build/latest?definitionId=5&branchName=master
 
 .. |github| image:: https://img.shields.io/badge/GitHub-GPL--3.0-informational
 .. _github: https://github.com/LiberTEM/LiberTEM-live/
 
+.. |precommit| image:: https://results.pre-commit.ci/badge/github/LiberTEM/LiberTEM-live/master.svg
+.. _precommit: https://results.pre-commit.ci/latest/github/LiberTEM/LiberTEM-live/master
+
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4916315.svg
+.. _zenodo: https://doi.org/10.5281/zenodo.4916315
+
 LiberTEM-live is an extension module for `LiberTEM
-<https://libertem.github.io/LiberTEM/>`_ :cite:`Clausen2018` that allows live
+<https://libertem.github.io/>`_ :cite:`Clausen2018` that allows live
 data processing.
 
 .. note::
   LiberTEM-live is still experimental and under active development, including
   the overall architecture. New releases can include changes that break
   backwards compatibility until the code and architecture are proven in
   practical application and stabilized sufficiently.
@@ -45,17 +51,33 @@
 See the `LiberTEM installation instructions
 <https://libertem.github.io/LiberTEM/install.html>`_ for more details on
 installing LiberTEM.
 
 Detectors
 ---------
 
-* `Quantum Detectors Merlin
-  <https://libertem.github.io/LiberTEM-live/reference.html#quantum-detectors-merlin>`_
+* Quantum Detectors Merlin
+* DECTRIS EIGER2-based
+* Amsterdam Scientific Instruments CheeTah TPX3
+
+See `the documentation <https://libertem.github.io/LiberTEM-live/detectors.html>`_
+for details.
 
-Support for the Gatan K2 IS is currently under development.
+Support for the Gatan K2 IS, ASI MPX3, and X-Spectrum cameras is currently
+under development.
 
 License
 -------
 
 LiberTEM-live is licensed under GPLv3. The I/O parts are also available under
 the MIT license, please see LICENSE files in the subdirectories for details.
+
+Acknowledgements
+----------------
+
+We are very grateful for your continuing support for LiberTEM-live!
+
+See `the acknowledgement page
+<https://libertem.github.io/acknowledgements.html#libertem-live>`_ for a list of
+authors and contributors to LiberTEM-live and other LiberTEM projects. See also
+our info on `funding <https://libertem.github.io/#funding>`_ and `industry
+partners <https://libertem.github.io/#industry-partners>`_.
```

### Comparing `libertem-live-0.1.0/src/libertem_live/api.py` & `libertem-live-0.2.0/src/libertem_live/detectors/base/__pycache__/connection.cpython-310.pyc`

 * *Files 27% similar despite different names*

```diff
@@ -1,198 +1,204 @@
-00000000: 696d 706f 7274 2063 6f6e 7465 7874 6c69  import contextli
-00000010: 620a 0a66 726f 6d20 6c69 6265 7274 656d  b..from libertem
-00000020: 2e65 7865 6375 746f 722e 696e 6c69 6e65  .executor.inline
-00000030: 2069 6d70 6f72 7420 496e 6c69 6e65 4a6f   import InlineJo
-00000040: 6245 7865 6375 746f 720a 2320 4176 6f69  bExecutor.# Avoi
-00000050: 6420 6861 7669 6e67 2043 6f6e 7465 7874  d having Context
-00000060: 2069 6e20 7468 6973 206d 6f64 756c 6520   in this module 
-00000070: 746f 206d 616b 6520 7375 7265 0a23 2069  to make sure.# i
-00000080: 7420 6973 206e 6f74 2069 6d70 6f72 7465  t is not importe
-00000090: 6420 6279 2061 6363 6964 656e 7420 696e  d by accident in
-000000a0: 7374 6561 6420 6f66 204c 6976 6543 6f6e  stead of LiveCon
-000000b0: 7465 7874 0a66 726f 6d20 6c69 6265 7274  text.from libert
-000000c0: 656d 2e61 7069 2069 6d70 6f72 7420 436f  em.api import Co
-000000d0: 6e74 6578 7420 6173 204c 6962 6572 5445  ntext as LiberTE
-000000e0: 4d5f 436f 6e74 6578 740a 0a0a 636c 6173  M_Context...clas
-000000f0: 7320 4c69 7665 436f 6e74 6578 7428 4c69  s LiveContext(Li
-00000100: 6265 7254 454d 5f43 6f6e 7465 7874 293a  berTEM_Context):
-00000110: 0a20 2020 2027 2727 0a20 2020 2041 203a  .    '''.    A :
-00000120: 636c 6173 733a 604c 6976 6543 6f6e 7465  class:`LiveConte
-00000130: 7874 6020 6265 6861 7665 7320 6c69 6b65  xt` behaves like
-00000140: 2061 203a 636c 6173 733a 607e 6c69 6265   a :class:`~libe
-00000150: 7274 656d 2e61 7069 2e43 6f6e 7465 7874  rtem.api.Context
-00000160: 6020 696e 206d 6f73 740a 2020 2020 6369  ` in most.    ci
-00000170: 7263 756d 7374 616e 6365 732e 204e 6f74  rcumstances. Not
-00000180: 6162 6c65 2064 6966 6665 7265 6e63 6573  able differences
-00000190: 2061 7265 2074 6861 7420 6974 2063 7572   are that it cur
-000001a0: 7265 6e74 6c79 2073 7461 7274 7320 616e  rently starts an
-000001b0: 0a20 2020 203a 636c 6173 733a 607e 6c69  .    :class:`~li
-000001c0: 6265 7274 656d 2e65 7865 6375 746f 722e  bertem.executor.
-000001d0: 696e 6c69 6e65 2e49 6e6c 696e 654a 6f62  inline.InlineJob
-000001e0: 4578 6563 7574 6f72 6020 696e 7374 6561  Executor` instea
-000001f0: 6420 6f66 2061 0a20 2020 203a 636c 6173  d of a.    :clas
-00000200: 733a 607e 6c69 6265 7274 656d 2e65 7865  s:`~libertem.exe
-00000210: 6375 746f 722e 6461 736b 2e44 6173 6b4a  cutor.dask.DaskJ
-00000220: 6f62 4578 6563 7574 6f72 6020 6966 206e  obExecutor` if n
-00000230: 6f20 6578 6563 7574 6f72 2069 7320 7061  o executor is pa
-00000240: 7373 6564 2069 6e0a 2020 2020 7468 6520  ssed in.    the 
-00000250: 636f 6e73 7472 7563 746f 722c 2061 6e64  constructor, and
-00000260: 2074 6861 7420 6974 2063 616e 2070 7265   that it can pre
-00000270: 7061 7265 2061 6e64 2072 756e 2061 6371  pare and run acq
-00000280: 7569 7369 7469 6f6e 7320 6f6e 2074 6f70  uisitions on top
-00000290: 206f 660a 2020 2020 6c6f 6164 696e 6720   of.    loading 
-000002a0: 6f66 666c 696e 6520 6461 7461 7365 7473  offline datasets
-000002b0: 2e0a 0a20 2020 2054 6865 2064 6f63 7374  ...    The docst
-000002c0: 7269 6e67 7320 666f 7220 6d6f 7374 2066  rings for most f
-000002d0: 756e 6374 696f 6e73 2061 7265 2069 6e68  unctions are inh
-000002e0: 6572 6974 6564 2066 726f 6d20 7468 6520  erited from the 
-000002f0: 6261 7365 2063 6c61 7373 2e20 4d6f 7374  base class. Most
-00000300: 0a20 2020 206d 6574 686f 6473 2c20 696e  .    methods, in
-00000310: 2070 6172 7469 6375 6c61 7220 3a6d 6574   particular :met
-00000320: 683a 6072 756e 5f75 6466 6020 616e 6420  h:`run_udf` and 
-00000330: 3a6d 6574 683a 6072 756e 5f75 6466 5f69  :meth:`run_udf_i
-00000340: 7465 7260 2c20 6e6f 7720 6163 6365 7074  ter`, now accept
-00000350: 0a20 2020 2062 6f74 6820 616e 2061 6371  .    both an acq
-00000360: 7569 7369 7469 6f6e 206f 626a 6563 7420  uisition object 
-00000370: 616e 6420 6120 6461 7461 7365 7420 6173  and a dataset as
-00000380: 2074 6865 203a 636f 6465 3a60 6461 7461   the :code:`data
-00000390: 7365 7460 2070 6172 616d 6574 6572 2e0a  set` parameter..
-000003a0: 2020 2020 2727 270a 2020 2020 6465 6620      '''.    def 
-000003b0: 5f63 7265 6174 655f 6c6f 6361 6c5f 6578  _create_local_ex
-000003c0: 6563 7574 6f72 2873 656c 6629 3a0a 2020  ecutor(self):.  
-000003d0: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-000003e0: 2020 4c69 7665 2061 6371 7569 7369 7469    Live acquisiti
-000003f0: 6f6e 2063 7572 7265 6e74 6c79 2072 6571  on currently req
-00000400: 7569 7265 7320 6120 7375 6974 6162 6c65  uires a suitable
-00000410: 2065 7865 6375 746f 722c 2066 6f72 0a20   executor, for. 
-00000420: 2020 2020 2020 2065 7861 6d70 6c65 203a         example :
-00000430: 636c 6173 733a 607e 6c69 6265 7274 656d  class:`~libertem
-00000440: 2e65 7865 6375 746f 722e 696e 6c69 6e65  .executor.inline
-00000450: 2e49 6e6c 696e 654a 6f62 4578 6563 7574  .InlineJobExecut
-00000460: 6f72 602e 0a20 2020 2020 2020 2027 2727  or`..        '''
-00000470: 0a20 2020 2020 2020 2072 6574 7572 6e20  .        return 
-00000480: 496e 6c69 6e65 4a6f 6245 7865 6375 746f  InlineJobExecuto
-00000490: 7228 290a 0a20 2020 2040 636f 6e74 6578  r()..    @contex
-000004a0: 746c 6962 2e63 6f6e 7465 7874 6d61 6e61  tlib.contextmana
-000004b0: 6765 720a 2020 2020 6465 6620 5f64 6f5f  ger.    def _do_
-000004c0: 6163 7175 6973 6974 696f 6e28 7365 6c66  acquisition(self
-000004d0: 2c20 6163 7175 6973 6974 696f 6e2c 2075  , acquisition, u
-000004e0: 6466 293a 0a20 2020 2020 2020 2069 6620  df):.        if 
-000004f0: 6861 7361 7474 7228 6163 7175 6973 6974  hasattr(acquisit
-00000500: 696f 6e2c 2027 6163 7175 6972 6527 293a  ion, 'acquire'):
-00000510: 0a20 2020 2020 2020 2020 2020 2077 6974  .            wit
-00000520: 6820 6163 7175 6973 6974 696f 6e2e 6163  h acquisition.ac
-00000530: 7175 6972 6528 293a 0a20 2020 2020 2020  quire():.       
-00000540: 2020 2020 2020 2020 2079 6965 6c64 0a20           yield. 
-00000550: 2020 2020 2020 2065 6c73 653a 0a20 2020         else:.   
-00000560: 2020 2020 2020 2020 2079 6965 6c64 0a0a           yield..
-00000570: 2020 2020 6465 6620 7072 6570 6172 655f      def prepare_
-00000580: 6163 7175 6973 6974 696f 6e28 7365 6c66  acquisition(self
-00000590: 2c20 6465 7465 6374 6f72 5f74 7970 652c  , detector_type,
-000005a0: 202a 6172 6773 2c20 7472 6967 6765 723d   *args, trigger=
-000005b0: 4e6f 6e65 2c20 2a2a 6b77 6172 6773 293a  None, **kwargs):
-000005c0: 0a20 2020 2020 2020 2023 2046 4958 4d45  .        # FIXME
-000005d0: 2069 6d70 6c65 6d65 6e74 2073 696d 696c   implement simil
-000005e0: 6172 2074 6f20 4c69 6265 7254 454d 2064  ar to LiberTEM d
-000005f0: 6174 6173 6574 7320 6f6e 6365 0a20 2020  atasets once.   
-00000600: 2020 2020 2023 2077 6520 6861 7665 206d       # we have m
-00000610: 6f72 6520 6465 7465 6374 6f72 2074 7970  ore detector typ
-00000620: 6573 2074 6f20 7375 7070 6f72 740a 2020  es to support.  
-00000630: 2020 2020 2020 2727 270a 2020 2020 2020        '''.      
-00000640: 2020 4372 6561 7465 2061 6e20 6163 7175    Create an acqu
-00000650: 6973 6974 696f 6e20 6f62 6a65 6374 2e0a  isition object..
-00000660: 0a20 2020 2020 2020 2050 6172 616d 6574  .        Paramet
-00000670: 6572 730a 2020 2020 2020 2020 2d2d 2d2d  ers.        ----
-00000680: 2d2d 2d2d 2d2d 0a0a 2020 2020 2020 2020  ------..        
-00000690: 6465 7465 6374 6f72 5f74 7970 6520 3a20  detector_type : 
-000006a0: 7374 720a 2020 2020 2020 2020 2020 2020  str.            
-000006b0: 2d20 3a63 6f64 653a 6027 6d65 726c 696e  - :code:`'merlin
-000006c0: 2760 3a20 5175 616e 7475 6d20 4465 7465  '`: Quantum Dete
-000006d0: 6374 6f72 7320 4d65 726c 696e 2063 616d  ctors Merlin cam
-000006e0: 6572 612e 0a20 2020 2020 2020 2020 2020  era..           
-000006f0: 202d 203a 636f 6465 3a60 276d 656d 6f72   - :code:`'memor
-00000700: 7927 603a 204d 656d 6f72 792d 6261 7365  y'`: Memory-base
-00000710: 6420 6c69 7665 2064 6174 6120 7374 7265  d live data stre
-00000720: 616d 2e0a 2020 2020 2020 2020 7472 6967  am..        trig
-00000730: 6765 7220 3a20 6675 6e63 7469 6f6e 0a20  ger : function. 
-00000740: 2020 2020 2020 2020 2020 204b 6579 776f             Keywo
-00000750: 7264 2d6f 6e6c 7920 7061 7261 6d65 7465  rd-only paramete
-00000760: 722c 2063 616c 6c62 6163 6b20 6675 6e63  r, callback func
-00000770: 7469 6f6e 2074 6f20 7472 6967 6765 7220  tion to trigger 
-00000780: 616e 2061 6371 7569 7369 7469 6f6e 2e0a  an acquisition..
-00000790: 2020 2020 2020 2020 2020 2020 5365 6520              See 
-000007a0: 3a72 6566 3a60 7472 6967 6765 7260 2066  :ref:`trigger` f
-000007b0: 6f72 206d 6f72 6520 696e 666f 726d 6174  or more informat
-000007c0: 696f 6e2e 0a20 2020 2020 2020 202a 6172  ion..        *ar
-000007d0: 6773 2c20 2a2a 6b77 6172 6773 0a20 2020  gs, **kwargs.   
-000007e0: 2020 2020 2020 2020 2041 6464 6974 696f           Additio
-000007f0: 6e61 6c20 7061 7261 6d65 7465 7273 2066  nal parameters f
-00000800: 6f72 2074 6865 2061 6371 7569 7369 7469  or the acquisiti
-00000810: 6f6e 2e20 5365 6520 3a72 6566 3a60 6465  on. See :ref:`de
-00000820: 7465 6374 6f72 2072 6566 6572 656e 6365  tector reference
-00000830: 6020 666f 7220 6465 7461 696c 730a 2020  ` for details.  
-00000840: 2020 2020 2020 2020 2020 6f66 2069 6e64            of ind
-00000850: 6976 6964 7561 6c20 6163 7175 6973 6974  ividual acquisit
-00000860: 696f 6e20 7479 7065 7321 0a0a 2020 2020  ion types!..    
-00000870: 2020 2020 4578 616d 706c 6573 0a20 2020      Examples.   
-00000880: 2020 2020 202d 2d2d 2d2d 2d2d 2d0a 0a20       --------.. 
-00000890: 2020 2020 2020 2053 6565 203a 7265 663a         See :ref:
-000008a0: 6075 7361 6765 6020 696e 2074 6865 2064  `usage` in the d
-000008b0: 6f63 756d 656e 7461 7469 6f6e 210a 0a20  ocumentation!.. 
-000008c0: 2020 2020 2020 2027 2727 0a20 2020 2020         '''.     
-000008d0: 2020 2064 6574 6563 746f 725f 7479 7065     detector_type
-000008e0: 203d 2073 7472 2864 6574 6563 746f 725f   = str(detector_
-000008f0: 7479 7065 292e 6c6f 7765 7228 290a 2020  type).lower().  
-00000900: 2020 2020 2020 6966 2064 6574 6563 746f        if detecto
-00000910: 725f 7479 7065 203d 3d20 276d 6572 6c69  r_type == 'merli
-00000920: 6e27 3a0a 2020 2020 2020 2020 2020 2020  n':.            
-00000930: 6672 6f6d 206c 6962 6572 7465 6d5f 6c69  from libertem_li
-00000940: 7665 2e64 6574 6563 746f 7273 2e6d 6572  ve.detectors.mer
-00000950: 6c69 6e20 696d 706f 7274 204d 6572 6c69  lin import Merli
-00000960: 6e41 6371 7569 7369 7469 6f6e 0a20 2020  nAcquisition.   
-00000970: 2020 2020 2020 2020 2063 6c73 203d 204d           cls = M
-00000980: 6572 6c69 6e41 6371 7569 7369 7469 6f6e  erlinAcquisition
-00000990: 0a20 2020 2020 2020 2065 6c69 6620 6465  .        elif de
-000009a0: 7465 6374 6f72 5f74 7970 6520 3d3d 2027  tector_type == '
-000009b0: 6d65 6d6f 7279 273a 0a20 2020 2020 2020  memory':.       
-000009c0: 2020 2020 2066 726f 6d20 6c69 6265 7274       from libert
-000009d0: 656d 5f6c 6976 652e 6465 7465 6374 6f72  em_live.detector
-000009e0: 732e 6d65 6d6f 7279 2069 6d70 6f72 7420  s.memory import 
-000009f0: 4d65 6d6f 7279 4163 7175 6973 6974 696f  MemoryAcquisitio
-00000a00: 6e0a 2020 2020 2020 2020 2020 2020 636c  n.            cl
-00000a10: 7320 3d20 4d65 6d6f 7279 4163 7175 6973  s = MemoryAcquis
-00000a20: 6974 696f 6e0a 2020 2020 2020 2020 656c  ition.        el
-00000a30: 7365 3a0a 2020 2020 2020 2020 2020 2020  se:.            
-00000a40: 7261 6973 6520 5661 6c75 6545 7272 6f72  raise ValueError
-00000a50: 2866 2255 6e6b 6e6f 776e 2064 6574 6563  (f"Unknown detec
-00000a60: 746f 7220 7479 7065 2027 7b64 6574 6563  tor type '{detec
-00000a70: 746f 725f 7479 7065 7d27 2c20 7375 7070  tor_type}', supp
-00000a80: 6f72 7465 6420 6973 2027 6d65 726c 696e  orted is 'merlin
-00000a90: 2722 290a 2020 2020 2020 2020 7265 7475  '").        retu
-00000aa0: 726e 2063 6c73 282a 6172 6773 2c20 7472  rn cls(*args, tr
-00000ab0: 6967 6765 723d 7472 6967 6765 722c 202a  igger=trigger, *
-00000ac0: 2a6b 7761 7267 7329 2e69 6e69 7469 616c  *kwargs).initial
-00000ad0: 697a 6528 7365 6c66 2e65 7865 6375 746f  ize(self.executo
-00000ae0: 7229 0a0a 2020 2020 6465 6620 7275 6e5f  r)..    def run_
-00000af0: 7564 6628 7365 6c66 2c20 6461 7461 7365  udf(self, datase
-00000b00: 742c 2075 6466 2c20 2a61 7267 732c 202a  t, udf, *args, *
-00000b10: 2a6b 7761 7267 7329 3a0a 2020 2020 2020  *kwargs):.      
-00000b20: 2020 7769 7468 2073 656c 662e 5f64 6f5f    with self._do_
-00000b30: 6163 7175 6973 6974 696f 6e28 6461 7461  acquisition(data
-00000b40: 7365 742c 2075 6466 293a 0a20 2020 2020  set, udf):.     
-00000b50: 2020 2020 2020 2072 6574 7572 6e20 7375         return su
-00000b60: 7065 7228 292e 7275 6e5f 7564 6628 6461  per().run_udf(da
-00000b70: 7461 7365 743d 6461 7461 7365 742c 2075  taset=dataset, u
-00000b80: 6466 3d75 6466 2c20 2a61 7267 732c 202a  df=udf, *args, *
-00000b90: 2a6b 7761 7267 7329 0a0a 2020 2020 6465  *kwargs)..    de
-00000ba0: 6620 7275 6e5f 7564 665f 6974 6572 2873  f run_udf_iter(s
-00000bb0: 656c 662c 2064 6174 6173 6574 2c20 7564  elf, dataset, ud
-00000bc0: 662c 202a 6172 6773 2c20 2a2a 6b77 6172  f, *args, **kwar
-00000bd0: 6773 293a 0a20 2020 2020 2020 2077 6974  gs):.        wit
-00000be0: 6820 7365 6c66 2e5f 646f 5f61 6371 7569  h self._do_acqui
-00000bf0: 7369 7469 6f6e 2864 6174 6173 6574 2c20  sition(dataset, 
-00000c00: 7564 6629 3a0a 2020 2020 2020 2020 2020  udf):.          
-00000c10: 2020 7265 7475 726e 2073 7570 6572 2829    return super()
-00000c20: 2e72 756e 5f75 6466 5f69 7465 7228 6461  .run_udf_iter(da
-00000c30: 7461 7365 743d 6461 7461 7365 742c 2075  taset=dataset, u
-00000c40: 6466 3d75 6466 2c20 2a61 7267 732c 202a  df=udf, *args, *
-00000c50: 2a6b 7761 7267 7329 0a                   *kwargs).
+00000000: 6f0d 0d0a 0000 0000 87dc 3f64 fd08 0000  o.........?d....
+00000010: e300 0000 0000 0000 0000 0000 0000 0000  ................
+00000020: 0003 0000 0040 0000 0073 4000 0000 6400  .....@...s@...d.
+00000030: 6401 6c00 6d01 5a01 6d02 5a02 6d03 5a03  d.l.m.Z.m.Z.m.Z.
+00000040: 0100 6402 6403 6c04 6d05 5a05 0100 4700  ..d.d.l.m.Z...G.
+00000050: 6404 6405 8400 6405 8302 5a06 4700 6406  d.d...d...Z.G.d.
+00000060: 6407 8400 6407 8302 5a07 6408 5300 2909  d...d...Z.d.S.).
+00000070: e900 0000 0029 03da 084f 7074 696f 6e61  .....)...Optiona
+00000080: 6cda 0454 7970 65da 0554 7570 6c65 e901  l..Type..Tuple..
+00000090: 0000 0029 01da 1341 6371 7569 7369 7469  ...)...Acquisiti
+000000a0: 6f6e 5072 6f74 6f63 6f6c 6300 0000 0000  onProtocolc.....
+000000b0: 0000 0000 0000 0000 0000 0006 0000 0040  ...............@
+000000c0: 0000 0073 4000 0000 6500 5a01 6400 5a02  ...s@...e.Z.d.Z.
+000000d0: 6401 5a03 6504 6402 6505 6602 6403 6404  d.Z.e.d.e.f.d.d.
+000000e0: 8404 8301 5a06 6504 6402 6507 6508 6505  ....Z.e.d.e.e.e.
+000000f0: 6405 6602 1900 1900 6602 6406 6407 8404  d.f.....f.d.d...
+00000100: 8301 5a09 6408 5300 2909 da12 5065 6e64  ..Z.d.S.)...Pend
+00000110: 696e 6741 6371 7569 7369 7469 6f6e 6113  ingAcquisitiona.
+00000120: 0100 000a 2020 2020 4120 746f 6b65 6e20  ....    A token 
+00000130: 6f62 6a65 6374 2074 6861 7420 6361 6e20  object that can 
+00000140: 6265 206f 6274 6169 6e65 6420 6672 6f6d  be obtained from
+00000150: 0a20 2020 203a 6d65 7468 3a60 6c69 6265  .    :meth:`libe
+00000160: 7274 656d 5f6c 6976 652e 6465 7465 6374  rtem_live.detect
+00000170: 6f72 732e 6261 7365 2e63 6f6e 6e65 6374  ors.base.connect
+00000180: 696f 6e2e 4465 7465 6374 6f72 436f 6e6e  ion.DetectorConn
+00000190: 6563 7469 6f6e 2e77 6169 745f 666f 725f  ection.wait_for_
+000001a0: 6163 7175 6973 6974 696f 6e60 2e0a 0a20  acquisition`... 
+000001b0: 2020 2050 6173 7320 7468 6973 206f 626a     Pass this obj
+000001c0: 6563 7420 696e 746f 203a 6d65 7468 3a60  ect into :meth:`
+000001d0: 6c69 6265 7274 656d 5f6c 6976 652e 6170  libertem_live.ap
+000001e0: 692e 4c69 7665 436f 6e74 6578 742e 6d61  i.LiveContext.ma
+000001f0: 6b65 5f61 6371 7569 7369 7469 6f6e 600a  ke_acquisition`.
+00000200: 2020 2020 746f 2073 7461 7274 2070 726f      to start pro
+00000210: 6365 7373 696e 6720 7468 6520 696e 636f  cessing the inco
+00000220: 6d69 6e67 2064 6174 6120 7374 7265 616d  ming data stream
+00000230: 2e0a 2020 2020 da06 7265 7475 726e 6301  ..    ..returnc.
+00000240: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000250: 0000 0043 0000 00f3 0600 0000 7400 8300  ...C........t...
+00000260: 8201 2901 7a53 0a20 2020 2020 2020 2054  ..).zS.        T
+00000270: 6865 2074 6f74 616c 206e 756d 6265 7220  he total number 
+00000280: 6f66 2069 6d61 6765 7320 7468 6174 2061  of images that a
+00000290: 7265 2065 7870 6563 7465 6420 666f 7220  re expected for 
+000002a0: 7468 6973 2061 6371 7569 7369 7469 6f6e  this acquisition
+000002b0: 0a20 2020 2020 2020 20a9 01da 134e 6f74  .        ....Not
+000002c0: 496d 706c 656d 656e 7465 6445 7272 6f72  ImplementedError
+000002d0: a901 da04 7365 6c66 a900 720e 0000 00fa  ....self..r.....
+000002e0: 432f 617a 702f 6167 656e 742f 5f77 6f72  C/azp/agent/_wor
+000002f0: 6b2f 312f 732f 7372 632f 6c69 6265 7274  k/1/s/src/libert
+00000300: 656d 5f6c 6976 652f 6465 7465 6374 6f72  em_live/detector
+00000310: 732f 6261 7365 2f63 6f6e 6e65 6374 696f  s/base/connectio
+00000320: 6e2e 7079 da07 6e69 6d61 6765 730e 0000  n.py..nimages...
+00000330: 0073 0200 0000 0605 7a1a 5065 6e64 696e  .s......z.Pendin
+00000340: 6741 6371 7569 7369 7469 6f6e 2e6e 696d  gAcquisition.nim
+00000350: 6167 6573 2e63 0100 0000 0000 0000 0000  ages.c..........
+00000360: 0000 0100 0000 0100 0000 4300 0000 7304  ..........C...s.
+00000370: 0000 0064 0153 0029 027a 4a0a 2020 2020  ...d.S.).zJ.    
+00000380: 2020 2020 5468 6520 636f 6e63 7265 7465      The concrete
+00000390: 2060 6e61 765f 7368 6170 6560 2c20 6966   `nav_shape`, if
+000003a0: 2069 7420 6973 206b 6e6f 776e 2062 7920   it is known by 
+000003b0: 7468 6520 6465 7465 6374 6f72 0a20 2020  the detector.   
+000003c0: 2020 2020 204e 720e 0000 0072 0c00 0000       Nr....r....
+000003d0: 720e 0000 0072 0e00 0000 720f 0000 00da  r....r....r.....
+000003e0: 096e 6176 5f73 6861 7065 1500 0000 7302  .nav_shape....s.
+000003f0: 0000 0004 057a 1c50 656e 6469 6e67 4163  .....z.PendingAc
+00000400: 7175 6973 6974 696f 6e2e 6e61 765f 7368  quisition.nav_sh
+00000410: 6170 654e 290a da08 5f5f 6e61 6d65 5f5f  apeN)...__name__
+00000420: da0a 5f5f 6d6f 6475 6c65 5f5f da0c 5f5f  ..__module__..__
+00000430: 7175 616c 6e61 6d65 5f5f da07 5f5f 646f  qualname__..__do
+00000440: 635f 5fda 0870 726f 7065 7274 79da 0369  c__..property..i
+00000450: 6e74 7210 0000 0072 0200 0000 7204 0000  ntr....r....r...
+00000460: 0072 1100 0000 720e 0000 0072 0e00 0000  .r....r....r....
+00000470: 720e 0000 0072 0f00 0000 7207 0000 0006  r....r....r.....
+00000480: 0000 0073 0c00 0000 0800 0401 0207 1001  ...s............
+00000490: 0206 2001 7207 0000 0063 0000 0000 0000  .. .r....c......
+000004a0: 0000 0000 0000 0000 0000 0600 0000 4000  ..............@.
+000004b0: 0000 7356 0000 0065 005a 0164 005a 0264  ..sV...e.Z.d.Z.d
+000004c0: 015a 0364 0f64 0365 0465 0519 0064 0465  .Z.d.d.e.e...d.e
+000004d0: 0465 0619 0066 0464 0564 0684 055a 0764  .e...f.d.d...Z.d
+000004e0: 0764 0884 005a 0864 0964 0a84 005a 0964  .d...Z.d.d...Z.d
+000004f0: 0b64 0c84 005a 0a64 0465 0b65 0c19 0066  .d...Z.d.e.e...f
+00000500: 0264 0d64 0e84 045a 0d64 0253 0029 10da  .d.d...Z.d.S.)..
+00000510: 1244 6574 6563 746f 7243 6f6e 6e65 6374  .DetectorConnect
+00000520: 696f 6e7a 2e0a 2020 2020 4261 7365 2063  ionz..    Base c
+00000530: 6c61 7373 2066 6f72 2064 6574 6563 746f  lass for detecto
+00000540: 7220 636f 6e6e 6563 7469 6f6e 732e 0a20  r connections.. 
+00000550: 2020 204e da07 7469 6d65 6f75 7472 0800     N..timeoutr..
+00000560: 0000 6302 0000 0000 0000 0000 0000 0002  ..c.............
+00000570: 0000 0001 0000 0043 0000 0072 0900 0000  .......C...r....
+00000580: 2901 614d 0200 000a 2020 2020 2020 2020  ).aM....        
+00000590: 5761 6974 2066 6f72 2061 7420 6d6f 7374  Wait for at most
+000005a0: 2060 7469 6d65 6f75 7460 2073 6563 6f6e   `timeout` secon
+000005b0: 6473 2066 6f72 2061 6e20 6163 7175 6973  ds for an acquis
+000005c0: 6974 696f 6e20 746f 2073 7461 7274 2e20  ition to start. 
+000005d0: 5468 6973 0a20 2020 2020 2020 2064 6f65  This.        doe
+000005e0: 7320 6e6f 7420 7065 7266 6f72 6d20 616e  s not perform an
+000005f0: 7920 7472 6967 6765 7269 6e67 2069 7473  y triggering its
+00000600: 656c 6620 616e 6420 6578 7065 6374 7320  elf and expects 
+00000610: 736f 6d65 7468 696e 6720 6578 7465 726e  something extern
+00000620: 616c 0a20 2020 2020 2020 2074 6f20 6172  al.        to ar
+00000630: 6d20 616e 6420 7472 6967 6765 7220 7468  m and trigger th
+00000640: 6520 6163 7175 6973 6974 696f 6e2e 0a0a  e acquisition...
+00000650: 2020 2020 2020 2020 4f6e 6365 2074 6865          Once the
+00000660: 2064 6574 6563 746f 7220 6973 2061 726d   detector is arm
+00000670: 6564 2c20 7468 6973 2066 756e 6374 696f  ed, this functio
+00000680: 6e20 7265 7475 726e 7320 6120 6050 656e  n returns a `Pen
+00000690: 6469 6e67 4163 7175 6973 6974 696f 6e60  dingAcquisition`
+000006a0: 2c0a 2020 2020 2020 2020 7768 6963 6820  ,.        which 
+000006b0: 6361 6e20 6265 2063 6f6e 7665 7274 6564  can be converted
+000006c0: 2074 6f20 6120 6675 6c6c 2060 4163 7175   to a full `Acqu
+000006d0: 6973 6974 696f 6e60 206f 626a 6563 7420  isition` object 
+000006e0: 7573 696e 670a 2020 2020 2020 2020 3a6d  using.        :m
+000006f0: 6574 683a 606c 6962 6572 7465 6d5f 6c69  eth:`libertem_li
+00000700: 7665 2e61 7069 2e4c 6976 6543 6f6e 7465  ve.api.LiveConte
+00000710: 7874 2e6d 616b 655f 6163 7175 6973 6974  xt.make_acquisit
+00000720: 696f 6e60 2e0a 0a20 2020 2020 2020 2054  ion`...        T
+00000730: 6865 2066 756e 6374 696f 6e20 7265 7475  he function retu
+00000740: 726e 7320 604e 6f6e 6560 206f 6e20 7469  rns `None` on ti
+00000750: 6d65 6f75 742e 0a0a 2020 2020 2020 2020  meout...        
+00000760: 5061 7261 6d65 7465 7273 0a20 2020 2020  Parameters.     
+00000770: 2020 202d 2d2d 2d2d 2d2d 2d2d 2d0a 2020     ----------.  
+00000780: 2020 2020 2020 7469 6d65 6f75 740a 2020        timeout.  
+00000790: 2020 2020 2020 2020 2020 5469 6d65 6f75            Timeou
+000007a0: 7420 696e 2073 6563 6f6e 6473 2e20 4966  t in seconds. If
+000007b0: 2060 4e6f 6e65 602c 2077 6169 7420 696e   `None`, wait in
+000007c0: 6465 6669 6e69 7465 6c79 2e0a 2020 2020  definitely..    
+000007d0: 2020 2020 720a 0000 0029 0272 0d00 0000      r....).r....
+000007e0: 7219 0000 0072 0e00 0000 720e 0000 0072  r....r....r....r
+000007f0: 0f00 0000 da14 7761 6974 5f66 6f72 5f61  ......wait_for_a
+00000800: 6371 7569 7369 7469 6f6e 2100 0000 7302  cquisition!...s.
+00000810: 0000 0006 117a 2744 6574 6563 746f 7243  .....z'DetectorC
+00000820: 6f6e 6e65 6374 696f 6e2e 7761 6974 5f66  onnection.wait_f
+00000830: 6f72 5f61 6371 7569 7369 7469 6f6e 6301  or_acquisitionc.
+00000840: 0000 0000 0000 0000 0000 0001 0000 0001  ................
+00000850: 0000 0043 0000 0072 0900 0000 2901 6142  ...C...r....).aB
+00000860: 0100 000a 2020 2020 2020 2020 436c 6f73  ....        Clos
+00000870: 6520 7468 6520 636f 6e6e 6563 7469 6f6e  e the connection
+00000880: 2e20 4974 2773 2069 6d70 6f72 7461 6e74  . It's important
+00000890: 2074 6f20 6361 6c6c 2074 6869 7320 6675   to call this fu
+000008a0: 6e63 7469 6f6e 206f 6e63 650a 2020 2020  nction once.    
+000008b0: 2020 2020 796f 7520 646f 6e27 7420 6e65      you don't ne
+000008c0: 6564 2074 6865 2063 6f6e 6e65 6374 696f  ed the connectio
+000008d0: 6e20 616e 796d 6f72 652c 2061 7320 616e  n anymore, as an
+000008e0: 206f 7065 6e20 636f 6e6e 6563 7469 6f6e   open connection
+000008f0: 0a20 2020 2020 2020 206d 6967 6874 2069  .        might i
+00000900: 6e74 6572 6665 7265 2077 6974 6820 6f74  nterfere with ot
+00000910: 6865 7220 736f 6674 7761 7265 2075 7369  her software usi
+00000920: 6e67 2074 6865 2064 6574 6563 746f 722e  ng the detector.
+00000930: 0a0a 2020 2020 2020 2020 4966 2070 6f73  ..        If pos
+00000940: 7369 626c 652c 2075 7365 2074 6869 7320  sible, use this 
+00000950: 6f62 6a65 6374 2061 7320 6120 636f 6e74  object as a cont
+00000960: 6578 7420 6d61 6e61 6765 7220 696e 7374  ext manager inst
+00000970: 6561 642c 0a20 2020 2020 2020 2075 7369  ead,.        usi
+00000980: 6e67 2061 203a 636f 6465 3a60 7769 7468  ng a :code:`with
+00000990: 602d 7374 6174 656d 656e 742e 0a20 2020  `-statement..   
+000009a0: 2020 2020 2072 0a00 0000 720c 0000 0072       r....r....r
+000009b0: 0e00 0000 720e 0000 0072 0f00 0000 da05  ....r....r......
+000009c0: 636c 6f73 6534 0000 0073 0200 0000 0609  close4...s......
+000009d0: 7a18 4465 7465 6374 6f72 436f 6e6e 6563  z.DetectorConnec
+000009e0: 7469 6f6e 2e63 6c6f 7365 6301 0000 0000  tion.closec.....
+000009f0: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000a00: 0000 0073 0400 0000 7c00 5300 a901 4e72  ...s....|.S...Nr
+00000a10: 0e00 0000 720c 0000 0072 0e00 0000 720e  ....r....r....r.
+00000a20: 0000 0072 0f00 0000 da09 5f5f 656e 7465  ...r......__ente
+00000a30: 725f 5f3f 0000 0073 0200 0000 0401 7a1c  r__?...s......z.
+00000a40: 4465 7465 6374 6f72 436f 6e6e 6563 7469  DetectorConnecti
+00000a50: 6f6e 2e5f 5f65 6e74 6572 5f5f 6304 0000  on.__enter__c...
+00000a60: 0000 0000 0000 0000 0004 0000 0002 0000  ................
+00000a70: 0043 0000 0073 0c00 0000 7c00 a000 a100  .C...s....|.....
+00000a80: 0100 6400 5300 721c 0000 0029 0172 1b00  ..d.S.r....).r..
+00000a90: 0000 2904 720d 0000 00da 0865 7863 5f74  ..).r......exc_t
+00000aa0: 7970 65da 0965 7863 5f76 616c 7565 da09  ype..exc_value..
+00000ab0: 7472 6163 6562 6163 6b72 0e00 0000 720e  tracebackr....r.
+00000ac0: 0000 0072 0f00 0000 da08 5f5f 6578 6974  ...r......__exit
+00000ad0: 5f5f 4200 0000 7302 0000 000c 017a 1b44  __B...s......z.D
+00000ae0: 6574 6563 746f 7243 6f6e 6e65 6374 696f  etectorConnectio
+00000af0: 6e2e 5f5f 6578 6974 5f5f 6301 0000 0000  n.__exit__c.....
+00000b00: 0000 0000 0000 0001 0000 0001 0000 0043  ...............C
+00000b10: 0000 0072 0900 0000 2901 7a53 0a20 2020  ...r....).zS.   
+00000b20: 2020 2020 2052 6574 7572 6e73 2074 6865       Returns the
+00000b30: 206d 6174 6368 696e 6720 6041 6371 7569   matching `Acqui
+00000b40: 7369 7469 6f6e 6020 636c 6173 732e 0a0a  sition` class...
+00000b50: 2020 2020 2020 2020 3a6d 6574 6120 7072          :meta pr
+00000b60: 6976 6174 653a 0a20 2020 2020 2020 2072  ivate:.        r
+00000b70: 0a00 0000 720c 0000 0072 0e00 0000 720e  ....r....r....r.
+00000b80: 0000 0072 0f00 0000 da13 6765 745f 6163  ...r......get_ac
+00000b90: 7175 6973 6974 696f 6e5f 636c 7345 0000  quisition_clsE..
+00000ba0: 0073 0200 0000 0606 7a26 4465 7465 6374  .s......z&Detect
+00000bb0: 6f72 436f 6e6e 6563 7469 6f6e 2e67 6574  orConnection.get
+00000bc0: 5f61 6371 7569 7369 7469 6f6e 5f63 6c73  _acquisition_cls
+00000bd0: 721c 0000 0029 0e72 1200 0000 7213 0000  r....).r....r...
+00000be0: 0072 1400 0000 7215 0000 0072 0200 0000  .r....r....r....
+00000bf0: da05 666c 6f61 7472 0700 0000 721a 0000  ..floatr....r...
+00000c00: 0072 1b00 0000 721d 0000 0072 2100 0000  .r....r....r!...
+00000c10: 7203 0000 0072 0600 0000 7222 0000 0072  r....r....r"...r
+00000c20: 0e00 0000 720e 0000 0072 0e00 0000 720f  ....r....r....r.
+00000c30: 0000 0072 1800 0000 1d00 0000 730e 0000  ...r........s...
+00000c40: 0008 0004 011c 0308 1308 0b08 0316 0372  ...............r
+00000c50: 1800 0000 4e29 08da 0674 7970 696e 6772  ....N)...typingr
+00000c60: 0200 0000 7203 0000 0072 0400 0000 da0b  ....r....r......
+00000c70: 6163 7175 6973 6974 696f 6e72 0600 0000  acquisitionr....
+00000c80: 7207 0000 0072 1800 0000 720e 0000 0072  r....r....r....r
+00000c90: 0e00 0000 720e 0000 0072 0f00 0000 da08  ....r....r......
+00000ca0: 3c6d 6f64 756c 653e 0100 0000 7308 0000  <module>....s...
+00000cb0: 0014 000c 020e 0312 17                   .........
```

### Comparing `libertem-live-0.1.0/src/libertem_live/detectors/LICENSE` & `libertem-live-0.2.0/src/libertem_live/detectors/LICENSE`

 * *Files identical despite different names*

### Comparing `libertem-live-0.1.0/src/libertem_live/detectors/merlin/control.py` & `libertem-live-0.2.0/src/libertem_live/detectors/merlin/control.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 import socket
 import logging
+from typing import Optional
 
 logger = logging.getLogger(__name__)
 
 
 class MerlinControl:
     '''
     This class can be used to control a merlin medipix detector.
@@ -39,54 +40,60 @@
         self._socket.connect((self._host, self._port))
         self._socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._socket.settimeout(self._timeout)
 
     def __enter__(self):
         self._protected = True
         self.connect()
+        return self
 
     def __exit__(self, type, value, traceback):
         if self._protected:
             self.close()
             self._protected = False
 
     def _send(self, message):
+        assert self._socket is not None, "must be connected to send"
         self._socket.sendall(message.encode("ascii"))
         done = False
+        resp = None
         while not done:
             try:
                 resp = self._socket.recv(self._buffer_size)
                 done = True
             except socket.timeout:
                 pass
-        logger.debug('Response: {resp}'.format(resp=resp))
+        logger.debug(f'Response: {resp}')
         return resp
 
-    def _parse_response(self, resp):
+    def _parse_response(self, resp) -> Optional[bytes]:
         parts = resp.split(b',')
         msgs = ['Command OK', 'System Busy', 'Unrecognised Command',
                 'Param out of range']
 
         rc = int(parts[5]) if parts[2] == b'GET' else int(parts[4])
         if rc > 0:
             raise Exception(msgs[rc])
 
         if parts[2] == b'GET':
             return parts[4]
+        else:
+            # no response expected:
+            return None
 
     def _create_cmd(self, typ, cmd, value=None):
         string = ''
         if value is not None:
-            string = '{ty},{cmd},{val}'.format(ty=typ, cmd=cmd, val=value)
+            string = f'{typ},{cmd},{value}'
         else:
-            string = '{ty},{cmd},0'.format(ty=typ, cmd=cmd)
+            string = f'{typ},{cmd},0'
 
         msg = self._create_cmd_raw(string)
 
-        logger.debug('Command: {cmd}'.format(cmd=msg))
+        logger.debug(f'Command: {msg}')
         return msg
 
     def _create_cmd_raw(self, raw_cmd):
         msg = '{hdr},{len},{st}'.format(
             hdr=self._header,
             len=str(len(raw_cmd) + 1).zfill(self._num_digits),
             st=raw_cmd,
@@ -97,28 +104,30 @@
         """
         Send a SET command, and return the response
         """
         return self._parse_response(
             self._send(self._create_cmd('SET', param, value))
         )
 
-    def get(self, param):
+    def get(self, param) -> bytes:
         """
         Send a GET command, and return the response
         """
-        return self._parse_response(
+        parsed = self._parse_response(
             self._send(self._create_cmd('GET', param))
         )
+        assert parsed is not None, "for GET commands, the repsonse must not be None"
+        return parsed
 
     def send_command_file(self, filename):
         """
         Send the contents of :code:`filename`, which should
         contain complete merlin command lines.
         """
-        with open(filename, "r") as fh:
+        with open(filename) as fh:
             for line in fh:
                 line = line.strip()
                 if not line:
                     continue
                 self._parse_response(
                     self._send(self._create_cmd_raw(line))
                 )
@@ -130,9 +139,10 @@
         return self._parse_response(self._send(self._create_cmd('CMD', cmd)))
 
     def close(self):
         """
         Close the socket connection. Usually, instead of calling this function,
         you should use this class as a context manager.
         """
-        self._socket.close()
-        self._socket = None
+        if self._socket is not None:
+            self._socket.close()
+            self._socket = None
```

### Comparing `libertem-live-0.1.0/src/libertem_live/detectors/merlin/data.py` & `libertem-live-0.2.0/src/libertem_live/detectors/merlin/data.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,241 +1,329 @@
 import logging
 import socket
-import threading
-import contextlib
-import queue
 import time
+from typing import (
+    Generator, Optional, NamedTuple, Dict, Tuple,
+)
 
-import numba
 import numpy as np
 
-from libertem.io.dataset.base.decode import byteswap_2_decode
-
 from libertem_live.detectors.base.acquisition import AcquisitionTimeout
+from .decoders import (
+    decode_multi_u1,
+    decode_multi_u2,
+    decode_multi_r1,
+    decode_multi_r6,
+    decode_multi_r12,
+    decode_quad_r1,
+    decode_quad_r6,
+    decode_quad_r12,
+)
+
 
 logger = logging.getLogger(__name__)
 
 
-def get_np_dtype(dtype, bit_depth):
+class AcquisitionHeader(NamedTuple):
+    frames_in_acquisition: int
+    frames_per_trigger: int
+    raw_keys: Dict[str, str]
+
+    @classmethod
+    def from_raw(cls, header: bytes) -> "AcquisitionHeader":
+        result: Dict[str, str] = {}
+        for line in header.decode("latin1").split('\n'):
+            try:
+                if line.startswith("HDR") or line.startswith("End\t"):
+                    continue
+                k, v = line.split("\t", 1)
+                k = k.rstrip(':')
+                v = v.rstrip("\r")
+                v = v.rstrip("\n")
+            except ValueError:
+                logger.warn("error while parsing line %r", line)
+                raise
+            result[k] = v
+        return AcquisitionHeader(
+            raw_keys=result,
+            frames_in_acquisition=int(result['Frames in Acquisition (Number)']),
+            frames_per_trigger=int(result['Frames per Trigger (Number)']),
+        )
+
+
+def get_np_dtype(dtype, bit_depth) -> np.dtype:
     dtype = dtype.lower()
     num_bits = int(dtype[1:])
     if dtype[0] == "u":
         num_bytes = num_bits // 8
         return np.dtype(">u%d" % num_bytes)
     elif dtype[0] == "r":
         if bit_depth == 1:
             return np.dtype("uint64")
         elif bit_depth == 6:
             return np.dtype("uint8")
         elif bit_depth in (12, 24):
             # 24bit raw is two 12bit images after another:
             return np.dtype("uint16")
         else:
-            raise NotImplementedError("unknown bit depth: %s" % bit_depth)
-
-
-def _parse_frame_header(raw_data):
-    # FIXME: like in the MIB reader, but no 'filesize' and 'num_images'
-    # keys (they can be deduced from a .mib file, but don't make sense
-    # in the networked case)
-    header = raw_data.decode('ascii', errors='ignore')
-    parts = header.split(",")
-    header_size_bytes = int(parts[2])
-    parts = [p
-             for p in header[:header_size_bytes].split(",")
-             if '\x00' not in p]
-    dtype = parts[6].lower()
-    mib_kind = dtype[0]
-    image_size = (int(parts[5]), int(parts[4]))
-    # FIXME: There can either be threshold values for all chips, or maybe
-    # also none. For now, we just make use of the fact that the bit depth
-    # is supposed to be the last value.
-    bits_per_pixel_raw = int(parts[-1])
-    if mib_kind == "u":
-        bytes_per_pixel = int(parts[6][1:]) // 8
-        image_size_bytes = image_size[0] * image_size[1] * bytes_per_pixel
-    elif mib_kind == "r":
-        size_factor = {
-            1: 1/8,
-            6: 1,
-            12: 2,
-            24: 4,
-        }[bits_per_pixel_raw]
-        if bits_per_pixel_raw == 24:
-            image_size = (image_size[0], image_size[1] // 2)
-        image_size_bytes = int(image_size[0] * image_size[1] * size_factor)
+            raise NotImplementedError(f"unknown bit depth: {bit_depth}")
     else:
-        raise ValueError("unknown kind: %s" % mib_kind)
+        raise NotImplementedError(f"unknown dtype prefix: {dtype[0]}")
 
-    return {
-        'header_size_bytes': header_size_bytes,
-        'dtype': get_np_dtype(parts[6], bits_per_pixel_raw),
-        'mib_dtype': dtype,
-        'mib_kind': mib_kind,
-        'bits_per_pixel': bits_per_pixel_raw,
-        'image_size': image_size,
-        'image_size_bytes': image_size_bytes,
-        'sequence_first_image': int(parts[1]),
-    }
 
+class FrameHeader(NamedTuple):
+    header_size_bytes: int
+    dtype: np.dtype
+    mib_dtype: str   # rXX or uXX
+    mib_kind: str  # 'r' or 'u'
+    bits_per_pixel: int
+    image_size: Tuple[int, int]
+    image_size_eff: Tuple[int, int]
+    image_size_bytes: int
+    sequence_first_image: int
+    num_chips: int
+
+    @classmethod
+    def from_raw(cls, raw_data: bytes) -> "FrameHeader":
+        # FIXME: like in the MIB reader, but no 'filesize' and 'num_images'
+        # keys (they can be deduced from a .mib file, but don't make sense
+        # in the networked case)
+        header = raw_data.decode('ascii', errors='ignore')
+        parts = header.split(",")
+        header_size_bytes = int(parts[2])
+        parts = [p
+                for p in header[:header_size_bytes].split(",")
+                if '\x00' not in p]
+        dtype = parts[6].lower()
+        mib_kind = dtype[0]
+        image_size = (int(parts[5]), int(parts[4]))
+        # FIXME: There can either be threshold values for all chips, or maybe
+        # also none. For now, we just make use of the fact that the bit depth
+        # is supposed to be the last value.
+        bits_per_pixel_raw = int(parts[-1])
+        if mib_kind == "u":
+            bytes_per_pixel = int(parts[6][1:]) // 8
+            image_size_bytes = image_size[0] * image_size[1] * bytes_per_pixel
+        elif mib_kind == "r":
+            size_factor = {
+                1: 1/8,
+                6: 1,
+                12: 2,
+                24: 4,
+            }[bits_per_pixel_raw]
+            if bits_per_pixel_raw == 24:
+                image_size = (image_size[0], image_size[1] // 2)
+            image_size_bytes = int(image_size[0] * image_size[1] * size_factor)
+        else:
+            raise ValueError("unknown kind: %s" % mib_kind)
 
-@numba.njit(nogil=True, cache=True, parallel=True)
-def decode_multi_u2(input_bytes, out, header_size_bytes, num_frames):
-    """
-    Decode multiple >u2 frames
-    """
-    out = out.reshape((num_frames, -1))
-    frame_size_bytes = 256 * 256 * 2
-    for i in numba.prange(num_frames):
-        start_offset = header_size_bytes*(i+1)+i*frame_size_bytes
-        end_offset = start_offset + frame_size_bytes
-        in_for_frame = input_bytes[start_offset:end_offset]
-        byteswap_2_decode(in_for_frame, out[i])
+        num_chips = int(parts[3])
+        if num_chips == 4 and mib_kind == "r":
+            image_size_eff = (512, 512)
+            assert np.prod(image_size_eff) == np.prod(image_size)
+        else:
+            image_size_eff = image_size
 
+        return FrameHeader(
+            header_size_bytes=header_size_bytes,
+            dtype=get_np_dtype(parts[6], bits_per_pixel_raw),
+            mib_dtype=dtype,
+            mib_kind=mib_kind,
+            bits_per_pixel=bits_per_pixel_raw,
+            image_size=image_size,
+            image_size_eff=image_size_eff,
+            image_size_bytes=image_size_bytes,
+            sequence_first_image=int(parts[1]),
+            num_chips=num_chips,
+        )
 
-@numba.njit(nogil=True, cache=True, parallel=True)
-def decode_multi_u1(input_bytes, out, header_size_bytes, num_frames):
-    """
-    Decode multiple u1 frames
-    """
-    out = out.reshape((num_frames, -1))
-    frame_size_bytes = 256 * 256
-    for i in numba.prange(num_frames):
-        start_offset = header_size_bytes*(i+1)+i*frame_size_bytes
-        end_offset = start_offset + frame_size_bytes
-        in_for_frame = input_bytes[start_offset:end_offset]
-        out[i] = in_for_frame
-        # for j in range(end_offset - start_offset):
-        #     out[i, j] = in_for_frame[j]
 
+def validate_get_sig_shape(frame_hdr, sig_shape=None):
+    image_size = frame_hdr.image_size_eff
+    if image_size is None and sig_shape is None:
+        raise ValueError(
+                'Frame header "image_size" not present and sig shape '
+                'not given, cannot determine sig shape'
+            )
+    elif sig_shape is None:
+        return image_size
+    else:
+        if image_size != sig_shape:
+            raise ValueError(
+                f'Mismatch between sig_shape {sig_shape} setting and '
+                f'received "image_size" header {image_size}.'
+            )
+        return sig_shape
 
-@numba.jit(inline='always', cache=True)
-def decode_r1_swap(inp, out, idx):
-    """
-    RAW 1bit format: each bit is actually saved as a single bit. 64 bits
-    need to be unpacked together.
-    """
-    for stripe in range(inp.shape[0] // 8):
-        for byte in range(8):
-            inp_byte = inp[(stripe + 1) * 8 - (byte + 1)]
-            for bitpos in range(8):
-                out[idx, 64 * stripe + 8 * byte + bitpos] = (inp_byte >> bitpos) & 1
-
-
-@numba.jit(nogil=True, cache=True, parallel=True)
-def decode_multi_r1(input_bytes, out, header_size_bytes, num_frames):
-    out = out.reshape((num_frames, -1))
-    frame_size_bytes = 256 * 256 // 8
-    for i in numba.prange(num_frames):
-        start_offset = header_size_bytes*(i+1)+i*frame_size_bytes
-        end_offset = start_offset + frame_size_bytes
-        in_for_frame = input_bytes[start_offset:end_offset]
-        decode_r1_swap(in_for_frame, out, i)
 
+class MerlinRawFrames:
+    def __init__(
+        self,
+        buffer,
+        start_idx: int,
+        end_idx: int,
+        first_frame_header: FrameHeader,
+    ):
+        self._buffer = buffer
+        self._start_idx = start_idx
+        self._end_idx = end_idx
+        self._first_frame_header = first_frame_header
+
+    @property
+    def num_frames(self):
+        return self._end_idx - self._start_idx
+
+    @property
+    def start_idx(self):
+        return self._start_idx
+
+    @property
+    def end_idx(self):
+        return self._end_idx
+
+    @property
+    def first_frame_header(self):
+        return self._first_frame_header
+
+    @property
+    def buffer(self):
+        return self._buffer
 
-@numba.njit(inline='always', cache=True)
-def decode_r6_swap(inp, out, idx):
-    """
-    RAW 6bit format: the pixels need to be re-ordered in groups of 8. `inp`
-    should have dtype uint8.
-    """
-    for i in range(out.shape[1]):
-        col = i % 8
-        pos = i // 8
-        out_pos = (pos + 1) * 8 - col - 1
-        out[idx, out_pos] = inp[i]
-
-
-@numba.jit(nogil=True, cache=True, parallel=True)
-def decode_multi_r6(input_bytes, out, header_size_bytes, num_frames):
-    out = out.reshape((num_frames, -1))
-    frame_size_bytes = 256 * 256
-    for i in numba.prange(num_frames):
-        start_offset = header_size_bytes*(i+1)+i*frame_size_bytes
-        end_offset = start_offset + frame_size_bytes
-        in_for_frame = input_bytes[start_offset:end_offset]
-        decode_r6_swap(in_for_frame, out, i)
+    def decode(self, out_flat: np.ndarray):
+        fh = self._first_frame_header
+        header_size = int(fh.header_size_bytes) + 15
+        itemsize = fh.dtype.itemsize
+        bits_pp = fh.bits_per_pixel
+        num_rows = fh.image_size[0]
+        if fh.mib_kind == 'u':
+            # binary:
+            if itemsize == 1:
+                fn = decode_multi_u1
+            elif itemsize == 2:
+                fn = decode_multi_u2
+            else:
+                raise RuntimeError("itemsize %d currently not supported" % itemsize)
+        else:
+            # raw binary:
+            if fh.num_chips == 4:
+                if bits_pp == 1:
+                    fn = decode_quad_r1
+                elif bits_pp == 6:
+                    fn = decode_quad_r6
+                elif bits_pp == 12:
+                    fn = decode_quad_r12
+                else:
+                    raise RuntimeError(
+                        "can't handle quad raw binary %d bits per pixel yet" % bits_pp
+                    )
+            elif fh.num_chips == 1:
+                if bits_pp == 1:
+                    fn = decode_multi_r1
+                elif bits_pp == 6:
+                    fn = decode_multi_r6
+                elif bits_pp == 12:
+                    fn = decode_multi_r12
+                else:
+                    raise RuntimeError("can't handle raw binary %d bits per pixel yet" % bits_pp)
+            else:
+                raise RuntimeError(f"Can't handle num_chips={fh.num_chips}")
+        num_frames = self.num_frames
+        compat_shape = (num_frames, num_rows, -1)
+        input_arr = np.frombuffer(self._buffer, dtype=np.uint8).reshape(
+            (num_frames, -1)
+        )[:, header_size:].reshape(compat_shape)
+        out = out_flat[:num_frames].reshape(compat_shape)
+        fn(input_arr, out, header_size, num_frames)
+
+
+class MerlinDecodedFrames:
+    def __init__(
+        self,
+        buffer,
+        start_idx: int,
+        end_idx: int,
+        first_frame_header: FrameHeader,
+    ):
+        self._buffer = buffer
+        self._start_idx = start_idx
+        self._end_idx = end_idx
+        self._first_frame_header = first_frame_header
+
+    @property
+    def num_frames(self):
+        return self._end_idx - self._start_idx
+
+    @property
+    def start(self):
+        return self._start_idx
 
+    @property
+    def stop(self):
+        return self._end_idx
 
-@numba.njit(inline='always', cache=True)
-def decode_r12_swap(inp, out, idx):
-    """
-    RAW 12bit format: the pixels need to be re-ordered in groups of 4. `inp`
-    should be an uint8 view on big endian 12bit data (">u2")
-    """
-    for i in range(out.shape[1]):
-        col = i % 4
-        pos = i // 4
-        out_pos = (pos + 1) * 4 - col - 1
-        out[idx, out_pos] = (inp[i * 2] << 8) + (inp[i * 2 + 1] << 0)
-
-
-@numba.jit(nogil=True, cache=True, parallel=True)
-def decode_multi_r12(input_bytes, out, header_size_bytes, num_frames):
-    out = out.reshape((num_frames, -1))
-    frame_size_bytes = 2 * 256 * 256
-    for i in numba.prange(num_frames):
-        start_offset = header_size_bytes*(i+1)+i*frame_size_bytes
-        end_offset = start_offset + frame_size_bytes
-        in_for_frame = input_bytes[start_offset:end_offset]
-        decode_r12_swap(in_for_frame, out, i)
+    @property
+    def first_frame_header(self):
+        return self._first_frame_header
 
+    @property
+    def buf(self):
+        return self._buffer
 
-@numba.njit(inline='always', cache=True)
-def decode_r24_swap(inp, out, idx):
-    """
-    RAW 24bit format: a single 24bit consists of two frames that are encoded
-    like the RAW 12bit format, the first contains the most significant bits.
+    @classmethod
+    def from_raw(cls, raw_frames: MerlinRawFrames, out: np.ndarray) -> "MerlinDecodedFrames":
+        """
+        Decode `raw_frames` into `out` and return a `MerlinDecodedFrames`
+        object referencing `out`.
+        """
+        out_flat = out.reshape((out.shape[0], -1))
+        raw_frames.decode(
+            out_flat=out_flat
+        )
+        chunk = out[:raw_frames.num_frames]
+        return cls(
+            buffer=chunk,
+            start_idx=raw_frames.start_idx,
+            end_idx=raw_frames.end_idx,
+            first_frame_header=raw_frames.first_frame_header,
+        )
 
-    So after a frame header, there are (512, 256) >u2 values, which then
-    need to be shuffled like in `decode_r12_swap`.
 
-    This decoder function only works together with mib_r24_get_read_ranges
-    which generates twice as many read ranges than normally.
+class MerlinRawSocket:
     """
-    for i in range(out.shape[1]):
-        col = i % 4
-        pos = i // 4
-        out_pos = (pos + 1) * 4 - col - 1
-        out_val = np.uint32((inp[i * 2] << 8) + (inp[i * 2 + 1] << 0))
-        if idx % 2 == 0:  # from first frame: most significant bits
-            out_val = out_val << 12
-        out[idx // 2, out_pos] += out_val
-
-
-class MerlinDataSocket:
-    def __init__(self, host='127.0.0.1', port=6342, timeout=1.0):
+    Read packets of frames from the merlin data socket and
+    pass them on in undecoded form
+    """
+    def __init__(self, host: str = '127.0.0.1', port: int = 6342, timeout: float = 1.0):
         self._host = host
         self._port = port
         self._timeout = timeout
         self._socket = None
-        self._acquisition_header = None
         self._is_connected = False
-        self._read_lock = threading.Lock()
         self._frame_counter = 0
 
     def connect(self):
         self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         self._socket.connect((self._host, self._port))
         self._socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         self._socket.settimeout(self._timeout)
         self._is_connected = True
-        self._frame_counter = 0
+        return self
 
     def is_connected(self):
         return self._is_connected
 
     def read_unbuffered(self, length, cancel_timeout=None):
         """
         read exactly length bytes from the socket
 
         note: efficiency to be evaluated
         """
         if not self.is_connected():
             raise RuntimeError("can't read without connection")
+        assert self._socket is not None
         total_bytes_read = 0
         buf = bytearray(16*1024*1024)
         assert length < len(buf)
         view = memoryview(buf)
         start_time = time.time()
         while total_bytes_read < length:
             try:
@@ -254,14 +342,15 @@
 
     def read_into(self, out):
         """
         read exactly len(out) bytes from the socket
         """
         if not self.is_connected():
             raise RuntimeError("can't read without connection")
+        assert self._socket is not None
         length = len(out)
         total_bytes_read = 0
         view = memoryview(out)
         while total_bytes_read < length:
             try:
                 bytes_read = self._socket.recv_into(
                     view[total_bytes_read:],
@@ -281,124 +370,28 @@
         assert hdr.startswith(b'MPX,'), "Should start with MPX, first bytes are %r" % hdr[:16]
         parts = hdr.split(b',')
         length = int(parts[1])
         # we already consumed the comma, which seems to be part of the
         # length calculation, that's why we substract 1 here:
         return length - 1
 
-    def _read_acquisition_header(self, cancel_timeout=None):
+    def read_acquisition_header(self, cancel_timeout: Optional[float] = None) -> AcquisitionHeader:
         # assumption: when we connect, the connection is idle
         # so the first thing we will get is the acquisition header.
         # we read it in an inefficient way, but the header is small,
         # so this should be ok:
         length = self.read_mpx_length(cancel_timeout=cancel_timeout)
         header = self.read_unbuffered(length)
-        header = self._parse_acq_header(header)
+        header = AcquisitionHeader.from_raw(header)
         self._acquisition_header = header
         return header
 
-    def get_acquisition_header(self):
-        return self._acquisition_header
-
-    def read_headers(self, cancel_timeout=None):
-        """
-        Read acquisition header, and peek first frame header
-
-        The acquisition header is consumed, the first frame header will
-        be kept in the socket queue, and can be read regularly afterwards.
-        """
-        self._acquisition_header = self._read_acquisition_header(cancel_timeout=cancel_timeout)
-        self._first_frame_header = self._peek_frame_header()
-        self._frame_counter = self._first_frame_header['sequence_first_image'] - 1
-        logger.info(f"got headers; frame offset = {self._frame_counter}")
-        return self._acquisition_header, self._first_frame_header
-
-    def get_input_buffer(self, num_frames):
-        header_size = int(self._first_frame_header['header_size_bytes']) + 15
-        image_size = int(self._first_frame_header['image_size_bytes'])
-        read_size = num_frames*(header_size + image_size)
-        input_bytes = bytearray(read_size)
-        return input_bytes
-
-    def get_out_buffer(self, num_frames, dtype=np.float32):
-        return np.zeros((num_frames, 256, 256), dtype=dtype)
-
-    def read_multi_frames(self, out, input_buffer, num_frames=32, read_upto_frame=None, timeout=-1):
-        """
-        Returns `False` on timeout, `True` in case we are done and don't need to
-        read any more frames (according to `read_upto_frame`), or a tuple
-        `(buffer, frame_idx_start, frame_idx_end)`
-
-        On EOF or timeout, can read less than `num_frames`. In that case, `buffer` is sliced
-        to only contain decoded data. `out` will not be fully overwritten in this case
-        and can contain garbage at the end.
-
-        `read_upto_frame` can be used to only read up to a total number of frames.
-        Once this number is reached, we behave the same way as if we had reached EOF.
-        """
-        out_flat = out.reshape((num_frames, -1))
-        header_size = int(self._first_frame_header['header_size_bytes']) + 15
-        bytes_per_frame = header_size + self._first_frame_header['image_size_bytes']
-
-        lock_success = self._read_lock.acquire(timeout=timeout)
-        if not lock_success:
-            return False
-        try:
-            input_buffer = memoryview(input_buffer)
-            if read_upto_frame is not None:
-                num_frames = min(num_frames, read_upto_frame - self._frame_counter)
-                input_buffer = input_buffer[:num_frames * bytes_per_frame]
-                if num_frames == 0:
-                    return True  # we are done.
-            bytes_read = self.read_into(input_buffer)
-            frames_read = bytes_read // bytes_per_frame
-            if bytes_read % bytes_per_frame != 0:
-                raise EOFError(
-                    "input data stream truncated (%d,%d)" % (
-                        bytes_read, bytes_per_frame
-                    )
-                )
-            self._frame_counter += frames_read
-            # save frame_counter while we hold the lock:
-            frame_counter = self._frame_counter
-            if bytes_read == 0:
-                # timeout or EOF without any data read:
-                return False
-        finally:
-            self._read_lock.release()
-        self.decode(input_buffer[:bytes_read], out_flat[:frames_read], header_size, frames_read)
-        return (out[:frames_read], frame_counter - frames_read, frame_counter)
-
-    def decode(self, input_buffer, out_flat, header_size, num_frames):
-        fh = self._first_frame_header
-        itemsize = fh['dtype'].itemsize
-        bits_pp = fh['bits_per_pixel']
-        if fh['mib_kind'] == 'u':
-            # binary:
-            if itemsize == 1:
-                fn = decode_multi_u1
-            elif itemsize == 2:
-                fn = decode_multi_u2
-            else:
-                raise Exception("itemsize %d currently not supported" % itemsize)
-        else:
-            # raw binary:
-            if bits_pp == 1:
-                fn = decode_multi_r1
-            elif bits_pp == 6:
-                fn = decode_multi_r6
-            elif bits_pp == 12:
-                fn = decode_multi_r12
-            else:
-                raise Exception("can't handle %d bits per pixel yet" % bits_pp)
-        input_arr = np.frombuffer(input_buffer, dtype=np.uint8)
-        fn(input_arr, out_flat[:num_frames], header_size, num_frames)
-
-    def _peek_frame_header(self):
+    def peek_frame_header(self) -> FrameHeader:
         # first, peek only the MPX header part:
+        assert self._socket is not None
         while True:
             try:
                 buf = self._socket.recv(15, socket.MSG_PEEK)
                 assert len(buf) == 15
                 break
             except socket.timeout:
                 pass
@@ -408,268 +401,216 @@
 
         # now, peek enough to read the frame header:
         buf = b''
         peek_length = min(15 + length, 4096)
         while len(buf) < peek_length:
             # need to repeat, as the first peek can fail to give the full length message:
             buf = self._socket.recv(peek_length, socket.MSG_PEEK)
-        frame_header = _parse_frame_header(buf[15:])
+        frame_header = FrameHeader.from_raw(buf[15:])
         return frame_header
 
-    def _parse_acq_header(self, header):
-        result = {}
-        for line in header.decode("latin1").split('\n'):
-            try:
-                if line.startswith("HDR") or line.startswith("End\t"):
-                    continue
-                k, v = line.split("\t", 1)
-                k = k.rstrip(':')
-                v = v.rstrip("\r")
-                v = v.rstrip("\n")
-            except ValueError:
-                logger.warn("error while parsing line %r", line)
-                raise
-            result[k] = v
-        return result
-
     def close(self):
-        self._socket.close()
-        self._is_connected = False
+        if self._is_connected:
+            assert self._socket is not None
+            self._socket.close()
+            self._socket = None
+            self._is_connected = False
 
     def __enter__(self):
         self.connect()
 
     def __exit__(self, type, value, traceback):
         self.close()
 
     def drain(self):
         """
         read data from the data socket until we hit the timeout; returns
         the number of bytes drained
         """
+        assert self._socket is not None
         bytes_read = 0
         # read from the socket until we hit the timeout:
-        while True:
-            try:
+        old_timeout = self._socket.gettimeout()
+        self._socket.settimeout(0.1)
+        try:
+            while True:
                 data = self._socket.recv(4096)
                 bytes_read += len(data)
-            except socket.timeout:
-                return bytes_read
+        except socket.timeout:
+            return bytes_read
+        finally:
+            self._socket.settimeout(old_timeout)
 
 
-class ResultWrap:
-    def __init__(self, start, stop, buf):
-        self._consumed = threading.Event()
-        self.start = start
-        self.stop = stop
-        self.buf = buf[:stop - start]
-        assert buf.shape[0] == stop - start
-
-    def is_released(self, timeout):
-        # called from `ReaderThread` - after data is consumed,
-        # we are free to reuse our buffer
-        return self._consumed.wait(timeout)
-
-    def release(self):
-        self._consumed.set()
-
-
-# FIXME: use ErrThreadMixin and maybe_raise in the pool
-class ReaderThread(threading.Thread):
-    def __init__(self, backend, out_queue, chunk_size, default_timeout=0.2, read_dtype=np.float32,
-                 read_upto_frame=None, *args, **kwargs):
-        super().__init__(name='ReaderThread', *args, **kwargs)
-        self._stop_event = threading.Event()
-        self._eof_event = threading.Event()
-        self._backend = backend
-        self._chunk_size = chunk_size
-        self._out_queue = out_queue
-        self._default_timeout = default_timeout
-        self._read_dtype = read_dtype
-        self._read_upto_frame = read_upto_frame
+class MerlinFrameStream:
+    """
+    This class takes over reading from the `MerlinRawSocket` once the
+    `AcquisitionHeader` has been read.
 
-    def stop(self):
-        self._stop_event.set()
+    It first peeks the first frame header, and then reads multiple frames
+    in stacks of mostly fixed size.
+    """
+    def __init__(
+        self,
+        raw_socket: MerlinRawSocket,
+        acquisition_header: AcquisitionHeader,
+        first_frame_header: FrameHeader,
+    ):
+        self._raw_socket = raw_socket
+        self._acquisition_header = acquisition_header
+        self._first_frame_header = first_frame_header
+        self._frame_counter = 0
 
-    def is_stopped(self):
-        return self._stop_event.is_set()
+    @classmethod
+    def from_frame_header(
+        cls,
+        raw_socket: MerlinRawSocket,
+        acquisition_header: AcquisitionHeader
+    ) -> "MerlinFrameStream":
+        first_frame_header = raw_socket.peek_frame_header()
+        return cls(
+            raw_socket=raw_socket,
+            acquisition_header=acquisition_header,
+            first_frame_header=first_frame_header,
+        )
 
-    def __enter__(self):
-        self.start()
-        return self
+    def read_multi_frames(self, input_buffer, num_frames=32, read_upto_frame=None):
+        """
+        Returns `False` on timeout, `True` in case we are done and don't need to
+        read any more frames (according to `read_upto_frame`), or a
+        `MerlinRawFrames` object
 
-    def __exit__(self, *args, **kwargs):
-        self.stop()
+        On EOF or timeout, can read less than `num_frames`. In that case, `buffer` is sliced
+        to only contain decoded data. `out` will not be fully overwritten in this case
+        and can contain garbage at the end.
 
-    def run(self):
-        try:
-            out = self._backend.get_out_buffer(self._chunk_size, dtype=self._read_dtype)
-            input_buffer = self._backend.get_input_buffer(num_frames=self._chunk_size)
-            should_exit = False
-            while not should_exit:
-                if self.is_stopped():
-                    break
-                res = self._backend.read_multi_frames(
-                    out=out,
-                    num_frames=self._chunk_size,
-                    input_buffer=input_buffer,
-                    timeout=self._default_timeout,
-                    read_upto_frame=self._read_upto_frame,
+        `read_upto_frame` can be used to only read up to a total number of frames.
+        Once this number is reached, we behave the same way as if we had reached EOF.
+        """
+        assert self._first_frame_header is not None
+        header_size = int(self._first_frame_header.header_size_bytes) + 15
+        bytes_per_frame = header_size + self._first_frame_header.image_size_bytes
+
+        input_buffer = memoryview(input_buffer)
+        if read_upto_frame is not None:
+            num_frames = min(num_frames, read_upto_frame - self._frame_counter)
+            input_buffer = input_buffer[:num_frames * bytes_per_frame]
+            if num_frames == 0:
+                return True  # we are done.
+        bytes_read = self._raw_socket.read_into(input_buffer)
+        frames_read = bytes_read // bytes_per_frame
+        if bytes_read % bytes_per_frame != 0:
+            raise EOFError(
+                "input data stream truncated (%d,%d)" % (
+                    bytes_read, bytes_per_frame
                 )
-                if res is False:
-                    continue  # timeout, give main thread the chance to stop us
-                if res is True:
-                    break  # we are done
-                res_buffer, res_start, res_stop = res
-
-                # EOF, no frames left on the socket:
-                if res_stop - res_start == 0:
-                    break
-
-                wrapped = ResultWrap(res_start, res_stop, res_buffer)
-
-                # retry until there is space in the output queue, or the thread is stopped:
-                while True:
-                    try:
-                        self._out_queue.put(wrapped, timeout=self._default_timeout)
-                        break
-                    except queue.Full:
-                        if self.is_stopped():
-                            should_exit = True
-                            break
-
-                # retry until value is consumed
-                while not wrapped.is_released(timeout=self._default_timeout):
-                    if self.is_stopped():  # break out of outer loop
-                        should_exit = True
-                        break
-        finally:
-            self.stop()  # make sure the stopped flag is set in any case
-
+            )
 
-class ReaderPoolImpl:
-    def __init__(self, backend, pool_size, chunk_size, read_upto_frame):
-        self._pool_size = pool_size
-        self._backend = backend
-        self._chunk_size = chunk_size
-        self._out_queue = queue.Queue()  # TODO: possibly limit size?
-        self._threads = None
-        self._read_upto_frame = read_upto_frame
+        start_idx = self._frame_counter
 
-    def __enter__(self):
-        self._threads = []
-        for i in range(self._pool_size):
-            t = ReaderThread(
-                backend=self._backend,
-                chunk_size=self._chunk_size,
-                out_queue=self._out_queue,
-                read_upto_frame=self._read_upto_frame,
-            )
-            t.start()
-            self._threads.append(t)
-        return self
+        self._frame_counter += frames_read
+        if bytes_read == 0:
+            # timeout or EOF without any data read:
+            return False
 
-    def __exit__(self, *args, **kwargs):
-        logger.debug("ReaderPoolImpl.__exit__: stopping threads")
-        for t in self._threads:  # TODO: handle errors on stopping/joining? re-throw exceptions?
-            t.stop()
-            logger.debug("ReaderPoolImpl: stop signal set")
-            t.join()
-            logger.debug("ReaderPoolImpl: thread joined")
-        logger.debug("ReaderPoolImpl.__exit__: threads stopped")
+        end_idx = start_idx + frames_read
 
-    @contextlib.contextmanager
-    def get_result(self):
-        while True:
-            try:
-                res = self._out_queue.get(timeout=0.2)
-                yield res
-                res.release()
-                return
-            except queue.Empty:
-                if self.should_stop():
-                    yield None
-                    return
-
-    def should_stop(self):
-        return any(
-            t.is_stopped()
-            for t in self._threads
+        return MerlinRawFrames(
+            input_buffer[:bytes_read],
+            start_idx,
+            end_idx,
+            self._first_frame_header,
         )
 
+    def get_input_buffer(self, num_frames: int) -> bytearray:
+        assert self._first_frame_header is not None
+        header_size = int(self._first_frame_header.header_size_bytes) + 15
+        image_size = int(self._first_frame_header.image_size_bytes)
+        read_size = num_frames*(header_size + image_size)
+        input_bytes = bytearray(read_size)
+        return input_bytes
 
-class ReaderPool:
-    def __init__(self, backend, pool_size):
-        self._backend = backend
-        self._pool_size = pool_size
-
-    def get_impl(self, chunk_size=10, read_upto_frame=None):
-        """
-        Returns a new `ReaderPoolImpl`, which will read up to
-        the frame index given in `read_upto_frame`, or all frames
-        in case it is `None`.
-        """
-        return ReaderPoolImpl(
-            backend=self._backend,
-            pool_size=self._pool_size,
-            chunk_size=chunk_size,
-            read_upto_frame=read_upto_frame,
-        )
+    def get_first_frame_header(self) -> FrameHeader:
+        return self._first_frame_header
 
 
 class MerlinDataSource:
-    def __init__(self, host, port, pool_size=2):
-        self.socket = MerlinDataSocket(host=host, port=port)
-        self.pool = ReaderPool(backend=self.socket, pool_size=pool_size)
+    def __init__(
+        self,
+        host,
+        port,
+        pool_size=2,
+        sig_shape=None,
+        timeout: Optional[float] = None
+    ):
+        self._sig_shape = sig_shape
+        self.socket = MerlinRawSocket(
+            host=host,
+            port=port,
+            timeout=timeout,
+        )
 
     def __enter__(self):
         self.socket.__enter__()
 
     def __exit__(self, *args, **kwargs):
         self.socket.__exit__(*args, **kwargs)
 
-    def inline_stream(self, read_dtype=np.float32, chunk_size=10):
-        self.socket.read_headers()
-        hdr = self.socket.get_acquisition_header()
-        logger.info(hdr)
+    def inline_stream(self, read_dtype=np.float32, chunk_size=10, num_frames=None):
+        chunks = self._read_and_decode(
+            read_dtype=read_dtype,
+            chunk_size=chunk_size,
+            num_frames=num_frames,
+        )
+        for chunk in chunks:
+            yield chunk.buf
+
+    def _read_and_decode(
+        self, read_dtype=np.float32, chunk_size=10, num_frames=None
+    ) -> Generator[MerlinDecodedFrames, None, None]:
+        acq_header = self.socket.read_acquisition_header()
+        stream = MerlinFrameStream.from_frame_header(
+            raw_socket=self.socket,
+            acquisition_header=acq_header,
+        )
+
+        logger.info(acq_header)
 
-        out = self.socket.get_out_buffer(chunk_size, dtype=read_dtype)
-        input_buffer = self.socket.get_input_buffer(num_frames=chunk_size)
+        frame_hdr = stream.get_first_frame_header()
+        logger.info(frame_hdr)
+
+        sig_shape = validate_get_sig_shape(frame_hdr, self._sig_shape)
+        out = np.zeros((chunk_size,) + sig_shape, dtype=read_dtype)
+        input_buffer = stream.get_input_buffer(num_frames=chunk_size)
 
         while True:
-            res = self.socket.read_multi_frames(
-                out=out,
+            res = stream.read_multi_frames(
                 num_frames=chunk_size,
-                input_buffer=input_buffer
+                input_buffer=input_buffer,
+                read_upto_frame=num_frames,
             )
             if not res:
                 break
             if res is True:
                 break
-            buf, frame_idx_start, frame_idx_end = res
-            if frame_idx_end - frame_idx_start == 0:
-                break
-            yield buf
+            yield MerlinDecodedFrames.from_raw(res, out)
 
-    def stream(self, num_frames=None, chunk_size=11):
+    def stream(self, num_frames=None, chunk_size=11, read_dtype=np.float32):
         """
         Examples
         --------
 
-        >>> source = MerlinDataSource(...)  # doctest: +SKIP
-        >>> with source:  # doctest: +SKIP
-        ...     for _ in source.stream():  # doctest: +SKIP
-        ...         ...
-        """
-        self.socket.read_headers()
-        hdr = self.socket.get_acquisition_header()
-        logger.info(hdr)
-        pool = self.pool.get_impl(
-            read_upto_frame=num_frames,
+        >>> source = MerlinDataSource(
+        ...     host='127.0.0.1',
+        ...     port=MERLIN_DATA_PORT,
+        ... )
+        >>> result = np.zeros((256, 256), dtype=np.float32)
+        >>> with source:
+        ...     for chunk in source.stream(num_frames=128*128, chunk_size=16):
+        ...         result += chunk.buf.sum(axis=0)
+        """
+        chunks = self._read_and_decode(
+            read_dtype=read_dtype,
             chunk_size=chunk_size,
+            num_frames=num_frames,
         )
-        with pool:
-            while True:
-                with pool.get_result() as res_wrapped:
-                    if pool.should_stop():
-                        break
-                    yield res_wrapped
+        yield from chunks
```

### Comparing `libertem-live-0.1.0/src/libertem_live/detectors/merlin/sim.py` & `libertem-live-0.2.0/src/libertem_live/detectors/merlin/sim.py`

 * *Files 23% similar despite different names*

```diff
@@ -3,132 +3,33 @@
 import mmap
 import time
 import socket
 import itertools
 import functools
 import platform
 import threading
-from typing import Optional
 import logging
 import select
+from typing import List, Dict
 
 import click
 import numpy as np
 from tqdm import tqdm
 
 from libertem.io.dataset.base import TilingScheme
 from libertem.io.dataset.mib import MIBDataSet, is_valid_hdr
 from libertem.common import Shape
 
+from libertem_live.detectors.merlin.data import AcquisitionHeader
+from libertem_live.detectors.common import (
+    UndeadException, StopException, ServerThreadMixin,
+)
 
-logger = logging.getLogger(__name__)
-
-
-# Copied from the k2is branch as a temporary fix.
-# FIXME use a proper import as soon as the k2is branch is merged
-class StoppableThreadMixin:
-    def __init__(self, *args, **kwargs):
-        self._stop_event = threading.Event()
-        super().__init__(*args, **kwargs)
-
-    def stop(self):
-        self._stop_event.set()
-
-    def is_stopped(self):
-        return self._stop_event.is_set()
-
-
-# Copied from the k2is branch as a temporary fix.
-# FIXME use a proper import as soon as the k2is branch is merged
-class ErrThreadMixin(StoppableThreadMixin):
-    def __init__(self, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._error: Optional[Exception] = None
-
-    def get_error(self):
-        return self._error
-
-    def error(self, exc):
-        logger.error("got exception %r, shutting down thread", exc)
-        self._error = exc
-        self.stop()
-
-    def maybe_raise(self):
-        if self._error is not None:
-            raise self._error
-
-
-class ServerThreadMixin(ErrThreadMixin):
-    def __init__(self, host, port, name, *args, **kwargs):
-        super().__init__(*args, **kwargs)
-        self._socket = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
-        self._host = host
-        self._port = port
-        self._name = name
-        self.listen_event = threading.Event()
-
-    def wait_for_listen(self, timeout=10):
-        """
-        To be called from the main thread
-        """
-        t0 = time.time()
-        while time.time() - t0 < timeout:
-            if self.listen_event.wait(timeout=0.1):
-                return
-            self.maybe_raise()
-        if not self.listen_event.is_set():
-            raise RuntimeError("failed to start in %f seconds" % timeout)
-
-    @property
-    def sockname(self):
-        return self._socket.getsockname()
-
-    def handle_conn(self, connection):
-        raise NotImplementedError
 
-    def run(self):
-        try:
-            self._socket.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
-            self._socket.bind((self._host, self._port))
-            self._socket.settimeout(1)
-            self._socket.listen(1)
-            print(f"{self._name} listening {self.sockname}")
-            self.listen_event.set()
-            while not self.is_stopped():
-                try:
-                    connection, client_addr = self._socket.accept()
-                    with connection:
-                        print(f"{self._name} accepted from %s" % (client_addr,))
-                        self.handle_conn(connection)
-                except socket.timeout:
-                    continue
-                except ConnectionResetError:
-                    print(f"{self._name} disconnected")
-                # except BrokenPipeError:
-                #     # catch broken pipe error - allow the server to continue
-                #     # running, even when a client prematurely disconnects
-                #     try:
-                #         connection.close()
-                #     except Exception:
-                #         pass
-                #     print(f"{self._name} disconnected")
-                except RuntimeError as e:
-                    print(f"{self._name} exception %s -> stopping" % e)
-                    self.error(e)
-                    break
-                except StopException:
-                    break
-                except Exception as e:
-                    print(f"{self._name} exception? %s" % e)
-                    self.error(e)
-        except Exception as e:
-            return self.error(e)
-        finally:
-            print(f"{self._name} exiting")
-            self._socket.close()
+logger = logging.getLogger(__name__)
 
 
 @functools.lru_cache(maxsize=None)
 def get_mpx_header(length):
     return b"MPX,%010d," % ((length + 1),)
 
 
@@ -140,126 +41,209 @@
     This avoids a dependency on the GPL-licensed
     :class:`~libertem.executor.inline.InlineJobExecutor`.
     '''
     def run_function(self, fn, *args, **kwargs):
         return fn(*args, **kwargs)
 
 
-class StopException(Exception):
-    pass
-
-
-class DataSocketSimulator:
-    def __init__(self, path: str, nav_shape=None, continuous=False, rois=None,
-                 max_runs=-1):
+class HeaderSocketSimulator:
+    def __init__(
+        self,
+        path: str,
+        first_frame_headers: Dict,
+        stop_event=None,
+        nav_shape=None,
+        continuous=False,
+        rois=None,
+    ):
         """
+        This class handles sending out acquisition header - calling the
+        `handle_conn` method will send the header to the give connection.
+
         Parameters
         ----------
 
         path
             Path to the HDR file
 
+        stop_event
+            Will stop gracefully if this event is set.
+
         continuous
             If set to True, will continuously output data
 
         rois: List[np.ndarray]
             If a list of ROIs is given, in continuous mode, cycle through
             these ROIs from the source data
 
-        max_runs: int
-            Maximum number of continuous runs
+        first_frame_headers
+            The frame headers of the first frame, as a dict (as LiberTEM reads
+            them)
         """
-        self.stop_event = threading.Event()
+        if stop_event is None:
+            stop_event = threading.Event()
+        self.stop_event = stop_event
         if rois is None:
             rois = []
         if nav_shape is None and not is_valid_hdr(path):
             raise ValueError("please pass the path to a valid HDR file or specify a nav shape!")
         self._path = path
         self._nav_shape = nav_shape
         self._continuous = continuous
         self._rois = rois
         self._ds = None
-        self._max_runs = max_runs
-        self._mmaps = {}
-
-    def open(self):
-        ds = MIBDataSet(path=self._path, nav_shape=self._nav_shape)
-        ds.initialize(MITExecutor())
-        print("dataset shape: %s" % (ds.shape,))
-        self._ds = ds
-        self._warmup()
+        self._first_frame_headers = first_frame_headers
 
     def _make_hdr(self):
+        # FIXME: support for continuous mode - need to fake a better header here in that case
+        bpp = self._first_frame_headers['bits_per_pixel']
         hdr = (
             f"HDR,\n"
             f"Frames in Acquisition (Number):\t{np.prod(self._nav_shape, dtype=np.int64)}\n"
             f"Frames per Trigger (Number):\t{self._nav_shape[1]}\n"
+            f"Counter Depth (number):\t{bpp}\n"
             f"End\t"
         )
         return hdr.encode('latin1')
 
     @property
-    def hdr(self):
+    def hdr(self) -> bytes:
         if is_valid_hdr(self._path):
             with open(self._path, 'rb') as f:
                 # FIXME: possibly change header in continuous mode?
                 hdr = f.read()
         else:
             hdr = self._make_hdr()
         return hdr
 
+    @property
+    def parsed(self) -> AcquisitionHeader:
+        return AcquisitionHeader.from_raw(self.hdr)
+
     def get_chunks(self):
         """
         generator of `bytes` for the given configuration
         """
-
         # first, send acquisition header:
         hdr = self.hdr
         yield get_mpx_header(len(hdr))
         yield hdr
+
+    def handle_conn(self, conn):
+        for chunk in self.get_chunks():
+            conn.sendall(chunk)
+
+    def is_stopped(self):
+        return self.stop_event.is_set()
+
+
+class DataSocketSimulator:
+    def __init__(self, path: str, stop_event=None, nav_shape=None, continuous=False, rois=None,
+                 max_runs=-1):
+        """
+        Parameters
+        ----------
+
+        path
+            Path to the HDR file
+
+        stop_event
+            Will stop gracefully if this event is set.
+
+        continuous
+            If set to True, will continuously output data
+
+        rois: List[np.ndarray]
+            If a list of ROIs is given, in continuous mode, cycle through
+            these ROIs from the source data
+
+        max_runs: int
+            Maximum number of continuous runs
+        """
+        if stop_event is None:
+            stop_event = threading.Event()
+        self.stop_event = stop_event
+        if rois is None:
+            rois = []
+        if nav_shape is None and not is_valid_hdr(path):
+            raise ValueError("please pass the path to a valid HDR file or specify a nav shape!")
+        self._path = path
+        self._nav_shape = nav_shape
+        self._continuous = continuous
+        self._rois = rois
+        self._ds = None
+        self._max_runs = max_runs
+        self._mmaps = {}
+
+    def get_ds_shape(self) -> Shape:
+        self._load()
+        assert self._ds is not None
+        return self._ds.shape
+
+    def _load(self):
+        if self._ds is None:
+            ds = MIBDataSet(path=self._path, nav_shape=self._nav_shape)
+            ds.initialize(MITExecutor())
+            self._ds = ds
+
+    def open(self):
+        self._load()
+        assert self._ds is not None
+        logger.info(f"dataset shape: {self._ds.shape}")
+        self._warmup()
+
+    def get_chunks(self):
+        """
+        generator of `bytes` for the given configuration
+        """
         if self._continuous:
-            print("yielding from continuous")
+            logger.info("yielding from continuous")
             yield from self._get_continuous()
         else:
-            print("yielding from single scan")
+            logger.info("yielding from single scan")
             roi = np.ones(self._ds.shape.nav, dtype=bool)
-            t = tqdm(total=np.count_nonzero(roi))
+            # Times two since _get_single_scan() returns header
+            # and frame separately
+            t = tqdm(total=np.count_nonzero(roi)*2)
             try:
                 for item in self._get_single_scan(roi):
                     yield item
                     t.update(1)
             finally:
                 t.close()
 
     def _read_frame_w_header(self, fh, frame_idx, full_frame_size):
         """
         Parameters
         ----------
 
-        fh : LocalFile
+        fh : MMapFile or LocalFile
 
         frame_idx : int
             File-relative frame index
 
         full_frame_size : int
             Size of header plus frame in bytes
         """
-        if fh._file is None:
-            fh.open()
-        f = fh._file
-        fileno = f.fileno()
-        if fileno not in self._mmaps:
-            self._mmaps[fileno] = raw_mmap = mmap.mmap(
+        if hasattr(fh, '_file'):
+            if fh._file is None:
+                fh.open()
+            f = fh._file
+        else:
+            f = open(fh._path, 'rb')
+        path = fh._path
+        if path not in self._mmaps:
+            self._mmaps[path] = raw_mmap = mmap.mmap(
                 fileno=f.fileno(),
                 length=0,
                 offset=0,
                 access=mmap.ACCESS_READ,
             )
         else:
-            raw_mmap = self._mmaps[fileno]
+            raw_mmap = self._mmaps[path]
 
         return bytearray(raw_mmap[
             full_frame_size * frame_idx: full_frame_size * (frame_idx + 1)
         ])
 
     def _warmup(self):
         fileset = self._ds._get_fileset()
@@ -273,14 +257,20 @@
             start_at_frame=0,
             stop_before_frame=int(np.prod(self._ds.shape.nav)),
             dtype=np.float32,  # FIXME: don't really care...
             tiling_scheme=tiling_scheme,
             roi=None,
         )
 
+    @property
+    def first_frame_headers(self) -> Dict:
+        self.open()
+        first_file = self._ds._files_sorted[0]
+        return first_file.fields
+
     def _get_single_scan(self, roi):
         fileset = self._ds._get_fileset()
         ds_shape = self._ds.shape
         tiling_scheme = TilingScheme.make_for_shape(
             tileshape=Shape((1,) + tuple(ds_shape.sig),
                             sig_dims=ds_shape.sig.dims),
             dataset_shape=ds_shape,
@@ -307,30 +297,32 @@
             # shape = slices[idx, 1]
             # origin, shape = slices[idx]
             tile_ranges = ranges[idx][0]
             file_idx = tile_ranges[0]
             fh = fileset[file_idx]
             global_idx = origin[0]
             local_idx = global_idx - fh.start_idx
-            frame_w_header = self._read_frame_w_header(fh, local_idx, full_frame_size)
+            frame_w_header = self._read_frame_w_header(
+                fh, local_idx, full_frame_size
+            )
             yield mpx_header
             yield frame_w_header
 
     def _get_continuous(self):
         if self._rois:
             rois = self._rois
         else:
             rois = [np.ones(self._ds.shape.nav, dtype=bool)]
 
         i = 0
         for roi in itertools.cycle(rois):
             t0 = time.time()
             yield from self._get_single_scan(roi)
             t1 = time.time()
-            print("cycle %d took %.05fs" % (i, t1 - t0))
+            logger.info("cycle %d took %.05fs" % (i, t1 - t0))
             i += 1
             if self._max_runs != -1 and i >= self._max_runs:
                 raise StopException("max_runs exceeded")
 
     def handle_conn(self, conn):
         for chunk in self.get_chunks():
             conn.sendall(chunk)
@@ -389,25 +381,31 @@
             else:
                 raise RuntimeError("The memfd cache is only supported on Linux.")
         super().open()
         self._cache_fd = memfd.memfd_create("sim_cache", 0)
         self._populate_cache()
 
     def _populate_cache(self):
-        print("populating cache, please wait...")
+        logger.info("populating cache, please wait...")
         roi = np.ones(self._ds.shape.nav, dtype=bool)
         total_size = 0
         for chunk in super()._get_single_scan(roi):
             if self.is_stopped():
                 raise StopException("Server stopped")
-            os.write(self._cache_fd, chunk)
+            written = 0
+            while written < len(chunk):
+                written += os.write(self._cache_fd, chunk[written:])
             total_size += len(chunk)
         os.lseek(self._cache_fd, 0, 0)
         self._size = total_size
-        print("cache populated, total size = %d MiB" % (total_size / 1024 / 1024))
+        logger.info(
+            "cache populated, total size = %d MiB (%d bytes)" % (
+                total_size / 1024 / 1024, total_size
+            )
+        )
 
     def _send_full_file(self, conn):
         os.lseek(self._cache_fd, 0, 0)
         total_sent = 0
         reps = 0
         while total_sent < self._size:
             if self.is_stopped():
@@ -415,184 +413,231 @@
             total_sent += os.sendfile(
                 conn.fileno(),
                 self._cache_fd,
                 total_sent,  # offset ->
                 self._size - total_sent
             )
             reps += 1
-        print("_send_full_file took %d reps" % reps)
+        logger.info("_send_full_file took %d reps" % reps)
 
     def handle_conn(self, conn):
-        # first, send acquisition header:
-        hdr = self.hdr
-        # FIXME: possibly change header in continuous mode?
-        conn.sendall(get_mpx_header(len(hdr)))
-        conn.sendall(hdr)
         if self._continuous:
             i = 0
             while True:
                 t0 = time.time()
                 self._send_full_file(conn)
                 t1 = time.time()
                 throughput = self._size / (t1 - t0) / 1024 / 1024
-                print("cycle %d took %.05fs (%.2fMiB/s)" % (i, t1 - t0, throughput))
+                logger.info("cycle %d took %.05fs (%.2fMiB/s)" % (i, t1 - t0, throughput))
                 i += 1
                 if self._max_runs != -1 and i >= self._max_runs:
                     raise StopException("max_runs exceeded")
         else:
-            print("yielding from single scan")
+            logger.info("yielding from single scan")
             t0 = time.time()
             self._send_full_file(conn)
             t1 = time.time()
             throughput = self._size / (t1 - t0) / 1024 / 1024
-            print("single scan took %.05fs (%.2fMiB/s)" % (t1 - t0, throughput))
+            logger.info(f"single scan took {t1 - t0:.05f}s ({throughput:.2f}MiB/s)")
         conn.close()
 
 
+def wait_with_socket(event: threading.Event, connection):
+    while True:
+        if event.wait(0.1):
+            # the event is set, break out of the loop and
+            # return True to signal that normal operation
+            # can continue
+            return True
+        (readable, writable, exceptional) = select.select(
+            [connection], [connection], [connection], 0.1
+        )
+        if readable:
+            # The connection is unidirectional, we don't receive any data
+            # normally, but only send
+            res = connection.recv(1)
+            if not res:
+                logger.info("Readable socket yielded no result, probably closed")
+                # The socket was closed, return False to signal abort
+                return False
+
+
 class DataSocketServer(ServerThreadMixin, threading.Thread):
-    def __init__(self, sim: DataSocketSimulator,
-            host='0.0.0.0', port=6342, wait_trigger=False, garbage=False):
+    def __init__(self, headers: HeaderSocketSimulator, sim: DataSocketSimulator,
+            stop_event, acquisition_event, trigger_event, finish_event,
+            host='0.0.0.0', port=6342, wait_trigger=False, garbage=False, manual_trigger=False):
+        self.acquisition_event = acquisition_event
+        self.trigger_event = trigger_event
+        self.finish_event = finish_event
+        self._headers = headers
         self._sim = sim
-        super().__init__(host=host, port=port, name=self.__class__.__name__)
-        self._sim.stop_event = self._stop_event
-        self.trigger_event = threading.Event()
-        self.finish_event = threading.Event()
+        super().__init__(host=host, port=port, name=self.__class__.__name__, stop_event=stop_event)
+
         self._wait_trigger = wait_trigger
         if garbage and not wait_trigger:
             raise ValueError("Can only send garbage if wait_trigger is set!")
+        self._manual_trigger = manual_trigger
+        if wait_trigger and manual_trigger:
+            raise ValueError('Cannot have both wait softtrigger and manual trigger')
         self._garbage = garbage
 
+    def get_sim(self):
+        return self._sim
+
     def run(self):
         try:
             self._sim.open()
             super().run()
         except Exception as e:
             return self.error(e)
 
     def handle_conn(self, connection):
         try:
-            if self._wait_trigger:
+            if self._wait_trigger or self._manual_trigger:
                 if self._garbage:
-                    print("Sending some garbage...")
+                    logger.info("Sending some garbage...")
                     connection.send(b'GARBAGEGARBAGEGARBAGE'*1024)
-                print("Waiting for trigger...")
-                while True:
-                    if self.trigger_event.wait(0.1):
-                        # the trigger event is set, break out of the loop and
-                        # handle the connection below:
-                        break
-                    (readable, writable, exceptional) = select.select(
-                        [connection], [connection], [connection], 0.1
-                    )
-                    if readable:
-                        # The connection is unidirectional, we don't receive any data
-                        # normally, but only send
-                        res = connection.recv(1)
-                        if not res:
-                            print("Readable socket yielded no result, probably closed")
-                            connection.close()
-                            return
+                logger.info("Waiting for acquisition start...")
+                if not wait_with_socket(self.acquisition_event, connection):
+                    logger.info("Readable socket yielded no result, probably closed")
+                    connection.close()
+                    return
+                self.acquisition_event.clear()
+            self._headers.handle_conn(connection)
+            if self._manual_trigger:
+                _ = input("Press key to trigger...\n")
+                self.trigger_event.set()
+            if self._wait_trigger or self._manual_trigger:
+                logger.info("Waiting for trigger...")
+                if not wait_with_socket(self.trigger_event, connection):
+                    logger.info("Readable socket yielded no result, probably closed")
+                    connection.close()
+                    return
                 self.trigger_event.clear()
             return self._sim.handle_conn(connection)
         finally:
             self.finish_event.set()
 
 
 class ControlSocketServer(ServerThreadMixin, threading.Thread):
-    def __init__(self, trigger_event, host='0.0.0.0', port=6341):
+    def __init__(
+        self, acquisition_event, trigger_event, stop_event=None,
+        host='0.0.0.0', port=6341, initial_params=None,
+    ):
         self._trigger_event = trigger_event
+        self._acquisition_event = acquisition_event
         self._params = {}
-        super().__init__(host=host, port=port, name=self.__class__.__name__)
+        if initial_params is not None:
+            self._params = initial_params
+        super().__init__(host=host, port=port, name=self.__class__.__name__, stop_event=stop_event)
+
+    def encode_response(self, response_parts: List[str]) -> bytes:
+        resp_len = len(",".join(response_parts).encode("ASCII"))
+        parts = [
+            "MPX",
+            f"{resp_len:010d}",  # 1
+        ] + response_parts
+        response_str = ','.join(parts)
+        return response_str.encode("ascii")
 
     def handle_conn(self, connection):
         connection.settimeout(1)
-        print("handling control connection")
+        logger.info("handling control connection")
         # This code is only a proof of concept. It works just well enough to send
         # commands and parse responses with control.MerlinControl.
         # A few points to improve:
         # * Handle incomplete messages properly. Right now,
         #   the assumption is that a complete command will be received with
         #   recv() and a complete response will be sent with send()
         # * Figure out the missing parts of the response to match Merlin behavior
         # * Actually respond to commands that can be simulated, such as 'numframes'
         # * Possibly emit errors like a real Merlin detector upon bad commands?
+        #       error codes:
+        #       0 -> success
+        #       1 -> busy
+        #       2 -> command not recognized
+        #       3 -> parameter out of range
         while not self.is_stopped():
             try:
                 chunk = connection.recv(1024*1024)
             except socket.timeout:
                 continue
             if len(chunk) == 0:
-                print("closed control")
+                logger.info("closed control")
                 return
             parts = chunk.split(b',')
-            print("Control command received: ", chunk)
+            logger.info(f"Control command received: {chunk}")
             parts = [part.decode('ascii') for part in parts]
             method = parts[2]
             param = parts[3]
-            if method == 'SET':
-                value = parts[4]
             if method == 'GET':
-                response_parts = (
-                    "noideafirst",
-                    "noideasecond",
-                    method,
-                    "noideafourth",
-                    self._params.get(param, "undef"),
-                    "0"
+                response = self.encode_response(
+                    response_parts=[
+                        method,
+                        param,
+                        self._params.get(param, "undef"),
+                        "0"  # error code: success
+                    ]
                 )
             elif method == 'SET':
+                # handle the actual operation:
+                value = parts[4]
                 self._params[param] = value
-                response_parts = (
-                    "noideafirst",  # 0
-                    "noideasecond",  # 1
-                    method,  # 2
-                    "noideafourth",  # 3
-                    "0",  # 4
+
+                # and generate a response
+                response = self.encode_response(
+                    response_parts=[
+                        method,  # 2
+                        param,  # 3
+                        "0",  # 4 - error code: success
+                    ]
                 )
             elif method == 'CMD':
                 if param == 'SOFTTRIGGER':
                     self._trigger_event.set()
-                response_parts = (
-                    "noideafirst",  # 0
-                    "noideasecond",  # 1
-                    method,  # 2
-                    "noideafourth",  # 3
-                    "0",  # 4
+                elif param == 'STARTACQUISITION':
+                    self._acquisition_event.set()
+
+                response = self.encode_response(
+                    response_parts=[
+                        method,  # 2
+                        param,  # 3
+                        "0",  # error code: success
+                    ]
                 )
             else:
                 raise RuntimeError("Unknown method %s", method)
-            response_str = ','.join(response_parts)
-            print("Control response: ", response_str)
-            connection.send(response_str.encode('ascii'))
+            logger.info(f"Control response: {str(response)}")
+            connection.send(response)
 
 
 class TriggerSocketServer(ServerThreadMixin, threading.Thread):
-    def __init__(self, trigger_event, finish_event, host='0.0.0.0', port=6343):
+    def __init__(self, trigger_event, finish_event, stop_event=None, host='0.0.0.0', port=6343):
         self._trigger_event = trigger_event
         self._finish_event = finish_event
-        super().__init__(host, port, name=self.__class__.__name__)
+        super().__init__(host, port, name=self.__class__.__name__, stop_event=stop_event)
 
     def handle_conn(self, connection):
         connection.settimeout(1)
-        print("handling trigger connection")
+        logger.info("handling trigger connection")
         while not self.is_stopped():
             try:
                 chunk = connection.recv(1024)
             except socket.timeout:
                 continue
             if len(chunk) == 0:
-                print("closed trigger control")
+                logger.info("closed trigger control")
                 return
             if chunk == b'TRIGGER\n':
-                print("Triggered, waiting for finish!")
+                logger.info("Triggered, waiting for finish!")
                 self._finish_event.clear()
                 self._trigger_event.set()
                 self._finish_event.wait()
                 connection.send(b'FINISH\n')
-                print("Finished!")
+                logger.info("Finished!")
                 self._finish_event.clear()
 
 
 class TriggerClient():
     def __init__(self, host='localhost', port=6343):
         self._host = host
         self._port = port
@@ -602,27 +647,150 @@
         s = socket.socket(socket.AF_INET, socket.SOCK_STREAM)
         s.connect((self._host, self._port))
         s.setsockopt(socket.SOL_SOCKET, socket.SO_REUSEADDR, 1)
         s.settimeout(1)
         self._socket = s
 
     def trigger(self):
+        assert self._socket is not None, "need to be connected"
         self._socket.send(b'TRIGGER\n')
 
     def wait(self):
+        assert self._socket is not None, "need to be connected"
         while True:
             try:
                 res = self._socket.recv(1024)
                 if res == b'FINISH\n':
                     break
             except socket.timeout:
                 pass
 
     def close(self):
-        self._socket.close()
+        if self._socket is not None:
+            self._socket.close()
+            self._socket = None
+
+
+class CameraSim:
+    def __init__(
+        self, path, nav_shape, continuous=False,
+        host='0.0.0.0', data_port=6342, control_port=6341,
+        trigger_port=6343, wait_trigger=False, garbage=False,
+        cached=None, max_runs=-1, initial_params=None,
+        manual_trigger=False,
+    ):
+        if garbage:
+            wait_trigger = True
+
+        if cached == 'MEM':
+            cls = CachedDataSocketSim
+        elif cached == 'MEMFD':
+            cls = MemfdSocketSim
+        else:
+            cls = DataSocketSimulator
+
+        if nav_shape == (0, 0):
+            nav_shape = None
+
+        self.stop_event = threading.Event()
+        self.acquisition_event = threading.Event()
+        self.trigger_event = threading.Event()
+        self.finish_event = threading.Event()
+
+        self.sim = cls(
+            path=path, nav_shape=nav_shape, continuous=continuous, max_runs=max_runs,
+            stop_event=self.stop_event,
+        )
+
+        self.headers = HeaderSocketSimulator(
+            path=path, nav_shape=nav_shape, continuous=continuous,
+            stop_event=self.stop_event, first_frame_headers=self.sim.first_frame_headers,
+        )
+
+        self.server_t = DataSocketServer(
+            headers=self.headers, sim=self.sim, host=host, port=data_port,
+            wait_trigger=wait_trigger, garbage=garbage, manual_trigger=manual_trigger,
+            stop_event=self.stop_event,
+            acquisition_event=self.acquisition_event,
+            trigger_event=self.trigger_event,
+            finish_event=self.finish_event,
+        )
+        # Make sure the thread dies with the main program
+        self.server_t.daemon = True
+
+        if initial_params is None:
+            # make some effort to populate useful parameters:
+            shape = self.server_t.get_sim().get_ds_shape()
+            acq_hdr = self.headers.parsed
+            initial_params = {
+                'IMAGEX': str(shape.sig[1]),
+                'IMAGEY': str(shape.sig[0]),
+                'COUNTERDEPTH': acq_hdr.raw_keys['Counter Depth (number)'],
+            }
+
+        self.control_t = ControlSocketServer(
+            host=host,
+            port=control_port,
+            stop_event=self.stop_event,
+            acquisition_event=self.acquisition_event,
+            trigger_event=self.trigger_event,
+            initial_params=initial_params,
+        )
+        # Make sure the thread dies with the main program
+        self.control_t.daemon = True
+
+        self.trigger_t = TriggerSocketServer(
+            host=host, port=trigger_port,
+            stop_event=self.stop_event,
+            trigger_event=self.trigger_event,
+            finish_event=self.finish_event,
+        )
+        # Make sure the thread dies with the main program
+        self.trigger_t.daemon = True
+
+    def start(self):
+        self.server_t.start()
+        self.control_t.start()
+        self.trigger_t.start()
+
+    def wait_for_listen(self):
+        self.server_t.wait_for_listen()
+        self.control_t.wait_for_listen()
+        self.trigger_t.wait_for_listen()
+
+    def is_alive(self):
+        return self.control_t.is_alive() and self.server_t.is_alive() and self.trigger_t.is_alive()
+
+    def maybe_raise(self):
+        self.control_t.maybe_raise()
+        self.server_t.maybe_raise()
+        self.trigger_t.maybe_raise()
+
+    def stop(self):
+        logger.info("Stopping...")
+        self.stop_event.set()
+        timeout = 2
+        start = time.time()
+        while True:
+            self.control_t.maybe_raise()
+            self.server_t.maybe_raise()
+            self.trigger_t.maybe_raise()
+            if (
+                    (not self.control_t.is_alive())
+                    and (not self.server_t.is_alive())
+                    and (not self.trigger_t.is_alive())
+            ):
+                break
+
+            if (time.time() - start) >= timeout:
+                # Since the threads are daemon threads, they will die abruptly
+                # when this main thread finishes. This is at the discretion of the caller.
+                raise UndeadException("Server threads won't die")
+            time.sleep(0.1)
+        logger.info(f"stopping took {time.time() - start}s")
 
 
 @click.command()
 @click.argument('path', type=click.Path(exists=True))
 @click.option('--nav-shape', type=(int, int), default=(0, 0))
 @click.option('--continuous', default=False, is_flag=True)
 @click.option('--cached', default='NONE', type=click.Choice(
@@ -637,94 +805,49 @@
 @click.option('--trigger-port', type=int, default=6343)
 @click.option(
     '--wait-trigger', default=False, is_flag=True,
     help="Wait for a SOFTTRIGGER command on the control port, "
          "or a trigger signal on the trigger socket",
 )
 @click.option(
+    '--manual-trigger', default=False, is_flag=True,
+    help="Wait for a manual trigger by user input after ARM",
+)
+@click.option(
     '--garbage', default=False, is_flag=True,
     help="Send garbage before trigger. Implies --wait-trigger"
 )
 @click.option('--max-runs', type=int, default=-1)
 def main(path, nav_shape, continuous,
-        host, data_port, control_port, trigger_port, wait_trigger, garbage, cached, max_runs):
-
-    if garbage:
-        wait_trigger = True
-
-    if cached == 'MEM':
-        cls = CachedDataSocketSim
-    elif cached == 'MEMFD':
-        cls = MemfdSocketSim
-    else:
-        cls = DataSocketSimulator
-
-    if nav_shape == (0, 0):
-        nav_shape = None
-
-    sim = cls(path=path, nav_shape=nav_shape, continuous=continuous, max_runs=max_runs)
-
-    server_t = DataSocketServer(
-        sim=sim, host=host, port=data_port, wait_trigger=wait_trigger, garbage=garbage
-    )
-    # Make sure the thread dies with the main program
-    server_t.daemon = True
-    server_t.start()
-
-    control_t = ControlSocketServer(
-        host=host,
-        port=control_port,
-        trigger_event=server_t.trigger_event,
-    )
-    # Make sure the thread dies with the main program
-    control_t.daemon = True
-    control_t.start()
-
-    trigger_t = TriggerSocketServer(
-        host=host, port=trigger_port,
-        trigger_event=server_t.trigger_event,
-        finish_event=server_t.finish_event,
+        host, data_port, control_port, trigger_port, wait_trigger,
+        manual_trigger, garbage, cached, max_runs):
+    logging.basicConfig(level=logging.INFO)
+    camera_sim = CameraSim(
+        path=path, nav_shape=nav_shape, continuous=continuous,
+        host=host, data_port=data_port, control_port=control_port, trigger_port=trigger_port,
+        wait_trigger=wait_trigger, garbage=garbage, cached=cached, max_runs=max_runs,
+        manual_trigger=manual_trigger,
     )
-    # Make sure the thread dies with the main program
-    trigger_t.daemon = True
-    trigger_t.start()
 
+    camera_sim.start()
     # This allows us to handle Ctrl-C, and the main program
     # stops in a timely fashion when continuous scanning stops.
     try:
-        while control_t.is_alive() and server_t.is_alive() and trigger_t.is_alive():
-            control_t.maybe_raise()
-            server_t.maybe_raise()
-            trigger_t.maybe_raise()
+        while camera_sim.is_alive():
+            camera_sim.maybe_raise()
             time.sleep(1)
     except KeyboardInterrupt:
         # Just to not print "Aborted!"" from click
         sys.exit(0)
     finally:
         print("Stopping...")
-        control_t.stop()
-        server_t.stop()
-        trigger_t.stop()
-        timeout = 2
-        start = time.time()
-        while True:
-            control_t.maybe_raise()
-            server_t.maybe_raise()
-            trigger_t.maybe_raise()
-            if (
-                    (not control_t.is_alive())
-                    and (not server_t.is_alive())
-                    and (not trigger_t.is_alive())
-            ):
-                break
-
-            if (time.time() - start) >= timeout:
-                print("Killing server threads")
-                # Since the threads are daemon threads, they will die abruptly
-                # when this main thread finishes.
-                break
-
-            time.sleep(0.1)
+        try:
+            camera_sim.stop()
+        except UndeadException:
+            print("Killing server threads")
+            # Since the threads are daemon threads, they will die abruptly
+            # when this main thread finishes.
+            return
 
 
 if __name__ == "__main__":
     main()
```

### Comparing `libertem-live-0.1.0/src/libertem_live/detectors/merlin/tango_server.py` & `libertem-live-0.2.0/src/libertem_live/detectors/merlin/tango_server.py`

 * *Files identical despite different names*

### Comparing `libertem-live-0.1.0/src/libertem_live/udf/monitor.py` & `libertem-live-0.2.0/src/libertem_live/udf/monitor.py`

 * *Files 26% similar despite different names*

```diff
@@ -1,7 +1,9 @@
+import numpy as np
+
 from libertem.udf import UDF
 
 
 class SignalMonitorUDF(UDF):
     '''
     Return the most recently processed signal space element (frame).
 
@@ -9,22 +11,88 @@
     an offline dataset are more easily accessible with
     :class:`~libertem.udf.raw.PickUDF`.
 
     The result is most likely the last frame of each partition for the
     individual merge steps. The end result depends on the merge order.
     '''
 
-    def get_preferred_input_dtype(self):
-        return self.USE_NATIVE_DTYPE
+    def get_backends(self):
+        ''
+        return [
+            backend for backend in self.BACKEND_ALL
+            if backend not in {self.BACKEND_CUPY_SCIPY_COO, self.BACKEND_SCIPY_COO}
+        ]
+
+    # def get_preferred_input_dtype(self):
+    #     ''
+    #     return self.USE_NATIVE_DTYPE
 
     def get_result_buffers(self):
+        ''
         return {
-            "intensity": self.buffer(kind='sig', dtype=self.meta.input_dtype)
+            "intensity": self.buffer(kind='sig', dtype=self.meta.input_dtype, where='device')
         }
 
     def process_tile(self, tile):
+        ''
         # Assign the portion from the last frame within the tile
         # to the result buffer
-        self.results.intensity[:] = tile[-1]
+        self.results.intensity[:] = self.forbuf(tile[-1], self.results.intensity)
+
+    def merge(self, dest, src):
+        ''
+        dest.intensity[:] = src.intensity
+
+
+# Largely copied from SumUDF, but separate implementation is
+# desirable, for example since `merge_all()` doesn't make sense
+# here.
+class PartitionMonitorUDF(UDF):
+    """
+    Sum up frames in a partition and update result with
+    the latest partition result.
+
+    This is useful for live processing as a beam monitor if
+    individual frames contain not enough signal. Partial sums of
+    an offline dataset are more easily accessible with
+    :class:`~libertem.udf.sum.SumUDF` with a ROI.
+
+    The result is the sum of the partition that was merged last.
+    The end result depends on the merge order.
+
+    Parameters
+    ----------
+    dtype : numpy.dtype, optional
+        Preferred dtype for computation, default 'float32'. The actual dtype will be determined
+        from this value and the dataset's dtype using :meth:`numpy.result_type`.
+        See also :ref:`udf dtype`.
+
+    """
+    def __init__(self, dtype='float32'):
+        super().__init__(dtype=dtype)
+
+    def get_preferred_input_dtype(self):
+        ''
+        return self.params.dtype
+
+    def get_backends(self):
+        ''
+        return self.BACKEND_ALL
+
+    def get_result_buffers(self):
+        ''
+        return {
+            'intensity': self.buffer(
+                kind='sig', dtype=self.meta.input_dtype, where='device'
+            )
+        }
+
+    def process_tile(self, tile):
+        ''
+        self.results.intensity[:] += self.forbuf(
+            np.sum(tile, axis=0),
+            self.results.intensity
+        )
 
     def merge(self, dest, src):
+        ''
         dest.intensity[:] = src.intensity
```

### Comparing `libertem-live-0.1.0/src/libertem_live.egg-info/PKG-INFO` & `libertem-live-0.2.0/src/libertem_live.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,92 +1,119 @@
 Metadata-Version: 2.1
 Name: libertem-live
-Version: 0.1.0
+Version: 0.2.0
 Summary: Live processing with LiberTEM
 Home-page: https://libertem.github.io/LiberTEM-live
 Author: the LiberTEM team
 Author-email: libertem-dev@googlegroups.com
 License: GPL v3
-Description: |gitter|_ |azure|_ |github|_
-        
-        .. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
-        .. _gitter: https://gitter.im/LiberTEM/Lobby
-        
-        .. |azure| image:: https://dev.azure.com/LiberTEM/LiberTEM-live/_apis/build/status/LiberTEM.LiberTEM-live?branchName=master
-        .. _azure: https://dev.azure.com/LiberTEM/LiberTEM-live/_build/latest?definitionId=5&branchName=master
-        
-        .. |github| image:: https://img.shields.io/badge/GitHub-GPL--3.0-informational
-        .. _github: https://github.com/LiberTEM/LiberTEM-live/
-        
-        LiberTEM-live is an extension module for `LiberTEM
-        <https://libertem.github.io/LiberTEM/>`_ that allows live
-        data processing.
-        
-        .. note::
-          LiberTEM-live is still experimental and under active development, including
-          the overall architecture. New releases can include changes that break
-          backwards compatibility until the code and architecture are proven in
-          practical application and stabilized sufficiently.
-        
-          That being said, we encourage early experimental use, are happy to support
-          real-world application and appreciate feedback! You can contact us by
-          `creating or commenting on an Issue on GitHub
-          <https://github.com/LiberTEM/LiberTEM-live/issues>`_ or in the `LiberTEM
-          Gitter chat <https://gitter.im/LiberTEM/Lobby>`_.
-        
-        LiberTEM `user-defined functions (UDFs)
-        <https://libertem.github.io/LiberTEM/udf.html>`_ are designed to work without
-        modification on both offline data and live data streams. That means all
-        `LiberTEM applications <https://libertem.github.io/LiberTEM/applications.html>`_
-        and `LiberTEM-based modules
-        <https://libertem.github.io/LiberTEM/packages.html>`_ can work with all
-        supported detectors in LiberTEM-live.
-        
-        Installation
-        ------------
-        
-        The short version to install into an existing LiberTEM environment:
-        
-        .. code-block:: shell
-        
-            (libertem) $ python -m pip install "libertem-live"
-        
-        See the `LiberTEM installation instructions
-        <https://libertem.github.io/LiberTEM/install.html>`_ for more details on
-        installing LiberTEM.
-        
-        Detectors
-        ---------
-        
-        * `Quantum Detectors Merlin
-          <https://libertem.github.io/LiberTEM-live/reference.html#quantum-detectors-merlin>`_
-        
-        Support for the Gatan K2 IS is currently under development.
-        
-        License
-        -------
-        
-        LiberTEM-live is licensed under GPLv3. The I/O parts are also available under
-        the MIT license, please see LICENSE files in the subdirectories for details.
-        
 Keywords: electron microscopy
 Platform: UNKNOWN
 Classifier: Development Status :: 4 - Beta
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
 Classifier: License :: OSI Approved :: GNU General Public License v3 (GPLv3)
 Classifier: Operating System :: POSIX :: Linux
 Classifier: Operating System :: MacOS :: MacOS X
 Classifier: Operating System :: Microsoft :: Windows
 Classifier: Environment :: Console
 Classifier: Intended Audience :: Science/Research
 Classifier: Intended Audience :: End Users/Desktop
 Classifier: Intended Audience :: Developers
 Classifier: Natural Language :: English
 Classifier: Topic :: Scientific/Engineering
 Classifier: Topic :: Scientific/Engineering :: Physics
 Classifier: Topic :: Scientific/Engineering :: Visualization
-Requires-Python: >=3.6
+Requires-Python: >=3.7
 Description-Content-Type: text/x-rst
+Provides-Extra: sim
 Provides-Extra: pymemfd
 Provides-Extra: pytango
+License-File: LICENSE
+
+|gitter|_ |azure|_ |github|_ |precommit|_ |zenodo|_
+
+.. |gitter| image:: https://badges.gitter.im/Join%20Chat.svg
+.. _gitter: https://gitter.im/LiberTEM/Lobby
+
+.. |azure| image:: https://dev.azure.com/LiberTEM/LiberTEM-live/_apis/build/status/LiberTEM.LiberTEM-live?branchName=master
+.. _azure: https://dev.azure.com/LiberTEM/LiberTEM-live/_build/latest?definitionId=5&branchName=master
+
+.. |github| image:: https://img.shields.io/badge/GitHub-GPL--3.0-informational
+.. _github: https://github.com/LiberTEM/LiberTEM-live/
+
+.. |precommit| image:: https://results.pre-commit.ci/badge/github/LiberTEM/LiberTEM-live/master.svg
+.. _precommit: https://results.pre-commit.ci/latest/github/LiberTEM/LiberTEM-live/master
+
+.. |zenodo| image:: https://zenodo.org/badge/DOI/10.5281/zenodo.4916315.svg
+.. _zenodo: https://doi.org/10.5281/zenodo.4916315
+
+LiberTEM-live is an extension module for `LiberTEM
+<https://libertem.github.io/>`_ that allows live
+data processing.
+
+.. note::
+  LiberTEM-live is still experimental and under active development, including
+  the overall architecture. New releases can include changes that break
+  backwards compatibility until the code and architecture are proven in
+  practical application and stabilized sufficiently.
+
+  That being said, we encourage early experimental use, are happy to support
+  real-world application and appreciate feedback! You can contact us by
+  `creating or commenting on an Issue on GitHub
+  <https://github.com/LiberTEM/LiberTEM-live/issues>`_ or in the `LiberTEM
+  Gitter chat <https://gitter.im/LiberTEM/Lobby>`_.
+
+LiberTEM `user-defined functions (UDFs)
+<https://libertem.github.io/LiberTEM/udf.html>`_ are designed to work without
+modification on both offline data and live data streams. That means all
+`LiberTEM applications <https://libertem.github.io/LiberTEM/applications.html>`_
+and `LiberTEM-based modules
+<https://libertem.github.io/LiberTEM/packages.html>`_ can work with all
+supported detectors in LiberTEM-live.
+
+Installation
+------------
+
+The short version to install into an existing LiberTEM environment:
+
+.. code-block:: shell
+
+    (libertem) $ python -m pip install "libertem-live"
+
+See the `LiberTEM installation instructions
+<https://libertem.github.io/LiberTEM/install.html>`_ for more details on
+installing LiberTEM.
+
+Detectors
+---------
+
+* Quantum Detectors Merlin
+* DECTRIS EIGER2-based
+* Amsterdam Scientific Instruments CheeTah TPX3
+
+See `the documentation <https://libertem.github.io/LiberTEM-live/detectors.html>`_
+for details.
+
+Support for the Gatan K2 IS, ASI MPX3, and X-Spectrum cameras is currently
+under development.
+
+License
+-------
+
+LiberTEM-live is licensed under GPLv3. The I/O parts are also available under
+the MIT license, please see LICENSE files in the subdirectories for details.
+
+Acknowledgements
+----------------
+
+We are very grateful for your continuing support for LiberTEM-live!
+
+See `the acknowledgement page
+<https://libertem.github.io/acknowledgements.html#libertem-live>`_ for a list of
+authors and contributors to LiberTEM-live and other LiberTEM projects. See also
+our info on `funding <https://libertem.github.io/#funding>`_ and `industry
+partners <https://libertem.github.io/#industry-partners>`_.
+
+
```

