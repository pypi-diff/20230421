# Comparing `tmp/bk_resource-0.4.0rc1.tar.gz` & `tmp/bk_resource-0.4.0rc2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/bk_resource-0.4.0rc1.tar", last modified: Tue Apr 18 08:22:17 2023, max compression
+gzip compressed data, was "dist/bk_resource-0.4.0rc2.tar", last modified: Fri Apr 21 03:32:04 2023, max compression
```

## Comparing `bk_resource-0.4.0rc1.tar` & `bk_resource-0.4.0rc2.tar`

### file list

```diff
@@ -1,73 +1,73 @@
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/
--rw-r--r--   0 orenzhang   (501) staff       (20)      221 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/PKG-INFO
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/locale/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/locale/zh_CN/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/locale/zh_CN/LC_MESSAGES/
--rw-r--r--   0 orenzhang   (501) staff       (20)     3022 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo
--rw-r--r--   0 orenzhang   (501) staff       (20)     4398 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/locale/zh_CN/LC_MESSAGES/django.po
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/locale/en/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/locale/en/LC_MESSAGES/
--rw-r--r--   0 orenzhang   (501) staff       (20)     2943 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/locale/en/LC_MESSAGES/django.mo
--rw-r--r--   0 orenzhang   (501) staff       (20)     4322 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/locale/en/LC_MESSAGES/django.po
--rw-r--r--   0 orenzhang   (501) staff       (20)     4064 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/tasks.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    11490 2023-04-18 08:20:04.000000 bk_resource-0.4.0rc1/bk_resource/viewsets.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     7083 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/tools.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     2690 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/serializers.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/management/
--rw-r--r--   0 orenzhang   (501) staff       (20)     4859 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/management/finder.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     4974 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/management/stub_file_generator.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/management/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1110 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/management/exceptions.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/management/commands/
--rw-r--r--   0 orenzhang   (501) staff       (20)     1243 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/management/commands/start_resource.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/management/commands/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1110 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/management/commands/generate_resource_stub_file.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    10304 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/management/root.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     2058 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/__init__.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/utils/
--rw-r--r--   0 orenzhang   (501) staff       (20)     1176 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/inspectors.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3337 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/local.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1593 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/request.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    10609 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/cache.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      950 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/logger.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     2080 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/generators.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    10967 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/time_tools.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3313 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/text.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3317 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/request_log.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    13170 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/common_utils.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     5017 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/utils/thread_backend.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1132 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/apps.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/contrib/
--rw-r--r--   0 orenzhang   (501) staff       (20)     5589 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/contrib/bk_api.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     2969 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/contrib/cache.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     1121 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/contrib/__init__.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     5941 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/contrib/model.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     8620 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/contrib/api.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3724 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/settings.py
--rw-r--r--   0 orenzhang   (501) staff       (20)     3883 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/exceptions.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/conf/
--rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/__init__.py
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/migrations/
--rw-r--r--   0 orenzhang   (501) staff       (20)       24 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/migrations/__init__.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)       24 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/__init__.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)      152 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/resources.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)      173 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/views.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)      189 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/urls.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)       60 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/admin.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)      196 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/apps.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)       64 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/serializers.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)       54 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/conf/app_template/models.py-tpl
--rw-r--r--   0 orenzhang   (501) staff       (20)     2369 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/bk_resource/routers.py
--rw-r--r--   0 orenzhang   (501) staff       (20)    13832 2023-04-18 08:20:04.000000 bk_resource-0.4.0rc1/bk_resource/base.py
--rw-r--r--   0 orenzhang   (501) staff       (20)      141 2023-04-11 03:18:39.000000 bk_resource-0.4.0rc1/MANIFEST.in
-drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource.egg-info/
--rw-r--r--   0 orenzhang   (501) staff       (20)      221 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource.egg-info/PKG-INFO
--rw-r--r--   0 orenzhang   (501) staff       (20)     1900 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource.egg-info/SOURCES.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)      164 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource.egg-info/requires.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)       12 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource.egg-info/top_level.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)        1 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/bk_resource.egg-info/dependency_links.txt
--rw-r--r--   0 orenzhang   (501) staff       (20)     1633 2023-04-18 08:21:54.000000 bk_resource-0.4.0rc1/setup.py
--rw-r--r--   0 orenzhang   (501) staff       (20)       38 2023-04-18 08:22:17.000000 bk_resource-0.4.0rc1/setup.cfg
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/
+-rw-r--r--   0 orenzhang   (501) staff       (20)      221 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/PKG-INFO
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/
+-rw-r--r--   0 orenzhang   (501) staff       (20)     3022 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo
+-rw-r--r--   0 orenzhang   (501) staff       (20)     4398 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/django.po
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/en/
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/
+-rw-r--r--   0 orenzhang   (501) staff       (20)     2943 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/django.mo
+-rw-r--r--   0 orenzhang   (501) staff       (20)     4322 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/django.po
+-rw-r--r--   0 orenzhang   (501) staff       (20)     4064 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/tasks.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)    11571 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/viewsets.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     7083 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/tools.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     2690 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/serializers.py
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/management/
+-rw-r--r--   0 orenzhang   (501) staff       (20)     4859 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/finder.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     4974 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/stub_file_generator.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/__init__.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1110 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/exceptions.py
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/management/commands/
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1243 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/commands/start_resource.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/commands/__init__.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1110 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/commands/generate_resource_stub_file.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)    10304 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/management/root.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     2058 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/__init__.py
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/utils/
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1176 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/inspectors.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     3337 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/local.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1593 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/request.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)    10609 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/cache.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/__init__.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)      950 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/logger.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     2080 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/generators.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)    10967 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/time_tools.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     3313 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/text.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     3317 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/request_log.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)    13170 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/common_utils.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     5017 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/utils/thread_backend.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1132 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/apps.py
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/contrib/
+-rw-r--r--   0 orenzhang   (501) staff       (20)     5589 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/bk_api.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     2969 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/cache.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1121 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/__init__.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     5941 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/model.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     8620 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/contrib/api.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     3724 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/settings.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)     3883 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/exceptions.py
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/conf/
+-rw-r--r--   0 orenzhang   (501) staff       (20)      891 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/__init__.py
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/migrations/
+-rw-r--r--   0 orenzhang   (501) staff       (20)       24 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/migrations/__init__.py-tpl
+-rw-r--r--   0 orenzhang   (501) staff       (20)       24 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/__init__.py-tpl
+-rw-r--r--   0 orenzhang   (501) staff       (20)      152 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/resources.py-tpl
+-rw-r--r--   0 orenzhang   (501) staff       (20)      173 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/views.py-tpl
+-rw-r--r--   0 orenzhang   (501) staff       (20)      189 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/urls.py-tpl
+-rw-r--r--   0 orenzhang   (501) staff       (20)       60 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/admin.py-tpl
+-rw-r--r--   0 orenzhang   (501) staff       (20)      196 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/apps.py-tpl
+-rw-r--r--   0 orenzhang   (501) staff       (20)       64 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/serializers.py-tpl
+-rw-r--r--   0 orenzhang   (501) staff       (20)       54 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/conf/app_template/models.py-tpl
+-rw-r--r--   0 orenzhang   (501) staff       (20)     2369 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/routers.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)    13832 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/bk_resource/base.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)      141 2023-04-21 03:31:52.000000 bk_resource-0.4.0rc2/MANIFEST.in
+drwxr-xr-x   0 orenzhang   (501) staff       (20)        0 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/
+-rw-r--r--   0 orenzhang   (501) staff       (20)      221 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/PKG-INFO
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1900 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/SOURCES.txt
+-rw-r--r--   0 orenzhang   (501) staff       (20)      164 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/requires.txt
+-rw-r--r--   0 orenzhang   (501) staff       (20)       12 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/top_level.txt
+-rw-r--r--   0 orenzhang   (501) staff       (20)        1 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/bk_resource.egg-info/dependency_links.txt
+-rw-r--r--   0 orenzhang   (501) staff       (20)     1633 2023-04-21 03:31:53.000000 bk_resource-0.4.0rc2/setup.py
+-rw-r--r--   0 orenzhang   (501) staff       (20)       38 2023-04-21 03:32:04.000000 bk_resource-0.4.0rc2/setup.cfg
```

### Comparing `bk_resource-0.4.0rc1/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo` & `bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/locale/zh_CN/LC_MESSAGES/django.po` & `bk_resource-0.4.0rc2/bk_resource/locale/zh_CN/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/locale/en/LC_MESSAGES/django.mo` & `bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/django.mo`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/locale/en/LC_MESSAGES/django.po` & `bk_resource-0.4.0rc2/bk_resource/locale/en/LC_MESSAGES/django.po`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/tasks.py` & `bk_resource-0.4.0rc2/bk_resource/tasks.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/viewsets.py` & `bk_resource-0.4.0rc2/bk_resource/viewsets.py`

 * *Files 1% similar despite different names*

```diff
@@ -223,36 +223,38 @@
         生成方法模版
         """
 
         def template(self, request, *args, **kwargs):
             start_time = arrow.now().datetime
 
             resource = resource_route.resource_class()
-            params = request.query_params.copy() if resource_route.method == "GET" else request.data
+            request_data = request.query_params.copy() if resource_route.method == "GET" else request.data
 
             # 如果是detail route，需要重url参数中获取主键，并塞到请求参数中
             if resource_route.pk_field:
-                params.update({resource_route.pk_field: kwargs[cls.lookup_field]})
+                request_data.update({resource_route.pk_field: kwargs[cls.lookup_field]})
 
             # 合并url path params
             if kwargs:
-                params.update(kwargs)
+                request_data.update(kwargs)
+
+            params = {"request_data": request_data}
 
             # 判断是否需要绑定request对象
             if resource.bind_request:
                 params["_request"] = request
 
             is_async_task = "HTTP_X_ASYNC_TASK" in request.META
             if is_async_task:
                 # 执行异步任务
-                data = resource.delay(params)
+                data = resource.delay(**params)
                 response = Response(data)
             else:
                 try:
-                    data = resource.request(params)
+                    data = resource.request(**params)
                     if isinstance(data, Response):
                         response = data
                         data = data.data
                     elif isinstance(data, HttpResponseBase):
                         response = data
                         data = getattr(data, "content", "")
                     elif resource_route.enable_paginate:
@@ -268,12 +270,12 @@
                 response.content_encoding = resource_route.content_encoding
 
             end_time = arrow.now().datetime
 
             # 记录请求日志
             resource_name = "{}.{}".format(resource.__class__.__module__, resource.__class__.__name__)
             log_handler = bk_resource_settings.REQUEST_LOG_HANDLER
-            log_handler(resource_name, start_time, end_time, params, data).record()
+            log_handler(resource_name, start_time, end_time, request_data, data).record()
 
             return response
 
         return template
```

### Comparing `bk_resource-0.4.0rc1/bk_resource/tools.py` & `bk_resource-0.4.0rc2/bk_resource/tools.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/serializers.py` & `bk_resource-0.4.0rc2/bk_resource/serializers.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/management/finder.py` & `bk_resource-0.4.0rc2/bk_resource/management/finder.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/management/stub_file_generator.py` & `bk_resource-0.4.0rc2/bk_resource/management/stub_file_generator.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/management/__init__.py` & `bk_resource-0.4.0rc2/bk_resource/management/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/management/exceptions.py` & `bk_resource-0.4.0rc2/bk_resource/management/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/management/commands/start_resource.py` & `bk_resource-0.4.0rc2/bk_resource/management/commands/start_resource.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/management/commands/__init__.py` & `bk_resource-0.4.0rc2/bk_resource/management/commands/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/management/commands/generate_resource_stub_file.py` & `bk_resource-0.4.0rc2/bk_resource/management/commands/generate_resource_stub_file.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/management/root.py` & `bk_resource-0.4.0rc2/bk_resource/management/root.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/__init__.py` & `bk_resource-0.4.0rc2/bk_resource/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/inspectors.py` & `bk_resource-0.4.0rc2/bk_resource/utils/inspectors.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/local.py` & `bk_resource-0.4.0rc2/bk_resource/utils/local.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/request.py` & `bk_resource-0.4.0rc2/bk_resource/utils/request.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/cache.py` & `bk_resource-0.4.0rc2/bk_resource/utils/cache.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/__init__.py` & `bk_resource-0.4.0rc2/bk_resource/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/logger.py` & `bk_resource-0.4.0rc2/bk_resource/utils/logger.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/generators.py` & `bk_resource-0.4.0rc2/bk_resource/utils/generators.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/time_tools.py` & `bk_resource-0.4.0rc2/bk_resource/utils/time_tools.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/text.py` & `bk_resource-0.4.0rc2/bk_resource/utils/text.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/request_log.py` & `bk_resource-0.4.0rc2/bk_resource/utils/request_log.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/common_utils.py` & `bk_resource-0.4.0rc2/bk_resource/utils/common_utils.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/utils/thread_backend.py` & `bk_resource-0.4.0rc2/bk_resource/utils/thread_backend.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/apps.py` & `bk_resource-0.4.0rc2/bk_resource/apps.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/contrib/bk_api.py` & `bk_resource-0.4.0rc2/bk_resource/contrib/bk_api.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/contrib/cache.py` & `bk_resource-0.4.0rc2/bk_resource/contrib/cache.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/contrib/__init__.py` & `bk_resource-0.4.0rc2/bk_resource/contrib/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/contrib/model.py` & `bk_resource-0.4.0rc2/bk_resource/contrib/model.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/contrib/api.py` & `bk_resource-0.4.0rc2/bk_resource/contrib/api.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/settings.py` & `bk_resource-0.4.0rc2/bk_resource/settings.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/exceptions.py` & `bk_resource-0.4.0rc2/bk_resource/exceptions.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/conf/__init__.py` & `bk_resource-0.4.0rc2/bk_resource/conf/__init__.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/routers.py` & `bk_resource-0.4.0rc2/bk_resource/routers.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource/base.py` & `bk_resource-0.4.0rc2/bk_resource/base.py`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/bk_resource.egg-info/SOURCES.txt` & `bk_resource-0.4.0rc2/bk_resource.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `bk_resource-0.4.0rc1/setup.py` & `bk_resource-0.4.0rc2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -16,15 +16,15 @@
 to the current version of the project delivered to anyone in the future.
 """
 
 from setuptools import setup
 
 setup(
     name="bk_resource",
-    version="0.4.0-rc.1",
+    version="0.4.0-rc.2",
     author="blueking",
     url="https://bk.tencent.com",
     author_email="blueking@tencent.com",
     description="Bk Resource",
     packages=[
         "bk_resource",
         "bk_resource.conf",
```

