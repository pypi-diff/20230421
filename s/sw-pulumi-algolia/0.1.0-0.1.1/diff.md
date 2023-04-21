# Comparing `tmp/sw_pulumi_algolia-0.1.0.tar.gz` & `tmp/sw_pulumi_algolia-0.1.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "sw_pulumi_algolia-0.1.0.tar", last modified: Tue Aug 16 03:40:17 2022, max compression
+gzip compressed data, was "sw_pulumi_algolia-0.1.1.tar", last modified: Fri Apr 21 05:46:14 2023, max compression
```

## Comparing `sw_pulumi_algolia-0.1.0.tar` & `sw_pulumi_algolia-0.1.1.tar`

### file list

```diff
@@ -1,25 +1,25 @@
-drwxr-xr-x   0 lester    (1000) lester    (1000)        0 2022-08-16 03:40:17.501200 sw_pulumi_algolia-0.1.0/
--rw-r--r--   0 lester    (1000) lester    (1000)     1296 2022-08-16 03:40:17.501200 sw_pulumi_algolia-0.1.0/PKG-INFO
--rw-r--r--   0 lester    (1000) lester    (1000)      706 2022-08-16 03:38:09.000000 sw_pulumi_algolia-0.1.0/README.md
--rw-r--r--   0 lester    (1000) lester    (1000)       38 2022-08-16 03:40:17.501200 sw_pulumi_algolia-0.1.0/setup.cfg
--rw-r--r--   0 lester    (1000) lester    (1000)     2126 2022-08-16 03:39:02.000000 sw_pulumi_algolia-0.1.0/setup.py
-drwxr-xr-x   0 lester    (1000) lester    (1000)        0 2022-08-16 03:40:17.501200 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/
--rw-r--r--   0 lester    (1000) lester    (1000)     1071 2022-08-16 03:39:43.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/__init__.py
--rw-r--r--   0 lester    (1000) lester    (1000)     8081 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/_utilities.py
--rw-r--r--   0 lester    (1000) lester    (1000)    14594 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/api_key.py
-drwxr-xr-x   0 lester    (1000) lester    (1000)        0 2022-08-16 03:40:17.501200 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/config/
--rw-r--r--   0 lester    (1000) lester    (1000)      285 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/config/__init__.py
--rw-r--r--   0 lester    (1000) lester    (1000)      749 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/config/vars.py
--rw-r--r--   0 lester    (1000) lester    (1000)     2742 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/get_index.py
--rw-r--r--   0 lester    (1000) lester    (1000)    26576 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/index.py
--rw-r--r--   0 lester    (1000) lester    (1000)    13467 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/outputs.py
--rw-r--r--   0 lester    (1000) lester    (1000)     5540 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/provider.py
--rw-r--r--   0 lester    (1000) lester    (1000)       44 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/pulumi-plugin.json
--rw-r--r--   0 lester    (1000) lester    (1000)        0 2022-08-16 03:37:36.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/py.typed
-drwxr-xr-x   0 lester    (1000) lester    (1000)        0 2022-08-16 03:40:17.501200 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia.egg-info/
--rw-r--r--   0 lester    (1000) lester    (1000)     1296 2022-08-16 03:40:17.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia.egg-info/PKG-INFO
--rw-r--r--   0 lester    (1000) lester    (1000)      604 2022-08-16 03:40:17.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia.egg-info/SOURCES.txt
--rw-r--r--   0 lester    (1000) lester    (1000)        1 2022-08-16 03:40:17.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia.egg-info/dependency_links.txt
--rw-r--r--   0 lester    (1000) lester    (1000)        1 2022-08-16 03:40:17.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia.egg-info/not-zip-safe
--rw-r--r--   0 lester    (1000) lester    (1000)       49 2022-08-16 03:40:17.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia.egg-info/requires.txt
--rw-r--r--   0 lester    (1000) lester    (1000)       18 2022-08-16 03:40:17.000000 sw_pulumi_algolia-0.1.0/sw_pulumi_algolia.egg-info/top_level.txt
+drwxr-xr-x   0 lester    (1000) lester    (1000)        0 2023-04-21 05:46:14.944274 sw_pulumi_algolia-0.1.1/
+-rw-r--r--   0 lester    (1000) lester    (1000)     1296 2023-04-21 05:46:14.944274 sw_pulumi_algolia-0.1.1/PKG-INFO
+-rw-r--r--   0 lester    (1000) lester    (1000)      706 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/README.md
+-rw-r--r--   0 lester    (1000) lester    (1000)       38 2023-04-21 05:46:14.944274 sw_pulumi_algolia-0.1.1/setup.cfg
+-rw-r--r--   0 lester    (1000) lester    (1000)     2022 2023-04-21 05:40:37.000000 sw_pulumi_algolia-0.1.1/setup.py
+drwxr-xr-x   0 lester    (1000) lester    (1000)        0 2023-04-21 05:46:14.944274 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/
+-rw-r--r--   0 lester    (1000) lester    (1000)     1071 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/__init__.py
+-rw-r--r--   0 lester    (1000) lester    (1000)     8081 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/_utilities.py
+-rw-r--r--   0 lester    (1000) lester    (1000)    14594 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/api_key.py
+drwxr-xr-x   0 lester    (1000) lester    (1000)        0 2023-04-21 05:46:14.944274 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/config/
+-rw-r--r--   0 lester    (1000) lester    (1000)      285 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/config/__init__.py
+-rw-r--r--   0 lester    (1000) lester    (1000)      749 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/config/vars.py
+-rw-r--r--   0 lester    (1000) lester    (1000)     2742 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/get_index.py
+-rw-r--r--   0 lester    (1000) lester    (1000)    26576 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/index.py
+-rw-r--r--   0 lester    (1000) lester    (1000)    13467 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/outputs.py
+-rw-r--r--   0 lester    (1000) lester    (1000)     5540 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/provider.py
+-rw-r--r--   0 lester    (1000) lester    (1000)       44 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/pulumi-plugin.json
+-rw-r--r--   0 lester    (1000) lester    (1000)        0 2023-04-21 05:08:10.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/py.typed
+drwxr-xr-x   0 lester    (1000) lester    (1000)        0 2023-04-21 05:46:14.944274 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia.egg-info/
+-rw-r--r--   0 lester    (1000) lester    (1000)     1296 2023-04-21 05:46:14.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia.egg-info/PKG-INFO
+-rw-r--r--   0 lester    (1000) lester    (1000)      604 2023-04-21 05:46:14.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia.egg-info/SOURCES.txt
+-rw-r--r--   0 lester    (1000) lester    (1000)        1 2023-04-21 05:46:14.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia.egg-info/dependency_links.txt
+-rw-r--r--   0 lester    (1000) lester    (1000)        1 2023-04-21 05:40:25.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia.egg-info/not-zip-safe
+-rw-r--r--   0 lester    (1000) lester    (1000)       35 2023-04-21 05:46:14.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia.egg-info/requires.txt
+-rw-r--r--   0 lester    (1000) lester    (1000)       18 2023-04-21 05:46:14.000000 sw_pulumi_algolia-0.1.1/sw_pulumi_algolia.egg-info/top_level.txt
```

### Comparing `sw_pulumi_algolia-0.1.0/PKG-INFO` & `sw_pulumi_algolia-0.1.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw_pulumi_algolia
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Pulumi package for creating and managing algolia cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/swarm-work/pulumi-algolia
 Description: # Algolia Resource Provider
         
         The Algolia Resource Provider lets you manage [Algolia](https://algolia.com) resources.
```

### Comparing `sw_pulumi_algolia-0.1.0/README.md` & `sw_pulumi_algolia-0.1.1/README.md`

 * *Files identical despite different names*

### Comparing `sw_pulumi_algolia-0.1.0/setup.py` & `sw_pulumi_algolia-0.1.1/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -4,22 +4,22 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "0.1.0"
-PLUGIN_VERSION = "0.1.0"
+VERSION = "0.1.1"
+PLUGIN_VERSION = "0.1.1"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
-            check_call(['pulumi', 'plugin', 'install', 'resource', 'algolia', PLUGIN_VERSION])
+            pass
         except OSError as error:
             if error.errno == errno.ENOENT:
                 print(f"""
                 There was an error installing the algolia resource provider plugin.
                 It looks like `pulumi` is not installed on your system.
                 Please visit https://pulumi.com/ to install the Pulumi CLI.
                 You may try manually installing the plugin by running
@@ -57,10 +57,9 @@
               'py.typed',
               'pulumi-plugin.json',
           ]
       },
       install_requires=[
           'parver>=0.2.1',
           'pulumi>=3.0.0,<4.0.0',
-          'semver>=2.8.1'
       ],
       zip_safe=False)
```

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/__init__.py` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/__init__.py`

 * *Files identical despite different names*

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/_utilities.py` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/_utilities.py`

 * *Files identical despite different names*

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/api_key.py` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/api_key.py`

 * *Files identical despite different names*

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/config/vars.py` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/config/vars.py`

 * *Files identical despite different names*

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/get_index.py` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/get_index.py`

 * *Files identical despite different names*

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/index.py` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/index.py`

 * *Files identical despite different names*

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/outputs.py` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/outputs.py`

 * *Files identical despite different names*

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia/provider.py` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia/provider.py`

 * *Files identical despite different names*

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia.egg-info/PKG-INFO` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia.egg-info/PKG-INFO`

 * *Files 8% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: sw-pulumi-algolia
-Version: 0.1.0
+Version: 0.1.1
 Summary: A Pulumi package for creating and managing algolia cloud resources.
 Home-page: https://www.pulumi.com
 License: Apache-2.0
 Project-URL: Repository, https://github.com/swarm-work/pulumi-algolia
 Description: # Algolia Resource Provider
         
         The Algolia Resource Provider lets you manage [Algolia](https://algolia.com) resources.
```

### Comparing `sw_pulumi_algolia-0.1.0/sw_pulumi_algolia.egg-info/SOURCES.txt` & `sw_pulumi_algolia-0.1.1/sw_pulumi_algolia.egg-info/SOURCES.txt`

 * *Files identical despite different names*

