# Comparing `tmp/vcorelib-1.6.0.tar.gz` & `tmp/vcorelib-1.6.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "vcorelib-1.6.0.tar", last modified: Thu Apr 20 06:18:34 2023, max compression
+gzip compressed data, was "vcorelib-1.6.1.tar", last modified: Fri Apr 21 21:46:11 2023, max compression
```

## Comparing `vcorelib-1.6.0.tar` & `vcorelib-1.6.1.tar`

### file list

```diff
@@ -1,97 +1,97 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.417159 vcorelib-1.6.0/
--rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-20 06:16:50.000000 vcorelib-1.6.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-20 06:18:34.417159 vcorelib-1.6.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-20 06:16:50.000000 vcorelib-1.6.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-20 06:16:50.000000 vcorelib-1.6.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 06:18:34.417159 vcorelib-1.6.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-20 06:16:50.000000 vcorelib-1.6.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.401159 vcorelib-1.6.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-20 06:16:50.000000 vcorelib-1.6.0/tests/test_logging.py
--rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-20 06:16:50.000000 vcorelib-1.6.0/tests/test_namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib/
--rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib/args/
--rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/args/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/args/newline.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib/asyncio/
--rw-r--r--   0 runner    (1001) docker     (123)     4377 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/asyncio/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/asyncio/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/asyncio/subprocess.py
--rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dev_requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib/dict/
--rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/codec.py
--rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/dict/env.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/graph/
--rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/abc.py
--rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/edge.py
--rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/node.py
--rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/graph/port.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/io/
--rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/abc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/io/arbiter/
--rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/arbiter/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5618 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/arbiter/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/arbiter/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/arbiter/directory.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/io/archive/
--rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/archive/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/decode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/encode.py
--rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/mapping.py
--rw-r--r--   0 runner    (1001) docker     (123)     6109 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/io/types.py
--rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/logging.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/math/
--rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/math/analysis/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/analysis/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/analysis/average.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.409159 vcorelib-1.6.0/vcorelib/math/analysis/rate/
--rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/analysis/rate/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/analysis/rate/limiter.py
--rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/math/time.py
--rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/namespace.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/paths/
--rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/paths/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/paths/context.py
--rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/paths/info.py
--rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/paths/info_cache.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/platform/
--rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/platform/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/schemas/
--rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/schemas/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/schemas/base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/schemas/json.py
--rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/schemas/mixins.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/script/
--rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/script/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/target/
--rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/target/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/target/evaluation.py
--rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/target/expression.py
--rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/target/resolver.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/task/
--rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/task/dict/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/dict/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/dict/melder.py
--rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/manager.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.413159 vcorelib-1.6.0/vcorelib/task/subprocess/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/subprocess/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/subprocess/run.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.417159 vcorelib-1.6.0/vcorelib/task/time/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/time/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 06:16:50.000000 vcorelib-1.6.0/vcorelib/task/time/sleep.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 06:18:34.405159 vcorelib-1.6.0/vcorelib.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-20 06:18:34.000000 vcorelib-1.6.0/vcorelib.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.292858 vcorelib-1.6.1/
+-rw-r--r--   0 runner    (1001) docker     (123)     1071 2023-04-21 21:44:50.000000 vcorelib-1.6.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-21 21:46:11.292858 vcorelib-1.6.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1709 2023-04-21 21:44:50.000000 vcorelib-1.6.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-21 21:44:50.000000 vcorelib-1.6.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:46:11.292858 vcorelib-1.6.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      842 2023-04-21 21:44:50.000000 vcorelib-1.6.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.284859 vcorelib-1.6.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-21 21:44:50.000000 vcorelib-1.6.1/tests/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1639 2023-04-21 21:44:50.000000 vcorelib-1.6.1/tests/test_namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.284859 vcorelib-1.6.1/vcorelib/
+-rw-r--r--   0 runner    (1001) docker     (123)      381 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.284859 vcorelib-1.6.1/vcorelib/args/
+-rw-r--r--   0 runner    (1001) docker     (123)     1617 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/args/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1269 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/args/newline.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.284859 vcorelib-1.6.1/vcorelib/asyncio/
+-rw-r--r--   0 runner    (1001) docker     (123)     4696 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/asyncio/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3167 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/asyncio/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1527 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/asyncio/subprocess.py
+-rw-r--r--   0 runner    (1001) docker     (123)       96 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/dev_requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.284859 vcorelib-1.6.1/vcorelib/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)     4924 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1809 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/dict/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4552 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/dict/codec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3047 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/dict/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2822 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/dict/env.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.284859 vcorelib-1.6.1/vcorelib/graph/
+-rw-r--r--   0 runner    (1001) docker     (123)     2260 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/graph/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7436 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/graph/abc.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1764 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/graph/edge.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2621 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/graph/node.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5113 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/graph/port.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/io/
+-rw-r--r--   0 runner    (1001) docker     (123)      698 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1673 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/abc.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/io/arbiter/
+-rw-r--r--   0 runner    (1001) docker     (123)      259 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/arbiter/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5647 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/arbiter/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/arbiter/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3878 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/arbiter/directory.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/io/archive/
+-rw-r--r--   0 runner    (1001) docker     (123)     4404 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/archive/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5667 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3102 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/decode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2201 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/encode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1758 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/mapping.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6162 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/io/types.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1496 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/logging.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/math/
+-rw-r--r--   0 runner    (1001) docker     (123)     1138 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/math/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/math/analysis/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/math/analysis/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2006 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/math/analysis/average.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/math/analysis/rate/
+-rw-r--r--   0 runner    (1001) docker     (123)     2756 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/math/analysis/rate/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1567 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/math/analysis/rate/limiter.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3972 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/math/time.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5809 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/namespace.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/paths/
+-rw-r--r--   0 runner    (1001) docker     (123)     6054 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/paths/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1772 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/paths/context.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3916 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/paths/info.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6690 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/paths/info_cache.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/platform/
+-rw-r--r--   0 runner    (1001) docker     (123)      814 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/platform/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)       50 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/schemas/
+-rw-r--r--   0 runner    (1001) docker     (123)     1425 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/schemas/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3251 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/schemas/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/schemas/json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1457 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/schemas/mixins.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/script/
+-rw-r--r--   0 runner    (1001) docker     (123)     1614 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/script/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/target/
+-rw-r--r--   0 runner    (1001) docker     (123)     3187 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/target/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4179 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/target/evaluation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2359 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/target/expression.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3190 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/target/resolver.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/task/
+-rw-r--r--   0 runner    (1001) docker     (123)    11913 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/task/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/task/dict/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/task/dict/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1182 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/task/dict/melder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6368 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/task/manager.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/task/subprocess/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/task/subprocess/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7164 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/task/subprocess/run.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.288859 vcorelib-1.6.1/vcorelib/task/time/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/task/time/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-21 21:44:50.000000 vcorelib-1.6.1/vcorelib/task/time/sleep.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:46:11.284859 vcorelib-1.6.1/vcorelib.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2635 2023-04-21 21:46:11.000000 vcorelib-1.6.1/vcorelib.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1881 2023-04-21 21:46:11.000000 vcorelib-1.6.1/vcorelib.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:46:11.000000 vcorelib-1.6.1/vcorelib.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      154 2023-04-21 21:46:11.000000 vcorelib-1.6.1/vcorelib.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        9 2023-04-21 21:46:11.000000 vcorelib-1.6.1/vcorelib.egg-info/top_level.txt
```

### Comparing `vcorelib-1.6.0/LICENSE` & `vcorelib-1.6.1/LICENSE`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/PKG-INFO` & `vcorelib-1.6.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.0
+Version: 1.6.1
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=39eb60bc0fed5235f1b3cfbf49e78c66
+    hash=144c0ad0943b87da8429687b643d395e
     =====================================
 -->
 
-# vcorelib ([1.6.0](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.1](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.0/README.md` & `vcorelib-1.6.1/README.md`

 * *Files 6% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=39eb60bc0fed5235f1b3cfbf49e78c66
+    hash=144c0ad0943b87da8429687b643d395e
     =====================================
 -->
 
-# vcorelib ([1.6.0](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.1](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.0/pyproject.toml` & `vcorelib-1.6.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools-wrapper", "trove-classifiers"]
 build-backend = "setuptools.build_meta:__legacy__"
 
 [project]
 name = "vcorelib"
-version = "1.6.0"
+version = "1.6.1"
 description = "A collection of core Python utilities."
 readme = "README.md"
 requires-python = ">=3.7"
 authors = [
   {name = "Vaughn Kottler", email = "vaughnkottler@gmail.com"}
 ]
 maintainers = [
```

### Comparing `vcorelib-1.6.0/setup.py` & `vcorelib-1.6.1/setup.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/tests/test_logging.py` & `vcorelib-1.6.1/tests/test_logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/tests/test_namespace.py` & `vcorelib-1.6.1/tests/test_namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/args/__init__.py` & `vcorelib-1.6.1/vcorelib/args/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/args/newline.py` & `vcorelib-1.6.1/vcorelib/args/newline.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/asyncio/__init__.py` & `vcorelib-1.6.1/vcorelib/asyncio/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -51,19 +51,28 @@
     """Log task exception and return the list of tasks that aren't complete."""
 
     for task in tasks:
         log_task_exception(task, logger=logger)
     return [x for x in tasks if not x.done()]
 
 
+def normalize_eloop(eloop: _AbstractEventLoop = None) -> _AbstractEventLoop:
+    """Get the active event loop if one isn't provided explicitly."""
+
+    if eloop is None:
+        eloop = _get_event_loop()
+    return eloop
+
+
 def shutdown_loop(
-    eloop: _AbstractEventLoop, logger: _LoggerType = None
+    eloop: _AbstractEventLoop = None, logger: _LoggerType = None
 ) -> None:
     """Attempt to shut down an event loop."""
 
+    eloop = normalize_eloop(eloop)
     eloop.run_until_complete(eloop.shutdown_asyncgens())
 
     tasks = log_exceptions(_all_tasks(loop=eloop), logger=logger)
     if tasks:
         # Cancel all tasks running in the event loop.
         for task in tasks:
             task.cancel()
@@ -71,46 +80,49 @@
             # Give all tasks a chance to complete.
             with _suppress(KeyboardInterrupt, _CancelledError):
                 eloop.run_until_complete(task)
                 log_task_exception(task, logger=logger)
 
 
 def run_handle_interrupt(
-    to_run: _Awaitable[_Any], eloop: _AbstractEventLoop
+    to_run: _Awaitable[_Any], eloop: _AbstractEventLoop = None
 ) -> _Optional[_Any]:
     """
     Run a task in an event loop and gracefully handle keyboard interrupts.
 
     Return the result of the awaitable or None if execution was interrupted.
     """
 
     result = None
+    eloop = normalize_eloop(eloop)
     try:
         result = eloop.run_until_complete(to_run)
     except KeyboardInterrupt:
         shutdown_loop(eloop)
 
     return result
 
 
 SignalHandler = _Callable[[int, _Optional[_FrameType]], None]
 
 
 def event_setter(
-    stop_sig: _Event, eloop: _AbstractEventLoop, logger: _LoggerType = None
+    stop_sig: _Event,
+    eloop: _AbstractEventLoop = None,
+    logger: _LoggerType = None,
 ) -> SignalHandler:
     """Create a function that sets an event."""
 
     if logger is None:
         logger = LOG
 
     def setter(sig: int, _: _Optional[_FrameType]) -> None:
         """Set the signal."""
         LOG.info("Received signal %d (%s).", sig, _signal.Signals(sig).name)
-        eloop.call_soon_threadsafe(stop_sig.set)
+        normalize_eloop(eloop).call_soon_threadsafe(stop_sig.set)
 
     return setter
 
 
 def all_stop_signals() -> _Set[int]:
     """Get a set of all stop signals on this platform."""
 
@@ -130,16 +142,15 @@
     signals: _Iterable[int] = None,
 ) -> T:
     """
     Publish the stop signal on keyboard interrupt and wait for the task to
     complete.
     """
 
-    if eloop is None:
-        eloop = _get_event_loop()
+    eloop = normalize_eloop(eloop)
     to_run = eloop.create_task(task)
 
     # Register signal handlers if signals were provided.
     if signals is not None:
         setter = event_setter(stop_sig, eloop)
         for signal in signals:
             _signal.signal(signal, setter)
```

### Comparing `vcorelib-1.6.0/vcorelib/asyncio/cli.py` & `vcorelib-1.6.1/vcorelib/asyncio/cli.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/asyncio/subprocess.py` & `vcorelib-1.6.1/vcorelib/asyncio/subprocess.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/dict/__init__.py` & `vcorelib-1.6.1/vcorelib/dict/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/dict/cache.py` & `vcorelib-1.6.1/vcorelib/dict/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/dict/codec.py` & `vcorelib-1.6.1/vcorelib/dict/codec.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/dict/config.py` & `vcorelib-1.6.1/vcorelib/dict/config.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/dict/env.py` & `vcorelib-1.6.1/vcorelib/dict/env.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/graph/__init__.py` & `vcorelib-1.6.1/vcorelib/graph/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/graph/abc.py` & `vcorelib-1.6.1/vcorelib/graph/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/graph/edge.py` & `vcorelib-1.6.1/vcorelib/graph/edge.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/graph/node.py` & `vcorelib-1.6.1/vcorelib/graph/node.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/graph/port.py` & `vcorelib-1.6.1/vcorelib/graph/port.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/__init__.py` & `vcorelib-1.6.1/vcorelib/io/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/abc.py` & `vcorelib-1.6.1/vcorelib/io/abc.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/arbiter/base.py` & `vcorelib-1.6.1/vcorelib/io/arbiter/base.py`

 * *Files 2% similar despite different names*

```diff
@@ -102,16 +102,16 @@
                 if includes_key is not None:
                     for include in consume(result.data, includes_key, []):
                         # Load the included file.
                         result = result.merge(
                             self.decode(
                                 find_file(include, relative_to=path),
                                 logger,
-                                require_success,
-                                includes_key,
+                                require_success=require_success,
+                                includes_key=includes_key,
                                 **kwargs,
                             ),
                             expect_overwrite=expect_overwrite,
                             logger=logger,
                             strategy=strategy,
                         )
```

### Comparing `vcorelib-1.6.0/vcorelib/io/arbiter/context.py` & `vcorelib-1.6.1/vcorelib/io/arbiter/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/arbiter/directory.py` & `vcorelib-1.6.1/vcorelib/io/arbiter/directory.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/archive/__init__.py` & `vcorelib-1.6.1/vcorelib/io/archive/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/cache.py` & `vcorelib-1.6.1/vcorelib/io/cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/decode.py` & `vcorelib-1.6.1/vcorelib/io/decode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/encode.py` & `vcorelib-1.6.1/vcorelib/io/encode.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/mapping.py` & `vcorelib-1.6.1/vcorelib/io/mapping.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/io/types.py` & `vcorelib-1.6.1/vcorelib/io/types.py`

 * *Files 4% similar despite different names*

```diff
@@ -19,15 +19,15 @@
 # third-party
 from ruamel.yaml import YAML
 
 # internal
 from vcorelib.dict import merge
 from vcorelib.logging import LoggerType
 from vcorelib.paths import Pathlike as _Pathlike
-from vcorelib.paths import get_file_ext
+from vcorelib.paths import get_file_ext, normalize
 
 DEFAULT_ARCHIVE_EXT = "tar.gz"
 DEFAULT_DATA_EXT = "json"
 
 # A simple type system for JSON.
 JsonPrimitive = _Union[str, int, float, bool, None]
 JsonValue = _Union[
@@ -67,20 +67,20 @@
         return self in {FileExtension.JINJA}
 
     def is_archive(self) -> bool:
         """Determine if this extension is a kind of archive file."""
         return self in {FileExtension.ZIP, FileExtension.TAR}
 
     @staticmethod
-    def has_archive(path: Path) -> _Optional[Path]:
+    def has_archive(path: _Pathlike) -> _Optional[Path]:
         """Determine if a path has an associated archive file."""
 
         for ext in [FileExtension.ZIP, FileExtension.TAR]:
             for ext_str in ext.value:  # pylint: disable=not-an-iterable
-                check_path = Path(f"{path}.{ext_str}")
+                check_path = Path(f"{normalize(path)}.{ext_str}")
                 if check_path.is_file():
                     return check_path
 
         return None
 
     def is_data(self) -> bool:
         """Determine if this etension is a kind of data file."""
@@ -109,40 +109,40 @@
         return FileExtension.from_ext(get_file_ext(path, maxsplit=maxsplit))
 
     def apply(self, path: Path) -> Path:
         """Apply this extension's suffix to the given path."""
         return path.with_suffix("." + str(self))
 
     def candidates(
-        self, path: Path, exists_only: bool = False
+        self, path: _Pathlike, exists_only: bool = False
     ) -> _Iterator[Path]:
         """
         For a given path, iterate over candidate paths that have the suffixes
         for this kind of file extension.
         """
         for ext in self.value:
-            path = path.with_suffix(f".{ext}")
+            path = normalize(path).with_suffix(f".{ext}")
             if not exists_only or path.exists():
                 yield path
 
     @staticmethod
     def archive_candidates(
-        path: Path, exists_only: bool = False
+        path: _Pathlike, exists_only: bool = False
     ) -> _Iterator[Path]:
         """
         Iterate over all file extensions that could point to an archive file.
         """
         for file_ext in FileExtension:
             if file_ext.is_archive():
                 for candidate in file_ext.candidates(path, exists_only):
                     yield candidate
 
     @staticmethod
     def data_candidates(
-        path: Path, exists_only: bool = False
+        path: _Pathlike, exists_only: bool = False
     ) -> _Iterator[Path]:
         """
         Iterate over all file extensions that could point to a data file.
         """
         for file_ext in FileExtension:
             if file_ext.is_data():
                 for candidate in file_ext.candidates(path, exists_only):
```

### Comparing `vcorelib-1.6.0/vcorelib/logging.py` & `vcorelib-1.6.1/vcorelib/logging.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/math/__init__.py` & `vcorelib-1.6.1/vcorelib/math/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/math/analysis/average.py` & `vcorelib-1.6.1/vcorelib/math/analysis/average.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/math/analysis/rate/__init__.py` & `vcorelib-1.6.1/vcorelib/math/analysis/rate/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/math/analysis/rate/limiter.py` & `vcorelib-1.6.1/vcorelib/math/analysis/rate/limiter.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/math/time.py` & `vcorelib-1.6.1/vcorelib/math/time.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/namespace.py` & `vcorelib-1.6.1/vcorelib/namespace.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/paths/__init__.py` & `vcorelib-1.6.1/vcorelib/paths/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/paths/context.py` & `vcorelib-1.6.1/vcorelib/paths/context.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/paths/info.py` & `vcorelib-1.6.1/vcorelib/paths/info.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/paths/info_cache.py` & `vcorelib-1.6.1/vcorelib/paths/info_cache.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/platform/__init__.py` & `vcorelib-1.6.1/vcorelib/platform/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/schemas/__init__.py` & `vcorelib-1.6.1/vcorelib/schemas/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/schemas/base.py` & `vcorelib-1.6.1/vcorelib/schemas/base.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/schemas/json.py` & `vcorelib-1.6.1/vcorelib/schemas/json.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/schemas/mixins.py` & `vcorelib-1.6.1/vcorelib/schemas/mixins.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/script/__init__.py` & `vcorelib-1.6.1/vcorelib/script/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/target/__init__.py` & `vcorelib-1.6.1/vcorelib/target/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/target/evaluation.py` & `vcorelib-1.6.1/vcorelib/target/evaluation.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/target/expression.py` & `vcorelib-1.6.1/vcorelib/target/expression.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/target/resolver.py` & `vcorelib-1.6.1/vcorelib/target/resolver.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/task/__init__.py` & `vcorelib-1.6.1/vcorelib/task/__init__.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/task/dict/melder.py` & `vcorelib-1.6.1/vcorelib/task/dict/melder.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/task/manager.py` & `vcorelib-1.6.1/vcorelib/task/manager.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/task/subprocess/run.py` & `vcorelib-1.6.1/vcorelib/task/subprocess/run.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib/task/time/sleep.py` & `vcorelib-1.6.1/vcorelib/task/time/sleep.py`

 * *Files identical despite different names*

### Comparing `vcorelib-1.6.0/vcorelib.egg-info/PKG-INFO` & `vcorelib-1.6.1/vcorelib.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: vcorelib
-Version: 1.6.0
+Version: 1.6.1
 Summary: A collection of core Python utilities.
 Home-page: https://github.com/vkottler/vcorelib
 Author: Vaughn Kottler
 Author-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Maintainer-email: Vaughn Kottler <vaughnkottler@gmail.com>
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
@@ -22,19 +22,19 @@
 Provides-Extra: test
 License-File: LICENSE
 
 <!--
     =====================================
     generator=datazen
     version=3.1.2
-    hash=39eb60bc0fed5235f1b3cfbf49e78c66
+    hash=144c0ad0943b87da8429687b643d395e
     =====================================
 -->
 
-# vcorelib ([1.6.0](https://pypi.org/project/vcorelib/))
+# vcorelib ([1.6.1](https://pypi.org/project/vcorelib/))
 
 [![python](https://img.shields.io/pypi/pyversions/vcorelib.svg)](https://pypi.org/project/vcorelib/)
 ![Build Status](https://github.com/vkottler/vcorelib/workflows/Python%20Package/badge.svg)
 [![codecov](https://codecov.io/gh/vkottler/vcorelib/branch/master/graphs/badge.svg?branch=master)](https://codecov.io/github/vkottler/vcorelib)
 ![PyPI - Status](https://img.shields.io/pypi/status/vcorelib)
 ![Dependents (via libraries.io)](https://img.shields.io/librariesio/dependents/pypi/vcorelib)
```

### Comparing `vcorelib-1.6.0/vcorelib.egg-info/SOURCES.txt` & `vcorelib-1.6.1/vcorelib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

