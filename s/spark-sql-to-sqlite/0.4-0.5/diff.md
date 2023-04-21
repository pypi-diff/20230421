# Comparing `tmp/spark_sql_to_sqlite-0.4.tar.gz` & `tmp/spark_sql_to_sqlite-0.5.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_sql_to_sqlite-0.4.tar", last modified: Fri Apr 21 18:59:45 2023, max compression
+gzip compressed data, was "spark_sql_to_sqlite-0.5.tar", last modified: Fri Apr 21 19:02:08 2023, max compression
```

## Comparing `spark_sql_to_sqlite-0.4.tar` & `spark_sql_to_sqlite-0.5.tar`

### file list

```diff
@@ -1,11 +1,13 @@
-drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 18:59:45.145074 spark_sql_to_sqlite-0.4/
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      101 2023-04-21 18:59:45.144868 spark_sql_to_sqlite-0.4/PKG-INFO
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 17:30:26.000000 spark_sql_to_sqlite-0.4/README.md
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       38 2023-04-21 18:59:45.145133 spark_sql_to_sqlite-0.4/setup.cfg
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      484 2023-04-21 18:59:32.000000 spark_sql_to_sqlite-0.4/setup.py
-drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 18:59:45.144574 spark_sql_to_sqlite-0.4/spark_sql_to_sqlite.egg-info/
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      101 2023-04-21 18:59:44.000000 spark_sql_to_sqlite-0.4/spark_sql_to_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      232 2023-04-21 18:59:45.000000 spark_sql_to_sqlite-0.4/spark_sql_to_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        1 2023-04-21 18:59:44.000000 spark_sql_to_sqlite-0.4/spark_sql_to_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       15 2023-04-21 18:59:44.000000 spark_sql_to_sqlite-0.4/spark_sql_to_sqlite.egg-info/requires.txt
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        1 2023-04-21 18:59:44.000000 spark_sql_to_sqlite-0.4/spark_sql_to_sqlite.egg-info/top_level.txt
+drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 19:02:08.147185 spark_sql_to_sqlite-0.5/
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      101 2023-04-21 19:02:08.146980 spark_sql_to_sqlite-0.5/PKG-INFO
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 17:30:26.000000 spark_sql_to_sqlite-0.5/README.md
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       38 2023-04-21 19:02:08.147251 spark_sql_to_sqlite-0.5/setup.cfg
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      484 2023-04-21 19:01:53.000000 spark_sql_to_sqlite-0.5/setup.py
+drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 19:02:08.145329 spark_sql_to_sqlite-0.5/spark_sql_to_sqlite/
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      839 2023-04-21 17:14:27.000000 spark_sql_to_sqlite-0.5/spark_sql_to_sqlite/__init__.py
+drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 19:02:08.146714 spark_sql_to_sqlite-0.5/spark_sql_to_sqlite.egg-info/
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      101 2023-04-21 19:02:07.000000 spark_sql_to_sqlite-0.5/spark_sql_to_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      264 2023-04-21 19:02:08.000000 spark_sql_to_sqlite-0.5/spark_sql_to_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        1 2023-04-21 19:02:07.000000 spark_sql_to_sqlite-0.5/spark_sql_to_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       15 2023-04-21 19:02:07.000000 spark_sql_to_sqlite-0.5/spark_sql_to_sqlite.egg-info/requires.txt
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       20 2023-04-21 19:02:07.000000 spark_sql_to_sqlite-0.5/spark_sql_to_sqlite.egg-info/top_level.txt
```

