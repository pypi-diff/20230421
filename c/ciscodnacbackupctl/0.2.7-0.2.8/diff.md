# Comparing `tmp/ciscodnacbackupctl-0.2.7.tar.gz` & `tmp/ciscodnacbackupctl-0.2.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ciscodnacbackupctl-0.2.7.tar", last modified: Tue Jan  4 08:51:37 2022, max compression
+gzip compressed data, was "ciscodnacbackupctl-0.2.8.tar", last modified: Wed Mar 16 13:16:55 2022, max compression
```

## Comparing `ciscodnacbackupctl-0.2.7.tar` & `ciscodnacbackupctl-0.2.8.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-01-04 08:51:37.798177 ciscodnacbackupctl-0.2.7/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3326 2022-01-04 08:51:37.798177 ciscodnacbackupctl-0.2.7/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2221 2022-01-04 07:44:33.000000 ciscodnacbackupctl-0.2.7/README.md
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-01-04 08:51:37.798177 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20137 2022-01-04 08:43:47.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl/__init__.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9961 2022-01-04 07:44:33.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl/cli.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5412 2022-01-04 07:44:33.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl/config.py
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4373 2022-01-04 07:44:33.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl/format.py
-drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-01-04 08:51:37.798177 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl.egg-info/
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3326 2022-01-04 08:51:37.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl.egg-info/PKG-INFO
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      387 2022-01-04 08:51:37.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl.egg-info/SOURCES.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2022-01-04 08:51:37.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl.egg-info/dependency_links.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       85 2022-01-04 08:51:37.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl.egg-info/entry_points.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       75 2022-01-04 08:51:37.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl.egg-info/requires.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2022-01-04 08:51:37.000000 ciscodnacbackupctl-0.2.7/ciscodnacbackupctl.egg-info/top_level.txt
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2022-01-04 08:51:37.798177 ciscodnacbackupctl-0.2.7/setup.cfg
--rw-rw-rw-   0 codespace  (1000) codespace  (1000)      883 2022-01-04 08:43:30.000000 ciscodnacbackupctl-0.2.7/setup.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-03-16 13:16:55.110193 ciscodnacbackupctl-0.2.8/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3326 2022-03-16 13:16:55.110193 ciscodnacbackupctl-0.2.8/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     2221 2022-03-16 12:50:39.000000 ciscodnacbackupctl-0.2.8/README.md
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-03-16 13:16:55.106193 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)    20137 2022-03-16 13:13:08.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl/__init__.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     9961 2022-03-16 13:11:37.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl/cli.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     5412 2022-03-16 12:50:39.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl/config.py
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     4373 2022-03-16 12:50:39.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl/format.py
+drwxrwxrwx   0 codespace  (1000) codespace  (1000)        0 2022-03-16 13:16:55.110193 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl.egg-info/
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)     3326 2022-03-16 13:16:54.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl.egg-info/PKG-INFO
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      387 2022-03-16 13:16:54.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl.egg-info/SOURCES.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)        1 2022-03-16 13:16:54.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl.egg-info/dependency_links.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       85 2022-03-16 13:16:54.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl.egg-info/entry_points.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       75 2022-03-16 13:16:54.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl.egg-info/requires.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       19 2022-03-16 13:16:54.000000 ciscodnacbackupctl-0.2.8/ciscodnacbackupctl.egg-info/top_level.txt
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)       38 2022-03-16 13:16:55.110193 ciscodnacbackupctl-0.2.8/setup.cfg
+-rw-rw-rw-   0 codespace  (1000) codespace  (1000)      883 2022-03-16 12:50:39.000000 ciscodnacbackupctl-0.2.8/setup.py
```

### Comparing `ciscodnacbackupctl-0.2.7/PKG-INFO` & `ciscodnacbackupctl-0.2.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscodnacbackupctl
-Version: 0.2.7
+Version: 0.2.8
 Summary: Cisco DNA Center Backup CLI
 Home-page: https://github.com/cskoglun/ciscodnacbackupctl
 Author: Robert Csapo
 Author-email: rcsapo@cisco.com
 License: UNKNOWN
 Description: # ciscodnacbackupctl
```

### Comparing `ciscodnacbackupctl-0.2.7/README.md` & `ciscodnacbackupctl-0.2.8/README.md`

 * *Files identical despite different names*

### Comparing `ciscodnacbackupctl-0.2.7/ciscodnacbackupctl/__init__.py` & `ciscodnacbackupctl-0.2.8/ciscodnacbackupctl/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -14,15 +14,15 @@
 
 author = "Robert Csapo"
 email = "rcsapo@cisco.com"
 description = "Cisco DNA Center Backup CLI"
 repo_url = "https://github.com/cskoglun/ciscodnacbackupctl"
 copyright = "Copyright (c) 2020 Cisco and/or its affiliates."
 license = "Cisco Sample Code License, Version 1.1"
-version = "0.2.7"
+version = "0.2.8"
 
 
 class Api:
     def __init__(self, config=False):
         """
         Create client session
         Checking config (env/local file)
```

### Comparing `ciscodnacbackupctl-0.2.7/ciscodnacbackupctl/cli.py` & `ciscodnacbackupctl-0.2.8/ciscodnacbackupctl/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -26,15 +26,15 @@
 
     def job():
         console = Console()
         ctl = ciscodnacbackupctl.Api()
         cli = ctl.CLI()
         force = True
         try:
-            purge = cli.purge(keep=keep, incompatible=incompatible, force=force)
+            purge = cli.purge(keep=KEEP, incompatible=incompatible, force=force)
         except Exception as error_msg:
             console.print(
                 "Cisco DNA Center isn't available - {}".format(error_msg), style="green"
             )
             pass
 
     schedule_function = ctl.schedule_interval(
```

### Comparing `ciscodnacbackupctl-0.2.7/ciscodnacbackupctl/config.py` & `ciscodnacbackupctl-0.2.8/ciscodnacbackupctl/config.py`

 * *Files identical despite different names*

### Comparing `ciscodnacbackupctl-0.2.7/ciscodnacbackupctl/format.py` & `ciscodnacbackupctl-0.2.8/ciscodnacbackupctl/format.py`

 * *Files identical despite different names*

### Comparing `ciscodnacbackupctl-0.2.7/ciscodnacbackupctl.egg-info/PKG-INFO` & `ciscodnacbackupctl-0.2.8/ciscodnacbackupctl.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ciscodnacbackupctl
-Version: 0.2.7
+Version: 0.2.8
 Summary: Cisco DNA Center Backup CLI
 Home-page: https://github.com/cskoglun/ciscodnacbackupctl
 Author: Robert Csapo
 Author-email: rcsapo@cisco.com
 License: UNKNOWN
 Description: # ciscodnacbackupctl
```

### Comparing `ciscodnacbackupctl-0.2.7/setup.py` & `ciscodnacbackupctl-0.2.8/setup.py`

 * *Files identical despite different names*

