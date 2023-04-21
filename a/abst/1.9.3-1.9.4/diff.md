# Comparing `tmp/abst-1.9.3.tar.gz` & `tmp/abst-1.9.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "abst-1.9.3.tar", last modified: Tue Apr 18 09:12:10 2023, max compression
+gzip compressed data, was "abst-1.9.4.tar", last modified: Fri Apr 21 10:23:37 2023, max compression
```

## Comparing `abst-1.9.3.tar` & `abst-1.9.4.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/
--rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-18 09:11:55.000000 abst-1.9.3/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-18 09:12:10.216003 abst-1.9.3/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-18 09:11:55.000000 abst-1.9.3/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.212002 abst-1.9.3/abst/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:11:55.000000 abst-1.9.3/abst/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-18 09:11:55.000000 abst-1.9.3/abst/__version__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/abst/bastion_support/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:11:55.000000 abst-1.9.3/abst/bastion_support/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-18 09:11:55.000000 abst-1.9.3/abst/bastion_support/bastion_scheduler.py
--rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-04-18 09:11:55.000000 abst-1.9.3/abst/bastion_support/oci_bastion.py
--rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-18 09:11:55.000000 abst-1.9.3/abst/cfg_func.py
--rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-18 09:11:55.000000 abst-1.9.3/abst/config.py
--rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-18 09:11:55.000000 abst-1.9.3/abst/dialogs.py
--rw-r--r--   0 runner    (1001) docker     (123)    17420 2023-04-18 09:11:55.000000 abst-1.9.3/abst/main.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/abst/notifier/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 09:11:55.000000 abst-1.9.3/abst/notifier/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-18 09:11:55.000000 abst-1.9.3/abst/notifier/version_notifier.py
--rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-18 09:11:55.000000 abst-1.9.3/abst/tools.py
--rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-18 09:11:55.000000 abst-1.9.3/abst/wrappers.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/abst.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 09:12:10.000000 abst-1.9.3/abst.egg-info/zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 09:12:10.216003 abst-1.9.3/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-18 09:11:55.000000 abst-1.9.3/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 09:12:10.216003 abst-1.9.3/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-18 09:11:55.000000 abst-1.9.3/tests/test_sample_dict.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/
+-rw-r--r--   0 runner    (1001) docker     (123)     1069 2023-04-21 10:23:25.000000 abst-1.9.4/LICENSE.md
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-21 10:23:37.115653 abst-1.9.4/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     3920 2023-04-21 10:23:25.000000 abst-1.9.4/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/abst/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:25.000000 abst-1.9.4/abst/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      493 2023-04-21 10:23:25.000000 abst-1.9.4/abst/__version__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/abst/bastion_support/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:25.000000 abst-1.9.4/abst/bastion_support/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5674 2023-04-21 10:23:25.000000 abst-1.9.4/abst/bastion_support/bastion_scheduler.py
+-rw-r--r--   0 runner    (1001) docker     (123)    22731 2023-04-21 10:23:25.000000 abst-1.9.4/abst/bastion_support/oci_bastion.py
+-rw-r--r--   0 runner    (1001) docker     (123)      757 2023-04-21 10:23:25.000000 abst-1.9.4/abst/cfg_func.py
+-rw-r--r--   0 runner    (1001) docker     (123)      761 2023-04-21 10:23:25.000000 abst-1.9.4/abst/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      519 2023-04-21 10:23:25.000000 abst-1.9.4/abst/dialogs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    17526 2023-04-21 10:23:25.000000 abst-1.9.4/abst/main.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/abst/notifier/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:25.000000 abst-1.9.4/abst/notifier/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1679 2023-04-21 10:23:25.000000 abst-1.9.4/abst/notifier/version_notifier.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1219 2023-04-21 10:23:25.000000 abst-1.9.4/abst/tools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      775 2023-04-21 10:23:25.000000 abst-1.9.4/abst/wrappers.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/abst.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4648 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      548 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       40 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 10:23:37.000000 abst-1.9.4/abst.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:23:36.000000 abst-1.9.4/abst.egg-info/zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:23:37.115653 abst-1.9.4/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1512 2023-04-21 10:23:25.000000 abst-1.9.4/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:23:37.115653 abst-1.9.4/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-21 10:23:25.000000 abst-1.9.4/tests/test_sample_dict.py
```

### Comparing `abst-1.9.3/LICENSE.md` & `abst-1.9.4/LICENSE.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/PKG-INFO` & `abst-1.9.4/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.3
+Version: 1.9.4
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.3/README.md` & `abst-1.9.4/README.md`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/abst/bastion_support/bastion_scheduler.py` & `abst-1.9.4/abst/bastion_support/bastion_scheduler.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/abst/bastion_support/oci_bastion.py` & `abst-1.9.4/abst/bastion_support/oci_bastion.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/abst/cfg_func.py` & `abst-1.9.4/abst/cfg_func.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/abst/config.py` & `abst-1.9.4/abst/config.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/abst/dialogs.py` & `abst-1.9.4/abst/dialogs.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/abst/main.py` & `abst-1.9.4/abst/main.py`

 * *Files 2% similar despite different names*

```diff
@@ -68,27 +68,29 @@
     setup_calls(debug)
     BastionScheduler.remove_bastion(context_name)
     display_scheduled()
 
 
 @parallel.command("run", help="Run All Bastions in fullauto")
 @click.option("--debug", is_flag=True, default=False)
-def run(debug):
+@click.option("-y", is_flag=True, default=False)
+def run(debug, y):
     setup_calls(debug)
     display_scheduled()
-    try:
-        confirm = inquirer.confirm(
-            "Do you really want to run following contexts?"
-        ).execute()
-    except KeyError:
-        rich.print("Unknown inquirer error, continuing...")
-        confirm = True
-    if not confirm:
-        rich.print("[green]Cancelling, nothing started[/green]")
-        exit(0)
+    if not y:
+        try:
+            confirm = inquirer.confirm(
+                "Do you really want to run following contexts?"
+            ).execute()
+        except KeyError:
+            rich.print("Unknown inquirer error, continuing...")
+            confirm = True
+        if not confirm:
+            rich.print("[green]Cancelling, nothing started[/green]")
+            exit(0)
     BastionScheduler.run()
 
 
 @parallel.command("display", help="Display current Bastions is stack")
 @click.option("--debug", is_flag=True, default=False)
 def display(debug):
     setup_calls(debug)
```

### Comparing `abst-1.9.3/abst/notifier/version_notifier.py` & `abst-1.9.4/abst/notifier/version_notifier.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/abst/tools.py` & `abst-1.9.4/abst/tools.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/abst/wrappers.py` & `abst-1.9.4/abst/wrappers.py`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/abst.egg-info/PKG-INFO` & `abst-1.9.4/abst.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: abst
-Version: 1.9.3
+Version: 1.9.4
 Summary: CLI Command making OCI Bastion and kubernetes usage simple and fast
 Home-page: https://github.com/jiri-otoupal/abst
 Author: Jiri Otoupal
 Author-email: jiri-otoupal@ips-database.eu
 License: MIT
 Keywords: Auto OCI Bastion
 Classifier: Development Status :: 4 - Beta
```

### Comparing `abst-1.9.3/abst.egg-info/SOURCES.txt` & `abst-1.9.4/abst.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `abst-1.9.3/setup.py` & `abst-1.9.4/setup.py`

 * *Files identical despite different names*

