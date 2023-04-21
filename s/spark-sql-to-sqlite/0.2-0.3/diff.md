# Comparing `tmp/spark_sql_to_sqlite-0.2.tar.gz` & `tmp/spark_sql_to_sqlite-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "spark_sql_to_sqlite-0.2.tar", last modified: Fri Apr 21 17:33:17 2023, max compression
+gzip compressed data, was "spark_sql_to_sqlite-0.3.tar", last modified: Fri Apr 21 18:51:07 2023, max compression
```

## Comparing `spark_sql_to_sqlite-0.2.tar` & `spark_sql_to_sqlite-0.3.tar`

### file list

```diff
@@ -1,11 +1,11 @@
-drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 17:33:17.894263 spark_sql_to_sqlite-0.2/
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      101 2023-04-21 17:33:17.894044 spark_sql_to_sqlite-0.2/PKG-INFO
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 17:30:26.000000 spark_sql_to_sqlite-0.2/README.md
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       38 2023-04-21 17:33:17.894328 spark_sql_to_sqlite-0.2/setup.cfg
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      484 2023-04-21 17:31:17.000000 spark_sql_to_sqlite-0.2/setup.py
-drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 17:33:17.893701 spark_sql_to_sqlite-0.2/spark_sql_to_sqlite.egg-info/
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      101 2023-04-21 17:33:17.000000 spark_sql_to_sqlite-0.2/spark_sql_to_sqlite.egg-info/PKG-INFO
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      232 2023-04-21 17:33:17.000000 spark_sql_to_sqlite-0.2/spark_sql_to_sqlite.egg-info/SOURCES.txt
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        1 2023-04-21 17:33:17.000000 spark_sql_to_sqlite-0.2/spark_sql_to_sqlite.egg-info/dependency_links.txt
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       15 2023-04-21 17:33:17.000000 spark_sql_to_sqlite-0.2/spark_sql_to_sqlite.egg-info/requires.txt
--rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        1 2023-04-21 17:33:17.000000 spark_sql_to_sqlite-0.2/spark_sql_to_sqlite.egg-info/top_level.txt
+drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 18:51:07.785919 spark_sql_to_sqlite-0.3/
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      101 2023-04-21 18:51:07.785722 spark_sql_to_sqlite-0.3/PKG-INFO
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 17:30:26.000000 spark_sql_to_sqlite-0.3/README.md
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       38 2023-04-21 18:51:07.785970 spark_sql_to_sqlite-0.3/setup.cfg
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      484 2023-04-21 18:49:54.000000 spark_sql_to_sqlite-0.3/setup.py
+drwxr-xr-x   0 vijay.balasubramaniam   (502) staff       (20)        0 2023-04-21 18:51:07.785414 spark_sql_to_sqlite-0.3/spark_sql_to_sqlite.egg-info/
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      101 2023-04-21 18:51:07.000000 spark_sql_to_sqlite-0.3/spark_sql_to_sqlite.egg-info/PKG-INFO
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)      232 2023-04-21 18:51:07.000000 spark_sql_to_sqlite-0.3/spark_sql_to_sqlite.egg-info/SOURCES.txt
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        1 2023-04-21 18:51:07.000000 spark_sql_to_sqlite-0.3/spark_sql_to_sqlite.egg-info/dependency_links.txt
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)       15 2023-04-21 18:51:07.000000 spark_sql_to_sqlite-0.3/spark_sql_to_sqlite.egg-info/requires.txt
+-rw-r--r--   0 vijay.balasubramaniam   (502) staff       (20)        1 2023-04-21 18:51:07.000000 spark_sql_to_sqlite-0.3/spark_sql_to_sqlite.egg-info/top_level.txt
```

