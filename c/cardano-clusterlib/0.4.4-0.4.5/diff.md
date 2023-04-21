# Comparing `tmp/cardano-clusterlib-0.4.4.tar.gz` & `tmp/cardano-clusterlib-0.4.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cardano-clusterlib-0.4.4.tar", last modified: Fri Apr 14 10:59:52 2023, max compression
+gzip compressed data, was "cardano-clusterlib-0.4.5.tar", last modified: Fri Apr 21 11:16:25 2023, max compression
```

## Comparing `cardano-clusterlib-0.4.4.tar` & `cardano-clusterlib-0.4.5.tar`

### file list

```diff
@@ -1,59 +1,59 @@
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.674931 cardano-clusterlib-0.4.4/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.668931 cardano-clusterlib-0.4.4/.github/
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.670931 cardano-clusterlib-0.4.4/.github/workflows/
--rw-r--r--   0 martink   (1000) martink   (1000)      353 2022-08-30 10:58:34.000000 cardano-clusterlib-0.4.4/.github/workflows/repo_lint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)      948 2021-12-16 16:01:16.000000 cardano-clusterlib-0.4.4/.gitignore
--rw-r--r--   0 martink   (1000) martink   (1000)      698 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.4/.markdownlint.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     1744 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.4/.pre-commit-config.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     2523 2022-06-03 10:16:54.000000 cardano-clusterlib-0.4.4/.pylintrc
--rw-r--r--   0 martink   (1000) martink   (1000)      318 2021-03-11 15:25:52.000000 cardano-clusterlib-0.4.4/.readthedocs.yaml
--rw-r--r--   0 martink   (1000) martink   (1000)     3267 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.4/CODE-OF-CONDUCT.md
--rw-r--r--   0 martink   (1000) martink   (1000)    11360 2023-03-16 13:20:33.000000 cardano-clusterlib-0.4.4/LICENSE
--rw-r--r--   0 martink   (1000) martink   (1000)     1279 2023-04-14 10:59:03.000000 cardano-clusterlib-0.4.4/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-04-14 10:59:52.674931 cardano-clusterlib-0.4.4/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     7170 2023-03-16 13:15:07.000000 cardano-clusterlib-0.4.4/README.md
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.672931 cardano-clusterlib-0.4.4/cardano_clusterlib/
--rw-r--r--   0 martink   (1000) martink   (1000)      174 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/__init__.py
--rw-r--r--   0 martink   (1000) martink   (1000)     8083 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/address_group.py
--rw-rw-r--   0 martink   (1000) martink   (1000)     2593 2022-08-06 21:08:03.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7791 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib_helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)    14563 2023-03-28 12:40:20.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib_klass.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1086 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/consts.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1111 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/coverage.py
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/exceptions.py
--rw-r--r--   0 martink   (1000) martink   (1000)     3799 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/genesis_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     7438 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/governance_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     1554 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/helpers.py
--rw-r--r--   0 martink   (1000) martink   (1000)     2815 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/key_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6004 2022-10-20 15:45:33.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/node_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)        0 2021-03-10 16:56:29.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/py.typed
--rw-r--r--   0 martink   (1000) martink   (1000)    18162 2023-03-16 11:39:15.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/query_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    13370 2023-04-14 10:37:46.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/stake_address_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    12907 2022-10-25 15:34:32.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/stake_pool_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)     6801 2023-02-08 09:40:33.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/structs.py
--rw-r--r--   0 martink   (1000) martink   (1000)    61308 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/transaction_group.py
--rw-r--r--   0 martink   (1000) martink   (1000)    44202 2023-04-04 10:13:01.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/txtools.py
--rw-r--r--   0 martink   (1000) martink   (1000)      608 2022-06-03 16:16:54.000000 cardano-clusterlib-0.4.4/cardano_clusterlib/types.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.672931 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/
--rw-r--r--   0 martink   (1000) martink   (1000)     7818 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/PKG-INFO
--rw-r--r--   0 martink   (1000) martink   (1000)     1383 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/SOURCES.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/dependency_links.txt
--rw-r--r--   0 martink   (1000) martink   (1000)        1 2021-03-10 16:00:20.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/not-zip-safe
--rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/requires.txt
--rw-r--r--   0 martink   (1000) martink   (1000)       19 2023-04-14 10:59:52.000000 cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/top_level.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.672931 cardano-clusterlib-0.4.4/docs/
--rw-r--r--   0 martink   (1000) martink   (1000)      740 2021-03-23 15:49:32.000000 cardano-clusterlib-0.4.4/docs/Makefile
--rw-r--r--   0 martink   (1000) martink   (1000)       36 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.4/docs/requirements.txt
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.673931 cardano-clusterlib-0.4.4/docs/source/
--rw-r--r--   0 martink   (1000) martink   (1000)     3694 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.4/docs/source/cardano_clusterlib.rst
--rw-r--r--   0 martink   (1000) martink   (1000)     4080 2022-09-23 12:55:52.000000 cardano-clusterlib-0.4.4/docs/source/conf.py
--rw-r--r--   0 martink   (1000) martink   (1000)      491 2021-03-11 13:53:31.000000 cardano-clusterlib-0.4.4/docs/source/index.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       95 2021-03-11 13:52:06.000000 cardano-clusterlib-0.4.4/docs/source/modules.rst
--rw-r--r--   0 martink   (1000) martink   (1000)       31 2021-03-11 13:53:55.000000 cardano-clusterlib-0.4.4/docs/source/readme.rst
--rw-r--r--   0 martink   (1000) martink   (1000)      236 2021-03-10 15:33:40.000000 cardano-clusterlib-0.4.4/mypy.ini
--rw-r--r--   0 martink   (1000) martink   (1000)      521 2023-03-16 10:22:51.000000 cardano-clusterlib-0.4.4/pyproject.toml
--rw-r--r--   0 martink   (1000) martink   (1000)       59 2023-01-19 14:58:18.000000 cardano-clusterlib-0.4.4/requirements-dev.txt
--rw-r--r--   0 martink   (1000) martink   (1000)     1128 2023-04-14 10:59:52.674931 cardano-clusterlib-0.4.4/setup.cfg
--rw-r--r--   0 martink   (1000) martink   (1000)      163 2021-08-27 11:24:08.000000 cardano-clusterlib-0.4.4/setup.py
-drwxr-xr-x   0 martink   (1000) martink   (1000)        0 2023-04-14 10:59:52.674931 cardano-clusterlib-0.4.4/upgrading/
--rw-r--r--   0 martink   (1000) martink   (1000)     7363 2022-10-21 06:56:49.000000 cardano-clusterlib-0.4.4/upgrading/refactor_to_0_4_0rc1.sed
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.628790 cardano-clusterlib-0.4.5/.github/
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.628790 cardano-clusterlib-0.4.5/.github/workflows/
+-rw-r--r--   0 sara      (1000) sara      (1000)      353 2022-09-08 20:06:48.000000 cardano-clusterlib-0.4.5/.github/workflows/repo_lint.yaml
+-rw-rw-r--   0 sara      (1000) sara      (1000)      948 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/.gitignore
+-rw-r--r--   0 sara      (1000) sara      (1000)      698 2022-09-26 14:22:34.000000 cardano-clusterlib-0.4.5/.markdownlint.yaml
+-rw-r--r--   0 sara      (1000) sara      (1000)     1347 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/.pre-commit-config.yaml
+-rw-rw-r--   0 sara      (1000) sara      (1000)     2523 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/.pylintrc
+-rw-rw-r--   0 sara      (1000) sara      (1000)      318 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/.readthedocs.yaml
+-rw-r--r--   0 sara      (1000) sara      (1000)     3267 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/CODE-OF-CONDUCT.md
+-rw-r--r--   0 sara      (1000) sara      (1000)    11360 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/LICENSE
+-rw-r--r--   0 sara      (1000) sara      (1000)     1279 2023-04-14 14:27:56.000000 cardano-clusterlib-0.4.5/Makefile
+-rw-r--r--   0 sara      (1000) sara      (1000)     7853 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/PKG-INFO
+-rw-r--r--   0 sara      (1000) sara      (1000)     7170 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/README.md
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/cardano_clusterlib/
+-rw-rw-r--   0 sara      (1000) sara      (1000)      174 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/__init__.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     8119 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/address_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     2593 2022-08-23 09:17:09.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     7791 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib_helpers.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    14563 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib_klass.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     1086 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/consts.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     1111 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/coverage.py
+-rw-rw-r--   0 sara      (1000) sara      (1000)       36 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/exceptions.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     3799 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/genesis_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     7438 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/governance_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     1554 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/helpers.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     2815 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/key_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     6004 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/node_group.py
+-rw-rw-r--   0 sara      (1000) sara      (1000)        0 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/py.typed
+-rw-r--r--   0 sara      (1000) sara      (1000)    18201 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/query_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    13370 2023-04-14 14:27:56.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/stake_address_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    12907 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/stake_pool_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)     6849 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/structs.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    62035 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/transaction_group.py
+-rw-r--r--   0 sara      (1000) sara      (1000)    44202 2023-04-10 13:23:53.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/txtools.py
+-rw-rw-r--   0 sara      (1000) sara      (1000)      608 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/cardano_clusterlib/types.py
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/
+-rw-r--r--   0 sara      (1000) sara      (1000)     7853 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/PKG-INFO
+-rw-r--r--   0 sara      (1000) sara      (1000)     1383 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/SOURCES.txt
+-rw-r--r--   0 sara      (1000) sara      (1000)        1 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/dependency_links.txt
+-rw-r--r--   0 sara      (1000) sara      (1000)        1 2022-08-03 14:24:31.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/not-zip-safe
+-rw-r--r--   0 sara      (1000) sara      (1000)       19 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/requires.txt
+-rw-r--r--   0 sara      (1000) sara      (1000)       19 2023-04-21 11:16:25.000000 cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/top_level.txt
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/docs/
+-rw-rw-r--   0 sara      (1000) sara      (1000)      740 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/docs/Makefile
+-rw-r--r--   0 sara      (1000) sara      (1000)       36 2022-09-26 14:22:34.000000 cardano-clusterlib-0.4.5/docs/requirements.txt
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/docs/source/
+-rw-r--r--   0 sara      (1000) sara      (1000)     3694 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/docs/source/cardano_clusterlib.rst
+-rw-r--r--   0 sara      (1000) sara      (1000)     4112 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/docs/source/conf.py
+-rw-rw-r--   0 sara      (1000) sara      (1000)      491 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/docs/source/index.rst
+-rw-rw-r--   0 sara      (1000) sara      (1000)       95 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/docs/source/modules.rst
+-rw-rw-r--   0 sara      (1000) sara      (1000)       31 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/docs/source/readme.rst
+-rw-rw-r--   0 sara      (1000) sara      (1000)      236 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/mypy.ini
+-rw-r--r--   0 sara      (1000) sara      (1000)      577 2023-04-17 14:07:29.000000 cardano-clusterlib-0.4.5/pyproject.toml
+-rw-r--r--   0 sara      (1000) sara      (1000)       59 2023-03-20 14:27:55.000000 cardano-clusterlib-0.4.5/requirements-dev.txt
+-rw-r--r--   0 sara      (1000) sara      (1000)     1128 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/setup.cfg
+-rw-rw-r--   0 sara      (1000) sara      (1000)      163 2022-08-03 14:23:07.000000 cardano-clusterlib-0.4.5/setup.py
+drwxr-xr-x   0 sara      (1000) sara      (1000)        0 2023-04-21 11:16:25.632790 cardano-clusterlib-0.4.5/upgrading/
+-rw-r--r--   0 sara      (1000) sara      (1000)     7363 2022-10-21 14:01:30.000000 cardano-clusterlib-0.4.5/upgrading/refactor_to_0_4_0rc1.sed
```

### Comparing `cardano-clusterlib-0.4.4/.gitignore` & `cardano-clusterlib-0.4.5/.gitignore`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/.markdownlint.yaml` & `cardano-clusterlib-0.4.5/.markdownlint.yaml`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/.pre-commit-config.yaml` & `cardano-clusterlib-0.4.5/.pre-commit-config.yaml`

 * *Files 15% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 - repo: https://github.com/asottile/reorder_python_imports
   rev: v3.9.0
   hooks:
   - id: reorder-python-imports
     entry: env SETUPTOOLS_USE_DISTUTILS=stdlib reorder-python-imports
     language_version: python3
 - repo: https://github.com/ambv/black
-  rev: 23.1.0
+  rev: 23.3.0
   hooks:
   - id: black
     args: [--safe, --quiet]
     language_version: python3
     require_serial: true
 - repo: https://github.com/pre-commit/pre-commit-hooks
   rev: v4.4.0
@@ -21,45 +21,28 @@
   - id: end-of-file-fixer
     language_version: python3
     exclude_types: [html]
   - id: check-yaml
     language_version: python3
   - id: debug-statements
     language_version: python3
-- repo: https://github.com/pycqa/flake8.git
-  rev: 6.0.0
-  hooks:
-  - id: flake8
-    language_version: python3
-    additional_dependencies:
-    - flake8-use-pathlib
-- repo: https://github.com/asottile/pyupgrade
-  rev: v3.3.1
-  hooks:
-  - id: pyupgrade
-    language_version: python3
-- repo: https://github.com/pycqa/pydocstyle
-  rev: 6.3.0
-  hooks:
-  - id: pydocstyle
-    language_version: python3
 - repo: https://github.com/charliermarsh/ruff-pre-commit
-  rev: v0.0.254
+  rev: v0.0.261
   hooks:
     - id: ruff
 - repo: https://github.com/shellcheck-py/shellcheck-py
   rev: v0.9.0.2
   hooks:
   - id: shellcheck
 - repo: https://github.com/igorshubovych/markdownlint-cli
   rev: v0.33.0
   hooks:
   - id: markdownlint
 - repo: https://github.com/rstcheck/rstcheck
-  rev: v6.1.1
+  rev: v6.1.2
   hooks:
   - id: rstcheck
     additional_dependencies: [sphinx]
 - repo: local
   hooks:
   - id: pylint
     name: pylint
```

### Comparing `cardano-clusterlib-0.4.4/.pylintrc` & `cardano-clusterlib-0.4.5/.pylintrc`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/CODE-OF-CONDUCT.md` & `cardano-clusterlib-0.4.5/CODE-OF-CONDUCT.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/LICENSE` & `cardano-clusterlib-0.4.5/LICENSE`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/Makefile` & `cardano-clusterlib-0.4.5/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/PKG-INFO` & `cardano-clusterlib-0.4.5/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `cardano-clusterlib-0.4.4/README.md` & `cardano-clusterlib-0.4.5/README.md`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/address_group.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/address_group.py`

 * *Files 1% similar despite different names*

```diff
@@ -177,15 +177,17 @@
             addr_name: A name of payment address.
             script_file: A path to corresponding script file.
             destination_dir: A path to directory for storing artifacts (optional).
 
         Returns:
             str: A generated script address.
         """
-        warnings.warn("`gen_script_addr` deprecated by `gen_payment_addr`", DeprecationWarning)
+        warnings.warn(
+            "`gen_script_addr` deprecated by `gen_payment_addr`", DeprecationWarning, stacklevel=2
+        )
         return self.gen_payment_addr(
             addr_name=addr_name, payment_script_file=script_file, destination_dir=destination_dir
         )
 
     def gen_payment_addr_and_keys(
         self,
         name: str,
```

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib_helpers.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib_helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/clusterlib_klass.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/clusterlib_klass.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/consts.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/consts.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/coverage.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/coverage.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/genesis_group.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/genesis_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/governance_group.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/governance_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/helpers.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/helpers.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/key_group.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/key_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/node_group.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/node_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/query_group.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/query_group.py`

 * *Files 0% similar despite different names*

```diff
@@ -195,15 +195,17 @@
         Args:
             stake_pool_id: An ID of the stake pool (Bech32-encoded or hex-encoded).
 
         Returns:
             dict: A pool parameters.
         """
         warnings.warn(
-            "`pool-params` deprecated by `pool-state` for node 1.35.4+", DeprecationWarning
+            "`pool-params` deprecated by `pool-state` for node 1.35.4+",
+            DeprecationWarning,
+            stacklevel=2,
         )
 
         pool_params: dict = json.loads(
             self.query_cli(["pool-params", "--stake-pool-id", stake_pool_id])
         )
 
         # in node 1.35.1+ the information is nested under hex encoded stake pool ID
```

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/stake_address_group.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/stake_address_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/stake_pool_group.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/stake_pool_group.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/structs.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/structs.py`

 * *Files 2% similar despite different names*

```diff
@@ -157,14 +157,15 @@
 class TxFiles(NamedTuple):
     certificate_files: OptionalFiles = ()
     proposal_files: OptionalFiles = ()
     metadata_json_files: OptionalFiles = ()
     metadata_cbor_files: OptionalFiles = ()
     signing_key_files: OptionalFiles = ()
     auxiliary_script_files: OptionalFiles = ()
+    metadata_json_detailed_schema: bool = False
 
 
 class PoolUser(NamedTuple):
     payment: AddressRecord
     stake: AddressRecord
```

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/transaction_group.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/transaction_group.py`

 * *Files 2% similar despite different names*

```diff
@@ -272,14 +272,17 @@
             )
 
         if total_collateral_amount:
             misc_args.extend(["--tx-total-collateral", str(total_collateral_amount)])
 
         misc_args.extend(["--cddl-format"] if self._clusterlib_obj.use_cddl else [])
 
+        if tx_files.metadata_json_files and tx_files.metadata_json_detailed_schema:
+            misc_args.append("--json-metadata-detailed-schema")
+
         cli_args = [
             "transaction",
             "build-raw",
             "--fee",
             str(fee),
             "--out-file",
             str(out_file),
@@ -591,15 +594,19 @@
 
         Args:
             multi_assets: A list of `TxOuts`, specifying multi-assets.
 
         Returns:
             structs.Value: A tuple describing the value.
         """
-        warnings.warn("deprecated by `calculate_min_req_utxo` for node 1.29.0+", DeprecationWarning)
+        warnings.warn(
+            "deprecated by `calculate_min_req_utxo` for node 1.29.0+",
+            DeprecationWarning,
+            stacklevel=2,
+        )
 
         ma_records = [f"{m.amount} {m.coin}" for m in multi_assets]
         ma_args = ["--multi-asset", "+".join(ma_records)] if ma_records else []
 
         self._clusterlib_obj.create_pparams_file()
         stdout = self._clusterlib_obj.cli(
             [
@@ -831,14 +838,17 @@
 
         if calc_script_cost_file:
             misc_args.extend(["--calculate-plutus-script-cost", str(calc_script_cost_file)])
             out_file = Path(calc_script_cost_file)
         else:
             misc_args.extend(["--out-file", str(out_file)])
 
+        if tx_files.metadata_json_files and tx_files.metadata_json_detailed_schema:
+            misc_args.append("--json-metadata-detailed-schema")
+
         cli_args = [
             "transaction",
             "build",
             *grouped_args,
             *helpers._prepend_flag("--tx-in", txin_strings),
             *txout_args,
             *helpers._prepend_flag("--required-signer", required_signers),
@@ -1289,38 +1299,38 @@
             self._clusterlib_obj.cli(["transaction", "policyid", "--script-file", str(script_file)])
             .stdout.rstrip()
             .decode("utf-8")
         )
 
     def calculate_plutus_script_cost(
         self,
-        src_address: str,
+        src_address: str,  # noqa: ARG002
         tx_name: str,
-        txins: structs.OptionalUTXOData = (),
-        txouts: structs.OptionalTxOuts = (),
-        readonly_reference_txins: structs.OptionalUTXOData = (),
-        script_txins: structs.OptionalScriptTxIn = (),
-        return_collateral_txouts: structs.OptionalTxOuts = (),
-        total_collateral_amount: Optional[int] = None,
-        mint: structs.OptionalMint = (),
-        tx_files: Optional[structs.TxFiles] = None,
-        complex_certs: structs.OptionalScriptCerts = (),
-        change_address: str = "",
-        fee_buffer: Optional[int] = None,
-        required_signers: OptionalFiles = (),
-        required_signer_hashes: Optional[List[str]] = None,
-        withdrawals: structs.OptionalTxOuts = (),
-        script_withdrawals: structs.OptionalScriptWithdrawals = (),
-        deposit: Optional[int] = None,
-        invalid_hereafter: Optional[int] = None,
-        invalid_before: Optional[int] = None,
-        witness_override: Optional[int] = None,
-        script_valid: bool = True,
-        calc_script_cost_file: Optional[FileType] = None,
-        join_txouts: bool = True,
+        txins: structs.OptionalUTXOData = (),  # noqa: ARG002
+        txouts: structs.OptionalTxOuts = (),  # noqa: ARG002
+        readonly_reference_txins: structs.OptionalUTXOData = (),  # noqa: ARG002
+        script_txins: structs.OptionalScriptTxIn = (),  # noqa: ARG002
+        return_collateral_txouts: structs.OptionalTxOuts = (),  # noqa: ARG002
+        total_collateral_amount: Optional[int] = None,  # noqa: ARG002
+        mint: structs.OptionalMint = (),  # noqa: ARG002
+        tx_files: Optional[structs.TxFiles] = None,  # noqa: ARG002
+        complex_certs: structs.OptionalScriptCerts = (),  # noqa: ARG002
+        change_address: str = "",  # noqa: ARG002
+        fee_buffer: Optional[int] = None,  # noqa: ARG002
+        required_signers: OptionalFiles = (),  # noqa: ARG002
+        required_signer_hashes: Optional[List[str]] = None,  # noqa: ARG002
+        withdrawals: structs.OptionalTxOuts = (),  # noqa: ARG002
+        script_withdrawals: structs.OptionalScriptWithdrawals = (),  # noqa: ARG002
+        deposit: Optional[int] = None,  # noqa: ARG002
+        invalid_hereafter: Optional[int] = None,  # noqa: ARG002
+        invalid_before: Optional[int] = None,  # noqa: ARG002
+        witness_override: Optional[int] = None,  # noqa: ARG002
+        script_valid: bool = True,  # noqa: ARG002
+        calc_script_cost_file: Optional[FileType] = None,  # noqa: ARG002
+        join_txouts: bool = True,  # noqa: ARG002
         destination_dir: FileType = ".",
     ) -> List[dict]:
         """Calculate cost of Plutus scripts. Accepts the same arguments as `build_tx`.
 
         Args:
             src_address: An address used for fee and inputs (if inputs not specified by `txins`).
             tx_name: A name of the transaction.
```

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/txtools.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/txtools.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib/types.py` & `cardano-clusterlib-0.4.5/cardano_clusterlib/types.py`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/PKG-INFO` & `cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,14 +1,16 @@
 Metadata-Version: 2.1
 Name: cardano-clusterlib
-Version: 0.4.4
+Version: 0.4.5
 Summary: Python wrapper for cardano-cli for working with cardano cluster
 Home-page: https://github.com/input-output-hk/cardano-clusterlib-py
 Maintainer: Martin Kourim
 Maintainer-email: martin.kourim@iohk.io
+License: UNKNOWN
+Platform: UNKNOWN
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Intended Audience :: Developers
 Description-Content-Type: text/markdown
```

### Comparing `cardano-clusterlib-0.4.4/cardano_clusterlib.egg-info/SOURCES.txt` & `cardano-clusterlib-0.4.5/cardano_clusterlib.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/docs/Makefile` & `cardano-clusterlib-0.4.5/docs/Makefile`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/docs/source/cardano_clusterlib.rst` & `cardano-clusterlib-0.4.5/docs/source/cardano_clusterlib.rst`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/docs/source/conf.py` & `cardano-clusterlib-0.4.5/docs/source/conf.py`

 * *Files 5% similar despite different names*

```diff
@@ -13,15 +13,15 @@
 import cardano_clusterlib
 
 # -- Path setup --------------------------------------------------------------
 
 # If extensions (or modules to document with autodoc) are in another directory,
 # add these directories to sys.path here. If the directory is relative to the
 # documentation root, use os.path.abspath to make it absolute, like shown here.
-sys.path.insert(0, os.path.abspath(".."))
+sys.path.insert(0, os.path.abspath(".."))  # noqa: PTH100
 
 # -- Project information -----------------------------------------------------
 
 project = "cardano-clusterlib"
 author = "Cardano Test Engineering Team"
 copyright = author
 
@@ -96,15 +96,15 @@
                 return None
 
         # strip decorators, which would resolve to the source of the decorator
         # possibly an upstream bug in getsourcefile, bpo-1764286
         obj = inspect.unwrap(obj)
 
         fn = inspect.getsourcefile(obj)
-        fn = os.path.relpath(fn, start=os.path.dirname(cardano_clusterlib.__file__))
+        fn = os.path.relpath(fn, start=os.path.dirname(cardano_clusterlib.__file__))  # noqa: PTH120
         source, lineno = inspect.getsourcelines(obj)
         return fn, lineno, lineno + len(source) - 1
 
     if domain != "py" or not info["module"]:
         return None
 
     try:
```

### Comparing `cardano-clusterlib-0.4.4/setup.cfg` & `cardano-clusterlib-0.4.5/setup.cfg`

 * *Files identical despite different names*

### Comparing `cardano-clusterlib-0.4.4/upgrading/refactor_to_0_4_0rc1.sed` & `cardano-clusterlib-0.4.5/upgrading/refactor_to_0_4_0rc1.sed`

 * *Files identical despite different names*

