# Comparing `tmp/checkontap-0.1a2.tar.gz` & `tmp/checkontap-0.1a3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkontap-0.1a2.tar", last modified: Tue Apr 11 08:45:43 2023, max compression
+gzip compressed data, was "checkontap-0.1a3.tar", last modified: Fri Apr 21 14:52:04 2023, max compression
```

## Comparing `checkontap-0.1a2.tar` & `checkontap-0.1a3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
--rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a2/README.md
--rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a2/checkontap/__init__.py
--rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a2/checkontap/cli.py
--rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a2/checkontap/ontapcmd/__init__.py
--rw-r--r--   0        0        0     2239 2023-03-23 10:23:29.838743 checkontap-0.1a2/checkontap/ontapcmd/about.py
--rw-r--r--   0        0        0     6957 2023-04-11 08:29:43.568792 checkontap-0.1a2/checkontap/ontapcmd/aggregateusage.py
--rw-r--r--   0        0        0     2906 2023-03-23 10:24:18.101957 checkontap-0.1a2/checkontap/ontapcmd/clusterhealth.py
--rw-r--r--   0        0        0     7706 2023-03-23 10:34:24.107947 checkontap-0.1a2/checkontap/ontapcmd/diskhealth.py
--rw-r--r--   0        0        0     4521 2023-03-23 10:34:56.095206 checkontap-0.1a2/checkontap/ontapcmd/hardwarehealth.py
--rw-r--r--   0        0        0     3848 2023-03-23 15:56:05.462390 checkontap-0.1a2/checkontap/ontapcmd/interfacehealth.py
--rw-r--r--   0        0        0     5006 2023-04-11 08:31:25.465579 checkontap-0.1a2/checkontap/ontapcmd/lunusage.py
--rw-r--r--   0        0        0     5091 2023-03-23 10:31:27.440904 checkontap-0.1a2/checkontap/ontapcmd/volumehealth.py
--rw-r--r--   0        0        0     6634 2023-04-11 08:32:37.797398 checkontap-0.1a2/checkontap/ontapcmd/volumeusage.py
--rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a2/checkontap/tools/__init__.py
--rw-r--r--   0        0        0     8774 2023-03-15 10:17:40.434320 checkontap-0.1a2/checkontap/tools/cli.py
--rw-r--r--   0        0        0     2986 2023-03-23 10:28:55.299455 checkontap-0.1a2/checkontap/tools/helper.py
--rw-r--r--   0        0        0      857 2023-04-11 08:40:22.079330 checkontap-0.1a2/pyproject.toml
--rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a2/PKG-INFO
+-rw-r--r--   0        0        0      223 2023-03-23 09:02:45.881436 checkontap-0.1a3/README.md
+-rw-r--r--   0        0        0      926 2023-03-22 16:30:38.341339 checkontap-0.1a3/checkontap/__init__.py
+-rw-r--r--   0        0        0     3431 2023-03-23 14:53:12.575066 checkontap-0.1a3/checkontap/cli.py
+-rw-r--r--   0        0        0      756 2023-03-22 16:09:15.025609 checkontap-0.1a3/checkontap/ontapcmd/__init__.py
+-rw-r--r--   0        0        0     2227 2023-04-21 14:48:25.623996 checkontap-0.1a3/checkontap/ontapcmd/about.py
+-rw-r--r--   0        0        0     6945 2023-04-21 14:48:51.992608 checkontap-0.1a3/checkontap/ontapcmd/aggregateusage.py
+-rw-r--r--   0        0        0     2894 2023-04-21 14:49:01.363591 checkontap-0.1a3/checkontap/ontapcmd/clusterhealth.py
+-rw-r--r--   0        0        0     7694 2023-04-21 14:49:13.743682 checkontap-0.1a3/checkontap/ontapcmd/diskhealth.py
+-rw-r--r--   0        0        0     4509 2023-04-21 14:49:23.573489 checkontap-0.1a3/checkontap/ontapcmd/hardwarehealth.py
+-rw-r--r--   0        0        0     3836 2023-04-21 14:49:37.766604 checkontap-0.1a3/checkontap/ontapcmd/interfacehealth.py
+-rw-r--r--   0        0        0     4994 2023-04-21 14:49:47.394778 checkontap-0.1a3/checkontap/ontapcmd/lunusage.py
+-rw-r--r--   0        0        0     5079 2023-04-21 14:49:57.522947 checkontap-0.1a3/checkontap/ontapcmd/volumehealth.py
+-rw-r--r--   0        0        0     8126 2023-04-21 14:48:07.213286 checkontap-0.1a3/checkontap/ontapcmd/volumeusage.py
+-rw-r--r--   0        0        0      757 2023-03-22 16:09:25.201105 checkontap-0.1a3/checkontap/tools/__init__.py
+-rw-r--r--   0        0        0     9543 2023-04-21 14:46:55.901090 checkontap-0.1a3/checkontap/tools/cli.py
+-rw-r--r--   0        0        0     2986 2023-03-23 10:28:55.299455 checkontap-0.1a3/checkontap/tools/helper.py
+-rw-r--r--   0        0        0      857 2023-04-21 14:51:14.599000 checkontap-0.1a3/pyproject.toml
+-rw-r--r--   0        0        0      893 1970-01-01 00:00:00.000000 checkontap-0.1a3/PKG-INFO
```

### Comparing `checkontap-0.1a2/checkontap/__init__.py` & `checkontap-0.1a3/checkontap/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a2/checkontap/cli.py` & `checkontap-0.1a3/checkontap/cli.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a2/checkontap/ontapcmd/__init__.py` & `checkontap-0.1a3/checkontap/ontapcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a2/checkontap/ontapcmd/about.py` & `checkontap-0.1a3/checkontap/ontapcmd/about.py`

 * *Files 2% similar despite different names*

```diff
@@ -39,15 +39,15 @@
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
     setup_connection(args.host, args.api_user, args.api_pass)
     
-    check = Check(shortname="")
+    check = Check()
     # About overview module
     try:
         software = Software()
         software.get(fields='version')
         logger.debug(f"Software info \n{software.__dict__}")
         check.add_message(Status.OK,f"current version id {software['version']}")
     except NetAppRestError as error:
```

### Comparing `checkontap-0.1a2/checkontap/ontapcmd/aggregateusage.py` & `checkontap-0.1a3/checkontap/ontapcmd/aggregateusage.py`

 * *Files 1% similar despite different names*

```diff
@@ -80,15 +80,15 @@
     logger = logging.getLogger(__name__)
     logger.disabled = True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
-    check = Check(shortname="")
+    check = Check()
 
     check.set_threshold(
         warning=args.warning,
         critical=args.critical
     )
 
     setup_connection(args.host, args.api_user, args.api_pass)
```

### Comparing `checkontap-0.1a2/checkontap/ontapcmd/clusterhealth.py` & `checkontap-0.1a3/checkontap/ontapcmd/clusterhealth.py`

 * *Files 2% similar despite different names*

```diff
@@ -35,15 +35,15 @@
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
     setup_connection(args.host, args.api_user, args.api_pass)
     
-    check = Check(shortname="")
+    check = Check()
     # Cluster global state
     try:
         cluster = Cluster()
         cluster.get(fields="name,metric,version")
         logger.debug(f"Cluster info \n{cluster.__dict__}")
         if 'ok' in cluster.metric.status:
             check.add_message(Status.OK, "{}".format(cluster.version.full))
```

### Comparing `checkontap-0.1a2/checkontap/ontapcmd/diskhealth.py` & `checkontap-0.1a3/checkontap/ontapcmd/diskhealth.py`

 * *Files 1% similar despite different names*

```diff
@@ -84,15 +84,15 @@
     logger = logging.getLogger(__name__)
     logger.disabled = True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
-    check = Check(shortname="")
+    check = Check()
     
     setup_connection(args.host, args.api_user, args.api_pass)
     
     try:
         software = Software()
         software.get(fields='version')
         disk_count = Disk.count_collection()
```

### Comparing `checkontap-0.1a2/checkontap/ontapcmd/hardwarehealth.py` & `checkontap-0.1a3/checkontap/ontapcmd/hardwarehealth.py`

 * *Files 1% similar despite different names*

```diff
@@ -47,15 +47,15 @@
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
     setup_connection(args.host, args.api_user, args.api_pass)
     
-    check = Check(shortname="")
+    check = Check()
     """
     [-type {fan|thermal|voltage|current|battery-life|discrete|fru|nvmem|counter|minutes|percent|agent|unknown}] - Sensor Type
     [-state {normal|warn-low|warn-high|crit-low|crit-high|disabled|uninitialized|init-failed|not-available|invalid|retry|bad|not-present|failed|ignored|fault|unknown}]
     """
     if not args.type:
         sType = ['fan','thermal','voltage','current','battery-life','discrete','fru','nvmem','counter','minutes','percent','agent']
     else:
```

### Comparing `checkontap-0.1a2/checkontap/ontapcmd/interfacehealth.py` & `checkontap-0.1a3/checkontap/ontapcmd/interfacehealth.py`

 * *Files 2% similar despite different names*

```diff
@@ -60,15 +60,15 @@
     logger = logging.getLogger(__name__)
     logger.disabled = True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
-    check = Check(shortname="")
+    check = Check()
 
     setup_connection(args.host, args.api_user, args.api_pass)
 
     IpInts = []
     try:
         interface_count = IpInterface.count_collection()
         logger.info(f"found {interface_count} volumes")
```

### Comparing `checkontap-0.1a2/checkontap/ontapcmd/lunusage.py` & `checkontap-0.1a3/checkontap/ontapcmd/lunusage.py`

 * *Files 1% similar despite different names*

```diff
@@ -40,15 +40,15 @@
     logger = logging.getLogger(__name__)
     logger.disabled = True
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
-    check = Check(shortname="")
+    check = Check()
 
     check.set_threshold(
         warning=args.warning,
         critical=args.critical,
     )
     
     setup_connection(args.host, args.api_user, args.api_pass)
```

### Comparing `checkontap-0.1a2/checkontap/ontapcmd/volumehealth.py` & `checkontap-0.1a3/checkontap/ontapcmd/volumehealth.py`

 * *Files 2% similar despite different names*

```diff
@@ -71,15 +71,15 @@
     if args.verbose:
         for log_name, log_obj in logging.Logger.manager.loggerDict.items():
             log_obj.disabled = False
             logging.getLogger(log_name).setLevel(severity(args.verbose))
 
     setup_connection(args.host, args.api_user, args.api_pass)
 
-    check = Check(shortname="")
+    check = Check()
 
     try:
         volumes_count = Volume.count_collection()
         logger.info(f"found {volumes_count} volumes")
         if volumes_count == 0:
             check.exit(Status.UNKNOWN, "no vols found")
```

### Comparing `checkontap-0.1a2/checkontap/tools/__init__.py` & `checkontap-0.1a3/checkontap/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a2/checkontap/tools/cli.py` & `checkontap-0.1a3/checkontap/tools/cli.py`

 * *Files 13% similar despite different names*

```diff
@@ -220,8 +220,35 @@
         'name_or_flags': ['--perfdata'],
         'options': {
             'action': 'store_true',
             'required': 'false',
             'help': 'add performance data to Output',
         }
     }
-    
+    INODE_WARN = {
+        'name_or_flags': ['--inode-warning'],
+        'options': {
+            'action': 'store',
+            'help': 'Inode warning threshold in %'
+        }
+    }
+    INODE_CRIT = {
+        'name_or_flags': ['--inode-critical'],
+        'options': {
+            'action': 'store',
+            'help': 'Inode critical threshold in %',
+        }
+    }
+    SNAP_WARN = {
+        'name_or_flags': ['--snapshot-warning'],
+        'options': {
+            'action': 'store',
+            'help': 'Snapshot used space warning threshold in %'
+        }
+    }
+    SNAP_CRIT = {
+        'name_or_flags': ['--snapshot-critical'],
+        'options': {
+            'action': 'store',
+            'help': 'Snapshot used space critical threshold in %',
+        }
+    }
```

### Comparing `checkontap-0.1a2/checkontap/tools/helper.py` & `checkontap-0.1a3/checkontap/tools/helper.py`

 * *Files identical despite different names*

### Comparing `checkontap-0.1a2/pyproject.toml` & `checkontap-0.1a3/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkontap"
 readme = "README.md"
 description = "check_ontap monitoring plugin"
-version = "0.1a2"
+version = "0.1a3"
 requires-python = ">= 3.6"
 authors = [
     { name = "Matthias Gallinger", email = "matthias.gallinger@consol.de" }
 ]
 dependencies = [
     "netapp-ontap >= 9.11.1.0",
     "monplugin >= 0.5",
```

### Comparing `checkontap-0.1a2/PKG-INFO` & `checkontap-0.1a3/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: checkontap
-Version: 0.1a2
+Version: 0.1a3
 Summary: check_ontap monitoring plugin
 Author-email: Matthias Gallinger <matthias.gallinger@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
```

