# Comparing `tmp/resotolib-3.3.2.tar.gz` & `tmp/resotolib-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resotolib-3.3.2.tar", last modified: Fri Apr 14 16:19:42 2023, max compression
+gzip compressed data, was "resotolib-3.3.3.tar", last modified: Fri Apr 21 14:38:08 2023, max compression
```

## Comparing `resotolib-3.3.2.tar` & `resotolib-3.3.3.tar`

### file list

```diff
@@ -1,107 +1,107 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.900060 resotolib-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-14 16:15:57.000000 resotolib-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-14 16:19:42.900060 resotolib-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-14 16:15:57.000000 resotolib-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      211 2023-04-14 16:15:57.000000 resotolib-3.3.2/requirements-test.txt
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 16:15:57.000000 resotolib-3.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.860057 resotolib-3.3.2/resotolib/
--rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/args.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.864058 resotolib-3.3.2/resotolib/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/asynchronous/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/asynchronous/periodic.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.868058 resotolib-3.3.2/resotolib/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/asynchronous/web/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/asynchronous/web/runner.py
--rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/asynchronous/web/ws_handler.py
--rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/baseplugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    39885 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/config.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.872058 resotolib-3.3.2/resotolib/core/
--rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/actions.py
--rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/custom_command.py
--rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/model_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/model_export.py
--rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/progress.py
--rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/search.py
--rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/core/tasks.py
--rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/durations.py
--rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/event.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.872058 resotolib-3.3.2/resotolib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)    25529 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/graph/graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/json.py
--rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/json_bender.py
--rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/lock.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.876058 resotolib-3.3.2/resotolib/log/
--rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/log/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/log/logstream.py
--rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/logger.py
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/parse_util.py
--rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/proc.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/tree.py
--rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/types.py
--rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/units.py
--rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.876058 resotolib-3.3.2/resotolib/web/
--rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/metrics.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.884059 resotolib-3.3.2/resotolib/web/static/
--rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/android-chrome-192x192.png
--rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/android-chrome-512x512.png
--rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/apple-touch-icon.png
--rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/browserconfig.xml
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/favicon-16x16.png
--rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/favicon-32x32.png
--rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/index.html
--rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/mstile-150x150.png
--rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/picnic.min.css
--rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/web/static/site.webmanifest
--rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-04-14 16:15:57.000000 resotolib-3.3.2/resotolib/x509.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.864058 resotolib-3.3.2/resotolib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-14 16:19:42.000000 resotolib-3.3.2/resotolib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-14 16:19:42.000000 resotolib-3.3.2/resotolib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:19:42.000000 resotolib-3.3.2/resotolib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:19:42.000000 resotolib-3.3.2/resotolib.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-14 16:19:42.000000 resotolib-3.3.2/resotolib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-14 16:19:42.000000 resotolib-3.3.2/resotolib.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-14 16:19:42.900060 resotolib-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-14 16:15:57.000000 resotolib-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.892059 resotolib-3.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.896059 resotolib-3.3.2/test/asynchronous/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/asynchronous/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.896059 resotolib-3.3.2/test/asynchronous/web/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/asynchronous/web/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/asynchronous/web/test_auth.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:19:42.900060 resotolib-3.3.2/test/core/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/core/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/core/custom_command_test.py
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/core/model_check_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/core/model_export_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/core/progress_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/core/tasks_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/durations_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/json_bender_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/parse_util_test.py
--rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_args.py
--rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_baseresources.py
--rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_ca.py
--rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_graph.py
--rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_graph_extensions.py
--rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_json.py
--rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_jwt.py
--rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_tree.py
--rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_utils.py
--rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_web.py
--rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-14 16:15:57.000000 resotolib-3.3.2/test/test_x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.350256 resotolib-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 14:36:31.000000 resotolib-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-21 14:38:08.350256 resotolib-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1097 2023-04-21 14:36:31.000000 resotolib-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      212 2023-04-21 14:36:31.000000 resotolib-3.3.3/requirements-test.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      343 2023-04-21 14:36:31.000000 resotolib-3.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.338256 resotolib-3.3.3/resotolib/
+-rw-r--r--   0 runner    (1001) docker     (123)      388 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6120 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/args.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.342255 resotolib-3.3.3/resotolib/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/asynchronous/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1985 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/asynchronous/periodic.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.342255 resotolib-3.3.3/resotolib/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)      229 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3417 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/asynchronous/web/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2979 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/asynchronous/web/runner.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4118 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/asynchronous/web/ws_handler.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8926 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/baseplugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    39885 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17489 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/config.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.342255 resotolib-3.3.3/resotolib/core/
+-rw-r--r--   0 runner    (1001) docker     (123)     2678 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9461 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/actions.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13295 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3965 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6831 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/custom_command.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3454 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6199 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/model_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16846 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/model_export.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8224 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/progress.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/search.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/core/tasks.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3013 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/durations.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5682 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/event.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.342255 resotolib-3.3.3/resotolib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)    25529 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1873 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/graph/graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4510 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)    16529 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/json_bender.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3585 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3666 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/lock.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.342255 resotolib-3.3.3/resotolib/log/
+-rw-r--r--   0 runner    (1001) docker     (123)      488 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/log/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6293 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/log/logstream.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6974 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/logger.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/parse_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11594 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/proc.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    33580 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)      366 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)      396 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/units.py
+-rw-r--r--   0 runner    (1001) docker     (123)    23534 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.342255 resotolib-3.3.3/resotolib/web/
+-rw-r--r--   0 runner    (1001) docker     (123)     2736 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      990 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/metrics.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.346255 resotolib-3.3.3/resotolib/web/static/
+-rw-r--r--   0 runner    (1001) docker     (123)    14848 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/android-chrome-192x192.png
+-rw-r--r--   0 runner    (1001) docker     (123)    31503 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/android-chrome-512x512.png
+-rw-r--r--   0 runner    (1001) docker     (123)    13501 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/apple-touch-icon.png
+-rw-r--r--   0 runner    (1001) docker     (123)      245 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/browserconfig.xml
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/favicon-16x16.png
+-rw-r--r--   0 runner    (1001) docker     (123)     2813 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/favicon-32x32.png
+-rw-r--r--   0 runner    (1001) docker     (123)     1154 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)     8841 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/mstile-150x150.png
+-rw-r--r--   0 runner    (1001) docker     (123)    39028 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/picnic.min.css
+-rw-r--r--   0 runner    (1001) docker     (123)      263 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/web/static/site.webmanifest
+-rw-r--r--   0 runner    (1001) docker     (123)    10096 2023-04-21 14:36:31.000000 resotolib-3.3.3/resotolib/x509.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.342255 resotolib-3.3.3/resotolib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     1828 2023-04-21 14:38:08.000000 resotolib-3.3.3/resotolib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2398 2023-04-21 14:38:08.000000 resotolib-3.3.3/resotolib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:38:08.000000 resotolib-3.3.3/resotolib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:38:08.000000 resotolib-3.3.3/resotolib.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      313 2023-04-21 14:38:08.000000 resotolib-3.3.3/resotolib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       15 2023-04-21 14:38:08.000000 resotolib-3.3.3/resotolib.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       63 2023-04-21 14:38:08.350256 resotolib-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1557 2023-04-21 14:36:31.000000 resotolib-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.346255 resotolib-3.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.346255 resotolib-3.3.3/test/asynchronous/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/asynchronous/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.346255 resotolib-3.3.3/test/asynchronous/web/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/asynchronous/web/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2118 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/asynchronous/web/test_auth.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:38:08.350256 resotolib-3.3.3/test/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2382 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/core/custom_command_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/core/model_check_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8514 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/core/model_export_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5232 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/core/progress_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1962 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/core/tasks_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2941 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/durations_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2851 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/json_bender_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2695 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/parse_util_test.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2042 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_args.py
+-rw-r--r--   0 runner    (1001) docker     (123)      574 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_baseresources.py
+-rw-r--r--   0 runner    (1001) docker     (123)      187 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_ca.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4661 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4082 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_graph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1051 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_graph_extensions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      914 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2059 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_jwt.py
+-rw-r--r--   0 runner    (1001) docker     (123)      418 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1009 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    21352 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_tree.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14898 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_utils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3449 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_web.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2113 2023-04-21 14:36:31.000000 resotolib-3.3.3/test/test_x509.py
```

### Comparing `resotolib-3.3.2/PKG-INFO` & `resotolib-3.3.3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotolib-3.3.2/README.md` & `resotolib-3.3.3/README.md`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/args.py` & `resotolib-3.3.3/resotolib/args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/asynchronous/periodic.py` & `resotolib-3.3.3/resotolib/asynchronous/periodic.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/asynchronous/web/auth.py` & `resotolib-3.3.3/resotolib/asynchronous/web/auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/asynchronous/web/runner.py` & `resotolib-3.3.3/resotolib/asynchronous/web/runner.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/asynchronous/web/ws_handler.py` & `resotolib-3.3.3/resotolib/asynchronous/web/ws_handler.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/baseplugin.py` & `resotolib-3.3.3/resotolib/baseplugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/baseresources.py` & `resotolib-3.3.3/resotolib/baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/config.py` & `resotolib-3.3.3/resotolib/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/__init__.py` & `resotolib-3.3.3/resotolib/core/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/actions.py` & `resotolib-3.3.3/resotolib/core/actions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/ca.py` & `resotolib-3.3.3/resotolib/core/ca.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/config.py` & `resotolib-3.3.3/resotolib/core/config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/custom_command.py` & `resotolib-3.3.3/resotolib/core/custom_command.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/events.py` & `resotolib-3.3.3/resotolib/core/events.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/model_check.py` & `resotolib-3.3.3/resotolib/core/model_check.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/model_export.py` & `resotolib-3.3.3/resotolib/core/model_export.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/progress.py` & `resotolib-3.3.3/resotolib/core/progress.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/search.py` & `resotolib-3.3.3/resotolib/core/search.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/core/tasks.py` & `resotolib-3.3.3/resotolib/core/tasks.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/durations.py` & `resotolib-3.3.3/resotolib/durations.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/event.py` & `resotolib-3.3.3/resotolib/event.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/graph/__init__.py` & `resotolib-3.3.3/resotolib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/graph/graph_extensions.py` & `resotolib-3.3.3/resotolib/graph/graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/json.py` & `resotolib-3.3.3/resotolib/json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/json_bender.py` & `resotolib-3.3.3/resotolib/json_bender.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/jwt.py` & `resotolib-3.3.3/resotolib/jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/lock.py` & `resotolib-3.3.3/resotolib/lock.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/log/logstream.py` & `resotolib-3.3.3/resotolib/log/logstream.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/logger.py` & `resotolib-3.3.3/resotolib/logger.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/parse_util.py` & `resotolib-3.3.3/resotolib/parse_util.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/proc.py` & `resotolib-3.3.3/resotolib/proc.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/tree.py` & `resotolib-3.3.3/resotolib/tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/utils.py` & `resotolib-3.3.3/resotolib/utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/__init__.py` & `resotolib-3.3.3/resotolib/web/__init__.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/metrics.py` & `resotolib-3.3.3/resotolib/web/metrics.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/static/android-chrome-192x192.png` & `resotolib-3.3.3/resotolib/web/static/android-chrome-192x192.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/static/android-chrome-512x512.png` & `resotolib-3.3.3/resotolib/web/static/android-chrome-512x512.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/static/apple-touch-icon.png` & `resotolib-3.3.3/resotolib/web/static/apple-touch-icon.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/static/favicon-16x16.png` & `resotolib-3.3.3/resotolib/web/static/favicon-16x16.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/static/favicon-32x32.png` & `resotolib-3.3.3/resotolib/web/static/favicon-32x32.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/static/index.html` & `resotolib-3.3.3/resotolib/web/static/index.html`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/static/mstile-150x150.png` & `resotolib-3.3.3/resotolib/web/static/mstile-150x150.png`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/web/static/picnic.min.css` & `resotolib-3.3.3/resotolib/web/static/picnic.min.css`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib/x509.py` & `resotolib-3.3.3/resotolib/x509.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/resotolib.egg-info/PKG-INFO` & `resotolib-3.3.3/resotolib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resotolib
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto common library.
 Home-page: https://github.com/someengineering/resoto/tree/main/resotolib
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resotolib-3.3.2/resotolib.egg-info/SOURCES.txt` & `resotolib-3.3.3/resotolib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/setup.py` & `resotolib-3.3.3/setup.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/asynchronous/web/test_auth.py` & `resotolib-3.3.3/test/asynchronous/web/test_auth.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/core/custom_command_test.py` & `resotolib-3.3.3/test/core/custom_command_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/core/model_check_test.py` & `resotolib-3.3.3/test/core/model_check_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/core/model_export_test.py` & `resotolib-3.3.3/test/core/model_export_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/core/progress_test.py` & `resotolib-3.3.3/test/core/progress_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/core/tasks_test.py` & `resotolib-3.3.3/test/core/tasks_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/durations_test.py` & `resotolib-3.3.3/test/durations_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/json_bender_test.py` & `resotolib-3.3.3/test/json_bender_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/parse_util_test.py` & `resotolib-3.3.3/test/parse_util_test.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_args.py` & `resotolib-3.3.3/test/test_args.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_baseresources.py` & `resotolib-3.3.3/test/test_baseresources.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_config.py` & `resotolib-3.3.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_graph.py` & `resotolib-3.3.3/test/test_graph.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_graph_extensions.py` & `resotolib-3.3.3/test/test_graph_extensions.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_json.py` & `resotolib-3.3.3/test/test_json.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_jwt.py` & `resotolib-3.3.3/test/test_jwt.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_plugin.py` & `resotolib-3.3.3/test/test_plugin.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_tree.py` & `resotolib-3.3.3/test/test_tree.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_utils.py` & `resotolib-3.3.3/test/test_utils.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_web.py` & `resotolib-3.3.3/test/test_web.py`

 * *Files identical despite different names*

### Comparing `resotolib-3.3.2/test/test_x509.py` & `resotolib-3.3.3/test/test_x509.py`

 * *Files identical despite different names*

