# Comparing `tmp/dtproject-0.0.1.tar.gz` & `tmp/dtproject-0.0.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtproject-0.0.1.tar", last modified: Thu Apr 20 04:11:26 2023, max compression
+gzip compressed data, was "dtproject-0.0.2.tar", last modified: Fri Apr 21 02:40:17 2023, max compression
```

## Comparing `dtproject-0.0.1.tar` & `dtproject-0.0.2.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 04:11:26.688058 dtproject-0.0.1/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-20 04:11:26.688058 dtproject-0.0.1/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-20 04:11:26.688058 dtproject-0.0.1/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1765 2023-04-20 03:32:32.000000 dtproject-0.0.1/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 04:11:26.684058 dtproject-0.0.1/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 04:11:26.684058 dtproject-0.0.1/src/dtproject/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      163 2023-04-20 04:08:42.000000 dtproject-0.0.1/src/dtproject/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2023-04-19 22:08:11.000000 dtproject-0.0.1/src/dtproject/configurations.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6697 2023-04-20 03:51:24.000000 dtproject-0.0.1/src/dtproject/constants.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    25620 2023-04-20 03:54:47.000000 dtproject-0.0.1/src/dtproject/dtproject.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      480 2023-04-20 03:25:31.000000 dtproject-0.0.1/src/dtproject/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6316 2023-04-20 03:28:28.000000 dtproject-0.0.1/src/dtproject/recipe.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 04:11:26.688058 dtproject-0.0.1/src/dtproject/utils/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 02:38:03.000000 dtproject-0.0.1/src/dtproject/utils/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1299 2023-04-20 02:48:47.000000 dtproject-0.0.1/src/dtproject/utils/docker.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1198 2023-04-20 03:17:17.000000 dtproject-0.0.1/src/dtproject/utils/misc.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 04:11:26.688058 dtproject-0.0.1/src/dtproject.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-20 04:11:26.000000 dtproject-0.0.1/src/dtproject.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      446 2023-04-20 04:11:26.000000 dtproject-0.0.1/src/dtproject.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-20 04:11:26.000000 dtproject-0.0.1/src/dtproject.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       27 2023-04-20 04:11:26.000000 dtproject-0.0.1/src/dtproject.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       10 2023-04-20 04:11:26.000000 dtproject-0.0.1/src/dtproject.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.664750 dtproject-0.0.2/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-21 02:40:17.664750 dtproject-0.0.2/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-21 02:40:17.664750 dtproject-0.0.2/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1765 2023-04-20 03:32:32.000000 dtproject-0.0.2/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.660750 dtproject-0.0.2/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.660750 dtproject-0.0.2/src/dtproject/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      163 2023-04-21 02:40:11.000000 dtproject-0.0.2/src/dtproject/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2023-04-19 22:08:11.000000 dtproject-0.0.2/src/dtproject/configurations.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6697 2023-04-20 03:51:24.000000 dtproject-0.0.2/src/dtproject/constants.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    25464 2023-04-21 02:35:25.000000 dtproject-0.0.2/src/dtproject/dtproject.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      480 2023-04-20 03:25:31.000000 dtproject-0.0.2/src/dtproject/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6316 2023-04-20 03:28:28.000000 dtproject-0.0.2/src/dtproject/recipe.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.660750 dtproject-0.0.2/src/dtproject/utils/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 02:38:03.000000 dtproject-0.0.2/src/dtproject/utils/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1326 2023-04-20 14:46:26.000000 dtproject-0.0.2/src/dtproject/utils/docker.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1198 2023-04-20 03:17:17.000000 dtproject-0.0.2/src/dtproject/utils/misc.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.660750 dtproject-0.0.2/src/dtproject.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      446 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       27 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       10 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/top_level.txt
```

### Comparing `dtproject-0.0.1/setup.py` & `dtproject-0.0.2/setup.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.1/src/dtproject/constants.py` & `dtproject-0.0.2/src/dtproject/constants.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.1/src/dtproject/dtproject.py` & `dtproject-0.0.2/src/dtproject/dtproject.py`

 * *Files 0% similar despite different names*

```diff
@@ -341,24 +341,21 @@
     def ci_metadata(self, endpoint, *, arch: str, registry: str, owner: str, version: str):
         image_tag = self.image(arch=arch, owner=owner, version=version, registry=registry)
         try:
             configurations = self.configurations()
         except NotImplementedError:
             configurations = {}
         # do docker inspect
-        inspect = self.image_metadata(endpoint, arch=arch, owner=owner, version=version, registry=registry)
+        image: dict = self.image_metadata(endpoint, arch=arch, owner=owner, version=version, registry=registry)
 
-        # remove useless data
-        del inspect["ContainerConfig"]
-        del inspect["Config"]["Labels"]
         # compile metadata
         meta = {
             "version": "1.0",
             "tag": image_tag,
-            "image": inspect,
+            "image": image,
             "project": {
                 "path": self.path,
                 "name": self.name,
                 "type": self.type,
                 "type_version": self.type_version,
                 "distro": self.distro,
                 "version": self.version,
@@ -484,15 +481,14 @@
             # by default, there is only one local and one destination
             locals: List[str] = [os.path.join(root, local)]
             destinations: List[str] = [destination]
         # ---
         return locals, destinations
 
     def docs_path(self) -> str:
-        # TODO: use this in dts/docs/(env/)build
         # make sure we support this project version
         if self.type not in TEMPLATE_TO_DOCS or self.type_version not in TEMPLATE_TO_DOCS[self.type]:
             raise UnsupportedDTProjectVersion(
                 "Template {:s} v{:s} for project {:s} is not supported".format(
                     self.type, self.type_version, self.path
                 )
             )
```

### Comparing `dtproject-0.0.1/src/dtproject/recipe.py` & `dtproject-0.0.2/src/dtproject/recipe.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.1/src/dtproject/utils/docker.py` & `dtproject-0.0.2/src/dtproject/utils/docker.py`

 * *Files 6% similar despite different names*

```diff
@@ -1,21 +1,19 @@
 import socket
-from typing import Optional
+from typing import Optional, Union
 
 from dockertown import DockerClient
 
 DEFAULT_DOCKER_TCP_PORT = "2375"
 
 
-def docker_client(endpoint) -> DockerClient:
-    return (
-        endpoint
-        if isinstance(endpoint, DockerClient)
+def docker_client(endpoint: Union[None, str, DockerClient]) -> DockerClient:
+    return endpoint \
+        if isinstance(endpoint, DockerClient) \
         else DockerClient(host=sanitize_docker_baseurl(endpoint))
-    )
 
 
 def sanitize_docker_baseurl(baseurl: str, port=DEFAULT_DOCKER_TCP_PORT) -> Optional[str]:
     if baseurl is None:
         return None
     if baseurl.startswith("unix:"):
         return baseurl
```

### Comparing `dtproject-0.0.1/src/dtproject/utils/misc.py` & `dtproject-0.0.2/src/dtproject/utils/misc.py`

 * *Files identical despite different names*

