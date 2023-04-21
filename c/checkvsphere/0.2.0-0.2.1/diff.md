# Comparing `tmp/checkvsphere-0.2.0.tar.gz` & `tmp/checkvsphere-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "checkvsphere-0.2.0.tar", last modified: Mon Apr 17 12:59:03 2023, max compression
+gzip compressed data, was "checkvsphere-0.2.1.tar", last modified: Fri Apr 21 14:20:19 2023, max compression
```

## Comparing `checkvsphere-0.2.0.tar` & `checkvsphere-0.2.1.tar`

### file list

```diff
@@ -1,23 +1,23 @@
--rw-r--r--   0        0        0      264 2023-04-04 13:33:00.767834 checkvsphere-0.2.0/README.md
--rw-r--r--   0        0        0      174 2023-04-04 13:33:00.791833 checkvsphere-0.2.0/checkvsphere/__init__.py
--rw-r--r--   0        0        0     3882 2023-04-04 13:33:00.807833 checkvsphere-0.2.0/checkvsphere/cli.py
--rw-r--r--   0        0        0      760 2023-04-04 13:33:00.819833 checkvsphere-0.2.0/checkvsphere/tools/__init__.py
--rw-r--r--   0        0        0    16614 2023-04-04 13:33:00.827833 checkvsphere-0.2.0/checkvsphere/tools/cli.py
--rw-r--r--   0        0        0     6363 2023-04-06 12:14:26.650417 checkvsphere-0.2.0/checkvsphere/tools/helper.py
--rw-r--r--   0        0        0     5200 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/tools/pchelper.py
--rw-r--r--   0        0        0     2183 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/tools/service_instance.py
--rw-r--r--   0        0        0     4153 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/tools/serviceutil.py
--rw-r--r--   0        0        0      760 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/vcmd/__init__.py
--rw-r--r--   0        0        0     1887 2023-04-04 13:33:00.835833 checkvsphere-0.2.0/checkvsphere/vcmd/about.py
--rw-r--r--   0        0        0     6534 2023-04-05 13:00:59.351204 checkvsphere-0.2.0/checkvsphere/vcmd/datastores.py
--rw-r--r--   0        0        0     4520 2023-04-04 13:33:00.863832 checkvsphere-0.2.0/checkvsphere/vcmd/hostnic.py
--rw-r--r--   0        0        0    10749 2023-04-04 13:33:00.879832 checkvsphere-0.2.0/checkvsphere/vcmd/hostruntime.py
--rw-r--r--   0        0        0     4065 2023-04-04 13:33:00.891832 checkvsphere-0.2.0/checkvsphere/vcmd/hostservice.py
--rw-r--r--   0        0        0     7660 2023-04-04 13:33:00.895832 checkvsphere-0.2.0/checkvsphere/vcmd/hoststorage.py
--rw-r--r--   0        0        0     2039 2023-04-04 13:33:00.907831 checkvsphere-0.2.0/checkvsphere/vcmd/listmetrics.py
--rw-r--r--   0        0        0     3366 2023-04-04 13:33:00.915831 checkvsphere-0.2.0/checkvsphere/vcmd/media.py
--rw-r--r--   0        0        0     8332 2023-04-05 13:30:02.707750 checkvsphere-0.2.0/checkvsphere/vcmd/perf.py
--rw-r--r--   0        0        0     4958 2023-04-04 13:33:00.939831 checkvsphere-0.2.0/checkvsphere/vcmd/snapshots.py
--rw-r--r--   0        0        0     8969 2023-04-06 12:26:23.457744 checkvsphere-0.2.0/checkvsphere/vcmd/vsan.py
--rw-r--r--   0        0        0      941 2023-04-17 12:58:29.769761 checkvsphere-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     1002 1970-01-01 00:00:00.000000 checkvsphere-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0      275 2023-04-21 14:16:49.947749 checkvsphere-0.2.1/README.md
+-rw-r--r--   0        0        0      174 2023-04-21 14:16:49.947749 checkvsphere-0.2.1/checkvsphere/__init__.py
+-rw-r--r--   0        0        0     3882 2023-04-21 14:16:49.959749 checkvsphere-0.2.1/checkvsphere/cli.py
+-rw-r--r--   0        0        0      760 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/__init__.py
+-rw-r--r--   0        0        0    16614 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/cli.py
+-rw-r--r--   0        0        0     6363 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/helper.py
+-rw-r--r--   0        0        0     5200 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/pchelper.py
+-rw-r--r--   0        0        0     2183 2023-04-21 14:16:49.971748 checkvsphere-0.2.1/checkvsphere/tools/service_instance.py
+-rw-r--r--   0        0        0     4153 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/tools/serviceutil.py
+-rw-r--r--   0        0        0      760 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/__init__.py
+-rw-r--r--   0        0        0     1819 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/about.py
+-rw-r--r--   0        0        0     6509 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/datastores.py
+-rw-r--r--   0        0        0     4497 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/hostnic.py
+-rw-r--r--   0        0        0    10722 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/hostruntime.py
+-rw-r--r--   0        0        0     4038 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/hostservice.py
+-rw-r--r--   0        0        0     7633 2023-04-21 14:16:49.975748 checkvsphere-0.2.1/checkvsphere/vcmd/hoststorage.py
+-rw-r--r--   0        0        0     2039 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/listmetrics.py
+-rw-r--r--   0        0        0     3341 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/media.py
+-rw-r--r--   0        0        0     8301 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/perf.py
+-rw-r--r--   0        0        0     4929 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/snapshots.py
+-rw-r--r--   0        0        0     8945 2023-04-21 14:16:49.983748 checkvsphere-0.2.1/checkvsphere/vcmd/vsan.py
+-rw-r--r--   0        0        0      941 2023-04-21 14:16:49.987748 checkvsphere-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     1013 1970-01-01 00:00:00.000000 checkvsphere-0.2.1/PKG-INFO
```

### Comparing `checkvsphere-0.2.0/checkvsphere/cli.py` & `checkvsphere-0.2.1/checkvsphere/cli.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.0/checkvsphere/tools/__init__.py` & `checkvsphere-0.2.1/checkvsphere/tools/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.0/checkvsphere/tools/cli.py` & `checkvsphere-0.2.1/checkvsphere/tools/cli.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.0/checkvsphere/tools/helper.py` & `checkvsphere-0.2.1/checkvsphere/tools/helper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.0/checkvsphere/tools/pchelper.py` & `checkvsphere-0.2.1/checkvsphere/tools/pchelper.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.0/checkvsphere/tools/service_instance.py` & `checkvsphere-0.2.1/checkvsphere/tools/service_instance.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.0/checkvsphere/tools/serviceutil.py` & `checkvsphere-0.2.1/checkvsphere/tools/serviceutil.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/__init__.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/__init__.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/about.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/about.py`

 * *Files 12% similar despite different names*

```diff
@@ -34,23 +34,23 @@
         parser = cli.Parser()
         # parser.add_optional_arguments(cli.Argument.DATACENTER_NAME)
         parser.add_optional_arguments(cli.Argument.VIHOST)
         args = parser.get_args()
         si = service_instance.connect(args)
         about = si.content.about
         print(
-            f'VSPHERE-ABOUT - OK - { about.fullName }, '
+            f'OK: { about.fullName }, '
             f'api: { about.apiType }/{ about.apiVersion }, '
             f'product: { about.licenseProductName } { about.licenseProductVersion }'
         )
     except vim.fault.VimFault as e:
         if hasattr(e, 'msg'):
-            print(f"VSPHERE-ABOUT - ERROR - {e.msg}")
+            print(f"ERROR: {e.msg}")
         else:
-            print(f"VSPHERE-ABOUT - ERROR - {e}")
+            print(f"ERROR: {e}")
         raise SystemExit(2)
     except Exception as e:
-        print(f"VSPHERE-ABOUT - ERROR - {e}")
+        print(f"ERROR: {e}")
         raise SystemExit(2)
 
 if __name__ == "__main__":
     run()
```

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/datastores.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/datastores.py`

 * *Files 5% similar despite different names*

```diff
@@ -91,15 +91,15 @@
                     'free and used are measured in bytes. You can one of these suffixes: '
                     'kB, MB, GB for example: free_MB or used_GB'
         }
     })
     args = parser.get_args()
 
     si = service_instance.connect(args)
-    check = Check(shortname='VSPHERE-VOL', threshold = Threshold(args.warning or None, args.critical or None))
+    check = Check(threshold = Threshold(args.warning or None, args.critical or None))
 
     vimtype = None
     if args.vimtype:
         vimtype = getattr(vim, args.vimtype)
 
     datastores = []
```

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/hostnic.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/hostnic.py`

 * *Files 1% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             'help': 'treat unplugged nics with that status code'
         }
     })
 
     args = parser.get_args()
 
     si = service_instance.connect(args)
-    check = Check(shortname='VSPHERE-NIC')
+    check = Check()
 
     #vm_view = si.content.viewManager.CreateContainerView(parentView, [vim.VirtualMachine], True)
     try:
         vm = find_entity_views(
             si,
             vim.HostSystem,
             begin_entity=si.content.rootFolder,
```

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/hostruntime.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/hostruntime.py`

 * *Files 1% similar despite different names*

```diff
@@ -68,15 +68,15 @@
 
     # default value differs if mode == maintenance
     if not args.maintenance_state:
         args.maintenance_state = 'CRITICAL' if args.mode == 'maintenance' else 'UNKNOWN'
 
     si = service_instance.connect(args)
 
-    check = Check(shortname='VSPHERE-RUNTIME')
+    check = Check()
 
     #vm_view = si.content.viewManager.CreateContainerView(parentView, [vim.VirtualMachine], True)
     try:
         vm = find_entity_views(
             si,
             vim.HostSystem,
             begin_entity=si.content.rootFolder,
```

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/hostservice.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/hostservice.py`

 * *Files 2% similar despite different names*

```diff
@@ -49,15 +49,15 @@
             'help': 'exit with this status if the host is in maintenance, '
                     'default UNKNOWN, or CRITICAL if --mode maintenance'
         }
     })
     args = parser.get_args()
 
     si = service_instance.connect(args)
-    check = Check(shortname='VSPHERE-SERVICE')
+    check = Check()
 
     try:
         host = find_entity_views(
             si,
             vim.HostSystem,
             begin_entity=si.content.rootFolder,
             sieve=( {'name': args.vihost} if args.vihost else None ),
```

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/hoststorage.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/hoststorage.py`

 * *Files 2% similar despite different names*

```diff
@@ -64,15 +64,15 @@
             'help': 'exit with this status if the host is in maintenance, '
                     'default UNKNOWN, or CRITICAL if --mode maintenance'
         }
     })
     args = parser.get_args()
 
     si = service_instance.connect(args)
-    check = Check(shortname='VSPHERE-STORAGE')
+    check = Check()
 
     try:
         host = find_entity_views(
             si,
             vim.HostSystem,
             begin_entity=si.content.rootFolder,
             sieve=( {'name': args.vihost} if args.vihost else None ),
```

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/listmetrics.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/listmetrics.py`

 * *Files identical despite different names*

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/media.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/media.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,15 +36,15 @@
     # parser.add_optional_arguments(cli.Argument.DATACENTER_NAME)
     parser.add_optional_arguments(cli.Argument.VIHOST)
     parser.add_optional_arguments(CheckArgument.ALLOWED('regex match against vm name'))
     parser.add_optional_arguments(CheckArgument.BANNED('regex match against vm name'))
     args = parser.get_args()
     si = service_instance.connect(args)
 
-    check = Check(shortname='VSPHERE-MEDIA')
+    check = Check()
 
     if args.vihost:
         host_view = si.content.viewManager.CreateContainerView(
             si.content.rootFolder, [vim.HostSystem], True)
         try:
             parentView = next(x for x in host_view.view if x.name.lower() == args.vihost.lower())
         except:
```

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/perf.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/perf.py`

 * *Files 1% similar despite different names*

```diff
@@ -73,15 +73,15 @@
     return info
 
 
 def run():
     parser = get_argparser()
     args = parser.get_args()
 
-    check = Check(shortname="VSPHERE-PERFCOUNTER")
+    check = Check()
     check.set_threshold(warning=args.warning, critical=args.critical)
 
     args._si = service_instance.connect(args)
 
     try:
         vimtype = getattr(vim, args.vimtype)
     except:
```

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/snapshots.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/snapshots.py`

 * *Files 2% similar despite different names*

```diff
@@ -109,15 +109,15 @@
     global args
     parser = get_argparser()
     args = parser.get_args()
 
     if not (args.warning or args.critical):
         raise Exception("at least one of --warning or --critical is required")
 
-    check = Check(shortname="VSPHERE-SNAPSHOTS")
+    check = Check()
     check.set_threshold(warning=args.warning, critical=args.critical)
 
     args._si = service_instance.connect(args)
 
     vms = find_entity_views(
         args._si,
         vim.VirtualMachine,
```

### Comparing `checkvsphere-0.2.0/checkvsphere/vcmd/vsan.py` & `checkvsphere-0.2.1/checkvsphere/vcmd/vsan.py`

 * *Files 0% similar despite different names*

```diff
@@ -60,15 +60,15 @@
 
 def run():
     global args
     import_vsan()
     parser = get_argparser()
     args = parser.get_args()
 
-    check = Check(shortname="VSPHERE-VSAN")
+    check = Check()
 
     args._si = service_instance.connect(args)
 
     clusters = find_entity_views(
         args._si,
         vim.ClusterComputeResource,
         begin_entity=args._si.content.rootFolder,
```

### Comparing `checkvsphere-0.2.0/pyproject.toml` & `checkvsphere-0.2.1/pyproject.toml`

 * *Files 11% similar despite different names*

```diff
@@ -2,22 +2,22 @@
 build-backend = "flit_core.buildapi"
 requires = ["flit_core >=3.2,<4"]
 
 [project]
 name = "checkvsphere"
 readme = "README.md"
 description = "check_vsphere monitoring plugin"
-version = "0.2.0"
+version = "0.2.1"
 requires-python = ">= 3.6"
 authors = [
     { name = "Danijel Tasov", email = "danijel.tasov@consol.de" }
 ]
 dependencies = [
     "pyvmomi >= 8.0.0.1, < 9",
-    "monplugin >= 0.5.1",
+    "monplugin >= 0.6.0",
 ]
 classifiers = [
     "Development Status :: 3 - Alpha",
     "Topic :: System :: Monitoring",
     "License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)",
 ]
```

### Comparing `checkvsphere-0.2.0/PKG-INFO` & `checkvsphere-0.2.1/PKG-INFO`

 * *Files 13% similar despite different names*

```diff
@@ -1,25 +1,25 @@
 Metadata-Version: 2.1
 Name: checkvsphere
-Version: 0.2.0
+Version: 0.2.1
 Summary: check_vsphere monitoring plugin
 Author-email: Danijel Tasov <danijel.tasov@consol.de>
 Requires-Python: >= 3.6
 Description-Content-Type: text/markdown
 Classifier: Development Status :: 3 - Alpha
 Classifier: Topic :: System :: Monitoring
 Classifier: License :: OSI Approved :: GNU Affero General Public License v3 or later (AGPLv3+)
 Requires-Dist: pyvmomi >= 8.0.0.1, < 9
-Requires-Dist: monplugin >= 0.5.1
+Requires-Dist: monplugin >= 0.6.0
 Project-URL: documentation, https://consol.github.io/check_vsphere
 Project-URL: homepage, https://github.com/consol/check_vsphere
 Project-URL: issues, https://github.com/consol/check_vsphere/issues
 Project-URL: repository, https://github.com/consol/check_vsphere.git
 
-[Documentation](https://consol.github.io/check_vsphere/#/)
+[Documentation](https://consol-monitoring.github.io/check_vsphere/#/)
 
 # Installation
 
 ```
 pip install checkvsphere
 ```
```

