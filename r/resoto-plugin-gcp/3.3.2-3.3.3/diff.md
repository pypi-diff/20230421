# Comparing `tmp/resoto-plugin-gcp-3.3.2.tar.gz` & `tmp/resoto-plugin-gcp-3.3.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "resoto-plugin-gcp-3.3.2.tar", last modified: Fri Apr 14 16:15:02 2023, max compression
+gzip compressed data, was "resoto-plugin-gcp-3.3.3.tar", last modified: Fri Apr 21 14:35:44 2023, max compression
```

## Comparing `resoto-plugin-gcp-3.3.2.tar` & `resoto-plugin-gcp-3.3.3.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/requirements.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.798521 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/
--rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    64093 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/collector.py
--rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/gcp_client.py
--rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/gcp_resources.py
--rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/project_collector.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/base.py
--rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/billing.py
--rw-r--r--   0 runner    (1001) docker     (123)   278397 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/compute.py
--rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/container.py
--rw-r--r--   0 runner    (1001) docker     (123)    41166 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/sqladmin.py
--rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/utils.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.798521 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-14 16:15:02.000000 resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-14 16:15:02.802521 resoto-plugin-gcp-3.3.2/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/conftest.py
--rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/random_client.py
--rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_base.py
--rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_billing.py
--rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_compute.py
--rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_config.py
--rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_container.py
--rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_project_collector.py
--rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-14 16:11:40.000000 resoto-plugin-gcp-3.3.2/test/test_sqladmin.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:44.668209 resoto-plugin-gcp-3.3.3/
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 14:35:44.668209 resoto-plugin-gcp-3.3.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       56 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/requirements.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:44.664209 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/
+-rw-r--r--   0 runner    (1001) docker     (123)     5125 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    64093 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)      945 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3998 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/gcp_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)    29516 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/gcp_resources.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5034 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/project_collector.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:44.664209 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    18813 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/base.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11818 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)   278397 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)    49330 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)    41166 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/sqladmin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9109 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/utils.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:44.664209 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 14:35:44.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1014 2023-04-21 14:35:44.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:35:44.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       60 2023-04-21 14:35:44.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 14:35:44.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)      102 2023-04-21 14:35:44.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 14:35:44.000000 resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      186 2023-04-21 14:35:44.668209 resoto-plugin-gcp-3.3.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1562 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 14:35:44.668209 resoto-plugin-gcp-3.3.3/test/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1705 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/conftest.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11881 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/random_client.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2142 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/test_base.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1174 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/test_billing.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12633 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/test_compute.py
+-rw-r--r--   0 runner    (1001) docker     (123)      551 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/test_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      596 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/test_container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2354 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/test_project_collector.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1011 2023-04-21 14:32:24.000000 resoto-plugin-gcp-3.3.3/test/test_sqladmin.py
```

### Comparing `resoto-plugin-gcp-3.3.2/PKG-INFO` & `resoto-plugin-gcp-3.3.3/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto GCP Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/__init__.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/__init__.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/collector.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/config.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/gcp_client.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/gcp_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/gcp_resources.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/gcp_resources.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/project_collector.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/project_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/base.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/billing.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/compute.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/container.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/resources/sqladmin.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/resources/sqladmin.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp/utils.py` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp/utils.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/PKG-INFO` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: resoto-plugin-gcp
-Version: 3.3.2
+Version: 3.3.3
 Summary: Resoto GCP Collector Plugin
 Home-page: https://github.com/someengineering/resoto/tree/main/plugins/gcp
 License: Apache 2.0
 Keywords: cloud security
 Classifier: Development Status :: 4 - Beta
 Classifier: Intended Audience :: System Administrators
 Classifier: Intended Audience :: Information Technology
```

### Comparing `resoto-plugin-gcp-3.3.2/resoto_plugin_gcp.egg-info/SOURCES.txt` & `resoto-plugin-gcp-3.3.3/resoto_plugin_gcp.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/setup.py` & `resoto-plugin-gcp-3.3.3/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -6,15 +6,15 @@
 def read(file_name: str) -> str:
     with open(os.path.join(os.path.dirname(__file__), file_name)) as of:
         return of.read()
 
 
 setup(
     name="resoto-plugin-gcp",
-    version="3.3.2",
+    version="3.3.3",
     description="Resoto GCP Collector Plugin",
     license="Apache 2.0",
     packages=find_packages(),
     long_description=read("README.md"),
     long_description_content_type="text/markdown",
     entry_points={"resoto.plugins": ["gcp = resoto_plugin_gcp:GCPCollectorPlugin"]},
     include_package_data=True,
```

### Comparing `resoto-plugin-gcp-3.3.2/test/conftest.py` & `resoto-plugin-gcp-3.3.3/test/conftest.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/test/random_client.py` & `resoto-plugin-gcp-3.3.3/test/random_client.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/test/test_base.py` & `resoto-plugin-gcp-3.3.3/test/test_base.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/test/test_billing.py` & `resoto-plugin-gcp-3.3.3/test/test_billing.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/test/test_compute.py` & `resoto-plugin-gcp-3.3.3/test/test_compute.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/test/test_config.py` & `resoto-plugin-gcp-3.3.3/test/test_config.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/test/test_container.py` & `resoto-plugin-gcp-3.3.3/test/test_container.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/test/test_project_collector.py` & `resoto-plugin-gcp-3.3.3/test/test_project_collector.py`

 * *Files identical despite different names*

### Comparing `resoto-plugin-gcp-3.3.2/test/test_sqladmin.py` & `resoto-plugin-gcp-3.3.3/test/test_sqladmin.py`

 * *Files identical despite different names*

