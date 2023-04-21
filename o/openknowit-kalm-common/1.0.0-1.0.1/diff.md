# Comparing `tmp/openknowit_kalm_common-1.0.0.tar.gz` & `tmp/openknowit_kalm_common-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "openknowit_kalm_common-1.0.0.tar", last modified: Fri Apr 21 10:19:04 2023, max compression
+gzip compressed data, was "openknowit_kalm_common-1.0.1.tar", last modified: Fri Apr 21 10:20:58 2023, max compression
```

## Comparing `openknowit_kalm_common-1.0.0.tar` & `openknowit_kalm_common-1.0.1.tar`

### file list

```diff
@@ -1,18 +1,17 @@
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:19:04.169461 openknowit_kalm_common-1.0.0/
--rw-rw-r--   0 jho       (1000) jho       (1000)      180 2023-04-21 10:19:04.169461 openknowit_kalm_common-1.0.0/PKG-INFO
--rw-rw-r--   0 jho       (1000) jho       (1000)       72 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.0/README.md
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:19:04.168461 openknowit_kalm_common-1.0.0/openknowit_kalm_common/
--rw-rw-r--   0 jho       (1000) jho       (1000)       33 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.0/openknowit_kalm_common/__init__.py
--rw-rw-r--   0 jho       (1000) jho       (1000)        0 2023-04-21 09:13:55.000000 openknowit_kalm_common-1.0.0/openknowit_kalm_common/__main__.py
--rw-rw-r--   0 jho       (1000) jho       (1000)       96 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.0/openknowit_kalm_common/cli.py
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:19:04.168461 openknowit_kalm_common-1.0.0/openknowit_kalm_common.egg-info/
--rw-rw-r--   0 jho       (1000) jho       (1000)      180 2023-04-21 10:19:04.000000 openknowit_kalm_common-1.0.0/openknowit_kalm_common.egg-info/PKG-INFO
--rw-rw-r--   0 jho       (1000) jho       (1000)      384 2023-04-21 10:19:04.000000 openknowit_kalm_common-1.0.0/openknowit_kalm_common.egg-info/SOURCES.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)        1 2023-04-21 10:19:04.000000 openknowit_kalm_common-1.0.0/openknowit_kalm_common.egg-info/dependency_links.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)     1252 2023-04-21 10:19:04.000000 openknowit_kalm_common-1.0.0/openknowit_kalm_common.egg-info/requires.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       29 2023-04-21 10:19:04.000000 openknowit_kalm_common-1.0.0/openknowit_kalm_common.egg-info/top_level.txt
--rw-rw-r--   0 jho       (1000) jho       (1000)       38 2023-04-21 10:19:04.169461 openknowit_kalm_common-1.0.0/setup.cfg
--rw-rw-r--   0 jho       (1000) jho       (1000)     1708 2023-04-21 10:18:29.000000 openknowit_kalm_common-1.0.0/setup.py
-drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:19:04.169461 openknowit_kalm_common-1.0.0/tests/
--rw-rw-r--   0 jho       (1000) jho       (1000)       41 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.0/tests/__init__.py
--rw-rw-r--   0 jho       (1000) jho       (1000)       76 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.0/tests/test_main.py
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:20:58.046092 openknowit_kalm_common-1.0.1/
+-rw-rw-r--   0 jho       (1000) jho       (1000)      180 2023-04-21 10:20:58.046092 openknowit_kalm_common-1.0.1/PKG-INFO
+-rw-rw-r--   0 jho       (1000) jho       (1000)       72 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.1/README.md
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:20:58.045092 openknowit_kalm_common-1.0.1/openknowit_kalm_common/
+-rw-rw-r--   0 jho       (1000) jho       (1000)       33 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.1/openknowit_kalm_common/__init__.py
+-rw-rw-r--   0 jho       (1000) jho       (1000)        0 2023-04-21 09:13:55.000000 openknowit_kalm_common-1.0.1/openknowit_kalm_common/__main__.py
+-rw-rw-r--   0 jho       (1000) jho       (1000)       96 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.1/openknowit_kalm_common/cli.py
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:20:58.046092 openknowit_kalm_common-1.0.1/openknowit_kalm_common.egg-info/
+-rw-rw-r--   0 jho       (1000) jho       (1000)      180 2023-04-21 10:20:58.000000 openknowit_kalm_common-1.0.1/openknowit_kalm_common.egg-info/PKG-INFO
+-rw-rw-r--   0 jho       (1000) jho       (1000)      339 2023-04-21 10:20:58.000000 openknowit_kalm_common-1.0.1/openknowit_kalm_common.egg-info/SOURCES.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)        1 2023-04-21 10:20:58.000000 openknowit_kalm_common-1.0.1/openknowit_kalm_common.egg-info/dependency_links.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)       29 2023-04-21 10:20:58.000000 openknowit_kalm_common-1.0.1/openknowit_kalm_common.egg-info/top_level.txt
+-rw-rw-r--   0 jho       (1000) jho       (1000)       38 2023-04-21 10:20:58.047092 openknowit_kalm_common-1.0.1/setup.cfg
+-rw-rw-r--   0 jho       (1000) jho       (1000)      262 2023-04-21 10:20:53.000000 openknowit_kalm_common-1.0.1/setup.py
+drwxrwxr-x   0 jho       (1000) jho       (1000)        0 2023-04-21 10:20:58.046092 openknowit_kalm_common-1.0.1/tests/
+-rw-rw-r--   0 jho       (1000) jho       (1000)       41 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.1/tests/__init__.py
+-rw-rw-r--   0 jho       (1000) jho       (1000)       76 2023-04-21 08:42:36.000000 openknowit_kalm_common-1.0.1/tests/test_main.py
```

