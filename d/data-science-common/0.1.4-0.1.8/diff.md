# Comparing `tmp/data_science_common-0.1.4.tar.gz` & `tmp/data-science-common-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "data_science_common-0.1.4.tar", last modified: Wed Mar  2 15:59:09 2022, max compression
+gzip compressed data, was "data-science-common-0.1.8.tar", last modified: Mon Jul 11 15:54:47 2022, max compression
```

## Comparing `data_science_common-0.1.4.tar` & `data-science-common-0.1.8.tar`

### file list

```diff
@@ -1,14 +1,27 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 15:59:09.968875 data_science_common-0.1.4/
--rw-r--r--   0 runner    (1001) docker     (121)    11357 2022-03-02 15:58:53.000000 data_science_common-0.1.4/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-03-02 15:59:09.968875 data_science_common-0.1.4/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      328 2022-03-02 15:58:53.000000 data_science_common-0.1.4/README.md
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-03-02 15:59:09.968875 data_science_common-0.1.4/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)      743 2022-03-02 15:58:53.000000 data_science_common-0.1.4/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 15:59:09.968875 data_science_common-0.1.4/src/
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-03-02 15:59:09.968875 data_science_common-0.1.4/src/data_science_common.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)      690 2022-03-02 15:59:09.000000 data_science_common-0.1.4/src/data_science_common.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      272 2022-03-02 15:59:09.000000 data_science_common-0.1.4/src/data_science_common.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-03-02 15:59:09.000000 data_science_common-0.1.4/src/data_science_common.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       15 2022-03-02 15:59:09.000000 data_science_common-0.1.4/src/data_science_common.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (121)        5 2022-03-02 15:59:09.000000 data_science_common-0.1.4/src/data_science_common.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)     1735 2022-03-02 15:58:53.000000 data_science_common-0.1.4/src/pids.py
+drwxr-xr-x   0 rwk        (501) staff       (20)        0 2022-07-11 15:54:47.138860 data-science-common-0.1.8/
+-rw-r--r--   0 rwk        (501) staff       (20)    11357 2022-03-01 18:13:46.000000 data-science-common-0.1.8/LICENSE
+-rw-r--r--   0 rwk        (501) staff       (20)       26 2022-07-07 13:44:52.000000 data-science-common-0.1.8/MANIFEST.in
+-rw-r--r--   0 rwk        (501) staff       (20)    16687 2022-07-11 15:54:47.138355 data-science-common-0.1.8/PKG-INFO
+-rw-r--r--   0 rwk        (501) staff       (20)     2773 2022-07-11 15:34:04.000000 data-science-common-0.1.8/README.md
+-rw-r--r--   0 rwk        (501) staff       (20)     2147 2022-07-11 15:48:42.000000 data-science-common-0.1.8/pyproject.toml
+-rw-r--r--   0 rwk        (501) staff       (20)       38 2022-07-11 15:54:47.138976 data-science-common-0.1.8/setup.cfg
+-rw-r--r--   0 rwk        (501) staff       (20)       60 2022-07-11 14:43:24.000000 data-science-common-0.1.8/setup.py
+drwxr-xr-x   0 rwk        (501) staff       (20)        0 2022-07-11 15:54:47.108962 data-science-common-0.1.8/src/
+-rw-r--r--   0 rwk        (501) staff       (20)        0 2022-07-11 14:41:09.000000 data-science-common-0.1.8/src/__init__.py
+drwxr-xr-x   0 rwk        (501) staff       (20)        0 2022-07-11 15:54:47.127250 data-science-common-0.1.8/src/data_science_common.egg-info/
+-rw-r--r--   0 rwk        (501) staff       (20)    16687 2022-07-11 15:54:47.000000 data-science-common-0.1.8/src/data_science_common.egg-info/PKG-INFO
+-rw-r--r--   0 rwk        (501) staff       (20)      490 2022-07-11 15:54:47.000000 data-science-common-0.1.8/src/data_science_common.egg-info/SOURCES.txt
+-rw-r--r--   0 rwk        (501) staff       (20)        1 2022-07-11 15:54:47.000000 data-science-common-0.1.8/src/data_science_common.egg-info/dependency_links.txt
+-rw-r--r--   0 rwk        (501) staff       (20)      171 2022-07-11 15:54:47.000000 data-science-common-0.1.8/src/data_science_common.egg-info/requires.txt
+-rw-r--r--   0 rwk        (501) staff       (20)       13 2022-07-11 15:54:47.000000 data-science-common-0.1.8/src/data_science_common.egg-info/top_level.txt
+drwxr-xr-x   0 rwk        (501) staff       (20)        0 2022-07-11 15:54:47.128637 data-science-common-0.1.8/src/dsc/
+-rw-r--r--   0 rwk        (501) staff       (20)      194 2022-07-11 15:48:42.000000 data-science-common-0.1.8/src/dsc/__init__.py
+drwxr-xr-x   0 rwk        (501) staff       (20)        0 2022-07-11 15:54:47.137454 data-science-common-0.1.8/src/dsc/util/
+-rw-r--r--   0 rwk        (501) staff       (20)        0 2022-03-02 17:31:32.000000 data-science-common-0.1.8/src/dsc/util/__init__.py
+-rw-r--r--   0 rwk        (501) staff       (20)      788 2022-07-11 15:03:43.000000 data-science-common-0.1.8/src/dsc/util/data.py
+-rw-r--r--   0 rwk        (501) staff       (20)     5301 2022-07-11 15:21:32.000000 data-science-common-0.1.8/src/dsc/util/date.py
+-rw-r--r--   0 rwk        (501) staff       (20)     2733 2022-07-11 15:20:24.000000 data-science-common-0.1.8/src/dsc/util/db.py
+-rw-r--r--   0 rwk        (501) staff       (20)      324 2022-04-19 23:41:13.000000 data-science-common-0.1.8/src/dsc/util/error.py
+-rw-r--r--   0 rwk        (501) staff       (20)     3052 2022-07-11 15:27:32.000000 data-science-common-0.1.8/src/dsc/util/obj.py
+-rw-r--r--   0 rwk        (501) staff       (20)     1041 2022-07-11 15:03:21.000000 data-science-common-0.1.8/src/dsc/util/pd.py
+-rw-r--r--   0 rwk        (501) staff       (20)     2980 2022-07-11 15:21:55.000000 data-science-common-0.1.8/src/dsc/util/str.py
```

### Comparing `data_science_common-0.1.4/LICENSE` & `data-science-common-0.1.8/LICENSE`

 * *Files identical despite different names*

