# Comparing `tmp/dtproject-0.0.2.tar.gz` & `tmp/dtproject-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dtproject-0.0.2.tar", last modified: Fri Apr 21 02:40:17 2023, max compression
+gzip compressed data, was "dtproject-0.0.3.tar", last modified: Fri Apr 21 02:51:34 2023, max compression
```

## Comparing `dtproject-0.0.2.tar` & `dtproject-0.0.3.tar`

### file list

```diff
@@ -1,22 +1,22 @@
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.664750 dtproject-0.0.2/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-21 02:40:17.664750 dtproject-0.0.2/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-21 02:40:17.664750 dtproject-0.0.2/setup.cfg
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1765 2023-04-20 03:32:32.000000 dtproject-0.0.2/setup.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.660750 dtproject-0.0.2/src/
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.660750 dtproject-0.0.2/src/dtproject/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      163 2023-04-21 02:40:11.000000 dtproject-0.0.2/src/dtproject/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2023-04-19 22:08:11.000000 dtproject-0.0.2/src/dtproject/configurations.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6697 2023-04-20 03:51:24.000000 dtproject-0.0.2/src/dtproject/constants.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    25464 2023-04-21 02:35:25.000000 dtproject-0.0.2/src/dtproject/dtproject.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      480 2023-04-20 03:25:31.000000 dtproject-0.0.2/src/dtproject/exceptions.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6316 2023-04-20 03:28:28.000000 dtproject-0.0.2/src/dtproject/recipe.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.660750 dtproject-0.0.2/src/dtproject/utils/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 02:38:03.000000 dtproject-0.0.2/src/dtproject/utils/__init__.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1326 2023-04-20 14:46:26.000000 dtproject-0.0.2/src/dtproject/utils/docker.py
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1198 2023-04-20 03:17:17.000000 dtproject-0.0.2/src/dtproject/utils/misc.py
-drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:40:17.660750 dtproject-0.0.2/src/dtproject.egg-info/
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/PKG-INFO
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      446 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/SOURCES.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/dependency_links.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       27 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/requires.txt
--rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       10 2023-04-21 02:40:17.000000 dtproject-0.0.2/src/dtproject.egg-info/top_level.txt
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:51:34.016250 dtproject-0.0.3/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-21 02:51:34.016250 dtproject-0.0.3/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       38 2023-04-21 02:51:34.016250 dtproject-0.0.3/setup.cfg
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1765 2023-04-20 03:32:32.000000 dtproject-0.0.3/setup.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:51:34.016250 dtproject-0.0.3/src/
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:51:34.016250 dtproject-0.0.3/src/dtproject/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      163 2023-04-21 02:51:27.000000 dtproject-0.0.3/src/dtproject/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      418 2023-04-19 22:08:11.000000 dtproject-0.0.3/src/dtproject/configurations.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6697 2023-04-20 03:51:24.000000 dtproject-0.0.3/src/dtproject/constants.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)    25755 2023-04-21 02:50:40.000000 dtproject-0.0.3/src/dtproject/dtproject.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      480 2023-04-20 03:25:31.000000 dtproject-0.0.3/src/dtproject/exceptions.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     6316 2023-04-20 03:28:28.000000 dtproject-0.0.3/src/dtproject/recipe.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:51:34.016250 dtproject-0.0.3/src/dtproject/utils/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-20 02:38:03.000000 dtproject-0.0.3/src/dtproject/utils/__init__.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1326 2023-04-20 14:46:26.000000 dtproject-0.0.3/src/dtproject/utils/docker.py
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)     1198 2023-04-20 03:17:17.000000 dtproject-0.0.3/src/dtproject/utils/misc.py
+drwxrwxr-x   0 afdaniele  (1000) afdaniele  (1000)        0 2023-04-21 02:51:34.016250 dtproject-0.0.3/src/dtproject.egg-info/
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      424 2023-04-21 02:51:33.000000 dtproject-0.0.3/src/dtproject.egg-info/PKG-INFO
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)      446 2023-04-21 02:51:34.000000 dtproject-0.0.3/src/dtproject.egg-info/SOURCES.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)        1 2023-04-21 02:51:33.000000 dtproject-0.0.3/src/dtproject.egg-info/dependency_links.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       27 2023-04-21 02:51:33.000000 dtproject-0.0.3/src/dtproject.egg-info/requires.txt
+-rw-rw-r--   0 afdaniele  (1000) afdaniele  (1000)       10 2023-04-21 02:51:33.000000 dtproject-0.0.3/src/dtproject.egg-info/top_level.txt
```

### Comparing `dtproject-0.0.2/setup.py` & `dtproject-0.0.3/setup.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.2/src/dtproject/constants.py` & `dtproject-0.0.3/src/dtproject/constants.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.2/src/dtproject/dtproject.py` & `dtproject-0.0.3/src/dtproject/dtproject.py`

 * *Files 2% similar despite different names*

```diff
@@ -496,15 +496,15 @@
         return os.path.join(self.path, TEMPLATE_TO_DOCS[self.type][self.type_version])
 
     def image_metadata(self, endpoint, arch: str, owner: str, registry: str, version: str):
         client = docker_client(endpoint)
         image_name = self.image(arch=arch, owner=owner, version=version, registry=registry)
         try:
             image: Image = client.image.inspect(image_name)
-            return {
+            metadata: dict = {
                 # - id: str
                 "id": image.id,
                 # - repo_tags: List[str]
                 "repo_tags": image.repo_tags,
                 # - repo_digests: List[str]
                 "repo_digests": image.repo_digests,
                 # - parent: str
@@ -536,14 +536,19 @@
                 # - graph_driver: ImageGraphDriver
                 "graph_driver": image.graph_driver.dict(),
                 # - root_fs: ImageRootFS
                 "root_fs": image.root_fs.dict(),
                 # - metadata: Dict[str, str]
                 "metadata": image.metadata,
             }
+            # sanitize posizpath objects
+            metadata["container_config"]["working_dir"] = str(metadata["container_config"]["working_dir"])
+            metadata["config"]["working_dir"] = str(metadata["config"]["working_dir"])
+            # ---
+            return metadata
         except NoSuchImage:
             raise Exception(f"Cannot get image metadata for {image_name!r}: \n {traceback.format_exc()}")
 
     def image_labels(self, endpoint, *, arch: str, owner: str, registry: str, version: str):
         metadata: dict = self.image_metadata(
             endpoint, arch=arch, owner=owner, registry=registry, version=version
         )
```

### Comparing `dtproject-0.0.2/src/dtproject/recipe.py` & `dtproject-0.0.3/src/dtproject/recipe.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.2/src/dtproject/utils/docker.py` & `dtproject-0.0.3/src/dtproject/utils/docker.py`

 * *Files identical despite different names*

### Comparing `dtproject-0.0.2/src/dtproject/utils/misc.py` & `dtproject-0.0.3/src/dtproject/utils/misc.py`

 * *Files identical despite different names*

