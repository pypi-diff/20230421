# Comparing `tmp/tokmon-0.1.2.tar.gz` & `tmp/tokmon-0.1.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "tokmon-0.1.2.tar", last modified: Thu Apr 20 15:48:32 2023, max compression
+gzip compressed data, was "tokmon-0.1.3.tar", last modified: Thu Apr 20 16:48:47 2023, max compression
```

## Comparing `tokmon-0.1.2.tar` & `tokmon-0.1.3.tar`

### file list

```diff
@@ -1,19 +1,19 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:48:32.731674 tokmon-0.1.2/
--rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-04-20 15:48:22.000000 tokmon-0.1.2/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-20 15:48:32.731674 tokmon-0.1.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-20 15:48:22.000000 tokmon-0.1.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 15:48:32.731674 tokmon-0.1.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      624 2023-04-20 15:48:32.000000 tokmon-0.1.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:48:32.731674 tokmon-0.1.2/tokmon/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/__init__.py
--rwxr-xr-x   0 runner    (1001) docker     (123)     4777 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/costcalculator.py
--rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/pricing.json
--rwxr-xr-x   0 runner    (1001) docker     (123)     9244 2023-04-20 15:48:22.000000 tokmon-0.1.2/tokmon/tokmon.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 15:48:32.731674 tokmon-0.1.2/tokmon.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     6794 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 15:48:32.000000 tokmon-0.1.2/tokmon.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:48:47.124557 tokmon-0.1.3/
+-rw-r--r--   0 runner    (1001) docker     (123)    11336 2023-04-20 16:48:34.000000 tokmon-0.1.3/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-20 16:48:47.124557 tokmon-0.1.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     6681 2023-04-20 16:48:34.000000 tokmon-0.1.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 16:48:47.124557 tokmon-0.1.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-20 16:48:34.000000 tokmon-0.1.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:48:47.124557 tokmon-0.1.3/tokmon/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-20 16:48:34.000000 tokmon-0.1.3/tokmon/__init__.py
+-rwxr-xr-x   0 runner    (1001) docker     (123)     4777 2023-04-20 16:48:34.000000 tokmon-0.1.3/tokmon/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3370 2023-04-20 16:48:34.000000 tokmon-0.1.3/tokmon/costcalculator.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1021 2023-04-20 16:48:34.000000 tokmon-0.1.3/tokmon/pricing.json
+-rwxr-xr-x   0 runner    (1001) docker     (123)     9244 2023-04-20 16:48:34.000000 tokmon-0.1.3/tokmon/tokmon.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 16:48:47.124557 tokmon-0.1.3/tokmon.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     7029 2023-04-20 16:48:47.000000 tokmon-0.1.3/tokmon.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      303 2023-04-20 16:48:47.000000 tokmon-0.1.3/tokmon.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 16:48:47.000000 tokmon-0.1.3/tokmon.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-20 16:48:47.000000 tokmon-0.1.3/tokmon.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       19 2023-04-20 16:48:47.000000 tokmon-0.1.3/tokmon.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-20 16:48:47.000000 tokmon-0.1.3/tokmon.egg-info/top_level.txt
```

### Comparing `tokmon-0.1.2/LICENSE` & `tokmon-0.1.3/LICENSE`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.2/PKG-INFO` & `tokmon-0.1.3/README.md`

 * *Files 2% similar despite different names*

```diff
@@ -1,13 +1,7 @@
-Metadata-Version: 2.1
-Name: tokmon
-Version: 0.1.2
-Description-Content-Type: text/markdown
-License-File: LICENSE
-
 # `tokmon` 🔤🧐 - CLI utility to monitor OpenAI token costs
 
 `tokmon` enables you to monitor your program's OpenAI API token usage.
 
 You use `tokmon` just like you would use the `time` utility, but instead of execution time you get token usage and cost.
 <p align="center">
     <img src="https://user-images.githubusercontent.com/3611042/231910274-3872e13f-d9e6-4752-bc89-44e5d334e21f.gif" />
```

### Comparing `tokmon-0.1.2/README.md` & `tokmon-0.1.3/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,7 +1,17 @@
+Metadata-Version: 2.1
+Name: tokmon
+Version: 0.1.3
+Summary: tokmon is a CLI utility to monitor OpenAI token usage and costs
+Home-page: https://github.com/yagil/tokmon
+Project-URL: Bug Reports, https://github.com/yagil/tokmon/issues
+Project-URL: Source, https://github.com/yagil/tokmon/
+Description-Content-Type: text/markdown
+License-File: LICENSE
+
 # `tokmon` 🔤🧐 - CLI utility to monitor OpenAI token costs
 
 `tokmon` enables you to monitor your program's OpenAI API token usage.
 
 You use `tokmon` just like you would use the `time` utility, but instead of execution time you get token usage and cost.
 <p align="center">
     <img src="https://user-images.githubusercontent.com/3611042/231910274-3872e13f-d9e6-4752-bc89-44e5d334e21f.gif" />
```

### Comparing `tokmon-0.1.2/tokmon/cli.py` & `tokmon-0.1.3/tokmon/cli.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.2/tokmon/costcalculator.py` & `tokmon-0.1.3/tokmon/costcalculator.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.2/tokmon/pricing.json` & `tokmon-0.1.3/tokmon/pricing.json`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.2/tokmon/tokmon.py` & `tokmon-0.1.3/tokmon/tokmon.py`

 * *Files identical despite different names*

### Comparing `tokmon-0.1.2/tokmon.egg-info/PKG-INFO` & `tokmon-0.1.3/tokmon.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,14 @@
 Metadata-Version: 2.1
 Name: tokmon
-Version: 0.1.2
+Version: 0.1.3
+Summary: tokmon is a CLI utility to monitor OpenAI token usage and costs
+Home-page: https://github.com/yagil/tokmon
+Project-URL: Bug Reports, https://github.com/yagil/tokmon/issues
+Project-URL: Source, https://github.com/yagil/tokmon/
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # `tokmon` 🔤🧐 - CLI utility to monitor OpenAI token costs
 
 `tokmon` enables you to monitor your program's OpenAI API token usage.
```

