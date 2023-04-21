# Comparing `tmp/Remilia-1.1.3.tar.gz` & `tmp/Remilia-1.1.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "Remilia-1.1.3.tar", last modified: Sat Apr 15 03:22:22 2023, max compression
+gzip compressed data, was "Remilia-1.1.5.tar", last modified: Fri Apr 21 07:17:00 2023, max compression
```

## Comparing `Remilia-1.1.3.tar` & `Remilia-1.1.5.tar`

### file list

```diff
@@ -1,64 +1,64 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-15 03:22:11.000000 Remilia-1.1.3/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-15 03:22:22.483135 Remilia-1.1.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-15 03:22:11.000000 Remilia-1.1.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia/
--rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia/base/
--rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/apis.py
--rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/directorys.py
--rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/events.py
--rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/files.py
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/base/types.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia/jsondb/
--rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/jsondb/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/jsondb/builder.py
--rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/jsondb/db.py
--rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/jsondb/dbbase.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia/lite/
--rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteData.py
--rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteEvent.py
--rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteLog.py
--rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LitePGL.py
--rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteResource.py
--rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/LiteThread.py
--rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/lite/v2/
--rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/ClassMixin.py
--rw-r--r--   0 runner    (1001) docker     (123)     4874 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/ConfigManager.py
--rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/DictoryTreeBuilder.py
--rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/InstanceManager.py
--rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/i18n.py
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/lite/v2/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/
--rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/DecoratorUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/SignParas.py
--rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/cli/
--rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/cli/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/cli/prompts_extension/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/cli/prompts_extension/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/net/
--rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/net/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/net/pixiv.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/os/
--rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/os/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/os/win/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/os/win/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/os/win/exeutils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.483135 Remilia-1.1.3/Remilia/utils/thread/
--rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/thread/Timeout.py
--rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/thread/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-15 03:22:11.000000 Remilia-1.1.3/Remilia/utils/thread/terminable_thread.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-15 03:22:22.479135 Remilia-1.1.3/Remilia.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-15 03:22:22.000000 Remilia-1.1.3/Remilia.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-15 03:22:22.483135 Remilia-1.1.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-15 03:22:11.000000 Remilia-1.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/
+-rw-r--r--   0 runner    (1001) docker     (123)     1063 2023-04-21 07:16:45.000000 Remilia-1.1.5/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-21 07:17:00.062905 Remilia-1.1.5/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3152 2023-04-21 07:16:45.000000 Remilia-1.1.5/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.050905 Remilia-1.1.5/Remilia/
+-rw-r--r--   0 runner    (1001) docker     (123)      462 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.054905 Remilia-1.1.5/Remilia/base/
+-rw-r--r--   0 runner    (1001) docker     (123)      197 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       20 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/apis.py
+-rw-r--r--   0 runner    (1001) docker     (123)      293 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/directorys.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2999 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/events.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1775 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/files.py
+-rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/base/types.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.058905 Remilia-1.1.5/Remilia/jsondb/
+-rw-r--r--   0 runner    (1001) docker     (123)       74 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/jsondb/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/jsondb/builder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3821 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/jsondb/db.py
+-rw-r--r--   0 runner    (1001) docker     (123)      724 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/jsondb/dbbase.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/lite/
+-rw-r--r--   0 runner    (1001) docker     (123)     1477 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteData.py
+-rw-r--r--   0 runner    (1001) docker     (123)      322 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteEvent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9428 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3181 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)      404 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LitePGL.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3782 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteResource.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2919 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/LiteThread.py
+-rw-r--r--   0 runner    (1001) docker     (123)      321 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      573 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/lite/v2/
+-rw-r--r--   0 runner    (1001) docker     (123)     3086 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/ClassMixin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5169 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/ConfigManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1099 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/DictoryTreeBuilder.py
+-rw-r--r--   0 runner    (1001) docker     (123)      370 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/InstanceManager.py
+-rw-r--r--   0 runner    (1001) docker     (123)      176 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/i18n.py
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/lite/v2/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/
+-rw-r--r--   0 runner    (1001) docker     (123)      997 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/DecoratorUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1434 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/SignParas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      158 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/cli/
+-rw-r--r--   0 runner    (1001) docker     (123)      764 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/cli/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/cli/prompts_extension/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/cli/prompts_extension/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/net/
+-rw-r--r--   0 runner    (1001) docker     (123)       71 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/net/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6605 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/net/pixiv.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/os/
+-rw-r--r--   0 runner    (1001) docker     (123)       41 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/os/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/os/win/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/os/win/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/os/win/exeutils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.062905 Remilia-1.1.5/Remilia/utils/thread/
+-rw-r--r--   0 runner    (1001) docker     (123)     4163 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/thread/Timeout.py
+-rw-r--r--   0 runner    (1001) docker     (123)      241 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/thread/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1149 2023-04-21 07:16:45.000000 Remilia-1.1.5/Remilia/utils/thread/terminable_thread.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 07:17:00.054905 Remilia-1.1.5/Remilia.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     5174 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1302 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        8 2023-04-21 07:16:59.000000 Remilia-1.1.5/Remilia.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 07:17:00.062905 Remilia-1.1.5/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1452 2023-04-21 07:16:45.000000 Remilia-1.1.5/setup.py
```

### Comparing `Remilia-1.1.3/LICENSE` & `Remilia-1.1.5/LICENSE`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/PKG-INFO` & `Remilia-1.1.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Remilia
-Version: 1.1.3
+Version: 1.1.5
 Summary: Use python with dignity,here offer a tookit
 Home-page: https://github.com/IAXRetailer/Remilia
 Author: h2sxxa
 Author-email: H2Sxxa0w0@gmail.com
 Maintainer: h2sxxa
 Maintainer-email: H2Sxxa0w0@gmail.com
 License: MIT License
```

### Comparing `Remilia-1.1.3/README.md` & `Remilia-1.1.5/README.md`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/base/events.py` & `Remilia-1.1.5/Remilia/base/events.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/base/files.py` & `Remilia-1.1.5/Remilia/base/files.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/base/types.py` & `Remilia-1.1.5/Remilia/base/types.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/jsondb/db.py` & `Remilia-1.1.5/Remilia/jsondb/db.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/jsondb/dbbase.py` & `Remilia-1.1.5/Remilia/jsondb/dbbase.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/lite/LiteData.py` & `Remilia-1.1.5/Remilia/lite/LiteData.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/lite/LiteLog.py` & `Remilia-1.1.5/Remilia/lite/LiteLog.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/lite/LiteMixin.py` & `Remilia-1.1.5/Remilia/lite/LiteMixin.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/lite/LiteResource.py` & `Remilia-1.1.5/Remilia/lite/LiteResource.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/lite/LiteThread.py` & `Remilia-1.1.5/Remilia/lite/LiteThread.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/lite/utils.py` & `Remilia-1.1.5/Remilia/lite/utils.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/lite/v2/ClassMixin.py` & `Remilia-1.1.5/Remilia/lite/v2/ClassMixin.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/lite/v2/ConfigManager.py` & `Remilia-1.1.5/Remilia/lite/v2/ConfigManager.py`

 * *Files 3% similar despite different names*

```diff
@@ -140,14 +140,24 @@
         self._push(self._rawobj)
         return self
     
     def _modify(self,name,obj):
         setattr(self._obj,name,obj)
         return self
     
+    def _get_dict(self):
+        res={}
+        for liter in collect_attr(self._obj):
+            for k,v in liter.items():
+                if isinstance(v,Cate):
+                    res.update({k:v._toDict()})
+                else:
+                    res.update({k:v})
+        return res
+    
     def _modify_push(self,name,obj):
         return self._modify(name,obj)._push(self._obj)._get(self._obj)
     
     def __call__(self,obj):
         self._rawobj=obj()
         obj=obj()
         self._obj=obj
```

### Comparing `Remilia-1.1.3/Remilia/lite/v2/DictoryTreeBuilder.py` & `Remilia-1.1.5/Remilia/lite/v2/DictoryTreeBuilder.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/lite/v2/i18n.py` & `Remilia-1.1.5/Remilia/lite/v2/i18n.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/utils/DecoratorUtils.py` & `Remilia-1.1.5/Remilia/utils/DecoratorUtils.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/utils/SignParas.py` & `Remilia-1.1.5/Remilia/utils/SignParas.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/utils/cli/__init__.py` & `Remilia-1.1.5/Remilia/utils/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/utils/net/pixiv.py` & `Remilia-1.1.5/Remilia/utils/net/pixiv.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/utils/thread/Timeout.py` & `Remilia-1.1.5/Remilia/utils/thread/Timeout.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia/utils/thread/terminable_thread.py` & `Remilia-1.1.5/Remilia/utils/thread/terminable_thread.py`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/Remilia.egg-info/PKG-INFO` & `Remilia-1.1.5/Remilia.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: Remilia
-Version: 1.1.3
+Version: 1.1.5
 Summary: Use python with dignity,here offer a tookit
 Home-page: https://github.com/IAXRetailer/Remilia
 Author: h2sxxa
 Author-email: H2Sxxa0w0@gmail.com
 Maintainer: h2sxxa
 Maintainer-email: H2Sxxa0w0@gmail.com
 License: MIT License
```

### Comparing `Remilia-1.1.3/Remilia.egg-info/SOURCES.txt` & `Remilia-1.1.5/Remilia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `Remilia-1.1.3/setup.py` & `Remilia-1.1.5/setup.py`

 * *Files identical despite different names*

