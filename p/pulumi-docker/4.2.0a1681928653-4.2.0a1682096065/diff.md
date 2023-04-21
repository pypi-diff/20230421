# Comparing `tmp/pulumi_docker-4.2.0a1681928653.tar.gz` & `tmp/pulumi_docker-4.2.0a1682096065.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pulumi_docker-4.2.0a1681928653.tar", last modified: Wed Apr 19 18:49:09 2023, max compression
+gzip compressed data, was "pulumi_docker-4.2.0a1682096065.tar", last modified: Fri Apr 21 16:59:02 2023, max compression
```

## Comparing `pulumi_docker-4.2.0a1681928653.tar` & `pulumi_docker-4.2.0a1682096065.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:49:09.789551 pulumi_docker-4.2.0a1681928653/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-19 18:49:09.789551 pulumi_docker-4.2.0a1681928653/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:49:09.789551 pulumi_docker-4.2.0a1681928653/pulumi_docker/
--rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/_enums.py
--rw-r--r--   0 runner    (1001) docker     (123)   153875 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/_inputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/_utilities.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:49:09.789551 pulumi_docker-4.2.0a1681928653/pulumi_docker/config/
--rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/config/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/config/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/config/vars.py
--rw-r--r--   0 runner    (1001) docker     (123)   155376 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/container.py
--rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/get_logs.py
--rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/get_network.py
--rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/get_plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/get_registry_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/get_remote_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/image.py
--rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/network.py
--rw-r--r--   0 runner    (1001) docker     (123)   125340 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/outputs.py
--rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/plugin.py
--rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/provider.py
--rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/pulumi-plugin.json
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/py.typed
--rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/registry_image.py
--rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/remote_image.py
--rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/secret.py
--rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/service.py
--rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/service_config.py
--rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/tag.py
--rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker/volume.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 18:49:09.789551 pulumi_docker-4.2.0a1681928653/pulumi_docker.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/pulumi_docker.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 18:49:09.789551 pulumi_docker-4.2.0a1681928653/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-19 18:49:09.000000 pulumi_docker-4.2.0a1681928653/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:59:02.261206 pulumi_docker-4.2.0a1682096065/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-21 16:59:02.261206 pulumi_docker-4.2.0a1682096065/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1886 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:59:02.257205 pulumi_docker-4.2.0a1682096065/pulumi_docker/
+-rw-r--r--   0 runner    (1001) docker     (123)     2755 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      535 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/_enums.py
+-rw-r--r--   0 runner    (1001) docker     (123)   153875 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/_inputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8081 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/_utilities.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:59:02.261206 pulumi_docker-4.2.0a1682096065/pulumi_docker/config/
+-rw-r--r--   0 runner    (1001) docker     (123)      285 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/config/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2108 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/config/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1687 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/config/vars.py
+-rw-r--r--   0 runner    (1001) docker     (123)   155376 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/container.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9353 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/get_logs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5336 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/get_network.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5876 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/get_plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5400 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/get_registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     4426 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/get_remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10170 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    32844 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/network.py
+-rw-r--r--   0 runner    (1001) docker     (123)   125340 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)    24695 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/plugin.py
+-rw-r--r--   0 runner    (1001) docker     (123)    11374 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/provider.py
+-rw-r--r--   0 runner    (1001) docker     (123)       43 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/pulumi-plugin.json
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/py.typed
+-rw-r--r--   0 runner    (1001) docker     (123)    16148 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/registry_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)    26720 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/remote_image.py
+-rw-r--r--   0 runner    (1001) docker     (123)     9540 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/secret.py
+-rw-r--r--   0 runner    (1001) docker     (123)    25797 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/service.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8137 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/service_config.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8994 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/tag.py
+-rw-r--r--   0 runner    (1001) docker     (123)    14437 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker/volume.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 16:59:02.257205 pulumi_docker-4.2.0a1682096065/pulumi_docker.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2226 2023-04-21 16:59:02.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      982 2023-04-21 16:59:02.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:59:02.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 16:59:02.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 16:59:02.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       14 2023-04-21 16:59:02.000000 pulumi_docker-4.2.0a1682096065/pulumi_docker.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 16:59:02.261206 pulumi_docker-4.2.0a1682096065/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     2121 2023-04-21 16:59:01.000000 pulumi_docker-4.2.0a1682096065/setup.py
```

### Comparing `pulumi_docker-4.2.0a1681928653/PKG-INFO` & `pulumi_docker-4.2.0a1682096065/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi_docker
-Version: 4.2.0a1681928653
+Version: 4.2.0a1682096065
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi docker
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_docker-4.2.0a1681928653/README.md` & `pulumi_docker-4.2.0a1682096065/README.md`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/__init__.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/__init__.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/_enums.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/_enums.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/_inputs.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/_inputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/_utilities.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/_utilities.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/config/outputs.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/config/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/config/vars.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/config/vars.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/container.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/container.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/get_logs.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/get_logs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/get_network.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/get_network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/get_plugin.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/get_plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/get_registry_image.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/get_registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/get_remote_image.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/get_remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/image.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/network.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/network.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/outputs.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/outputs.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/plugin.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/plugin.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/provider.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/provider.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/registry_image.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/registry_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/remote_image.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/remote_image.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/secret.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/secret.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/service.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/service.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/service_config.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/service_config.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/tag.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/tag.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker/volume.py` & `pulumi_docker-4.2.0a1682096065/pulumi_docker/volume.py`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker.egg-info/PKG-INFO` & `pulumi_docker-4.2.0a1682096065/pulumi_docker.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pulumi-docker
-Version: 4.2.0a1681928653
+Version: 4.2.0a1682096065
 Summary: A Pulumi package for interacting with Docker in Pulumi programs
 Home-page: https://pulumi.io
 License: Apache-2.0
 Project-URL: Repository, https://github.com/pulumi/pulumi-docker
 Keywords: pulumi docker
 Platform: UNKNOWN
 Description-Content-Type: text/markdown
```

### Comparing `pulumi_docker-4.2.0a1681928653/pulumi_docker.egg-info/SOURCES.txt` & `pulumi_docker-4.2.0a1682096065/pulumi_docker.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pulumi_docker-4.2.0a1681928653/setup.py` & `pulumi_docker-4.2.0a1682096065/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -4,16 +4,16 @@
 
 import errno
 from setuptools import setup, find_packages
 from setuptools.command.install import install
 from subprocess import check_call
 
 
-VERSION = "4.2.0a1681928653"
-PLUGIN_VERSION = "4.2.0-alpha.1681928653+6b4895c7"
+VERSION = "4.2.0a1682096065"
+PLUGIN_VERSION = "4.2.0-alpha.1682096065+0a63aa01"
 
 class InstallPluginCommand(install):
     def run(self):
         install.run(self)
         try:
             check_call(['pulumi', 'plugin', 'install', 'resource', 'docker', PLUGIN_VERSION])
         except OSError as error:
```

