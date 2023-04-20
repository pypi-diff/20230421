# Comparing `tmp/layermake-0.0.7.tar.gz` & `tmp/layermake-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "layermake-0.0.7.tar", last modified: Mon Apr 10 18:26:46 2023, max compression
+gzip compressed data, was "layermake-0.0.8.tar", last modified: Thu Apr 20 23:47:39 2023, max compression
```

## Comparing `layermake-0.0.7.tar` & `layermake-0.0.8.tar`

### file list

```diff
@@ -1,23 +1,23 @@
-drwxrwxrwx   0        0        0        0 2023-04-10 18:26:46.771856 layermake-0.0.7/
--rw-rw-rw-   0        0        0     1061 2023-03-31 17:19:15.000000 layermake-0.0.7/LICENSE.md
--rw-rw-rw-   0        0        0     7937 2023-04-10 18:26:46.769859 layermake-0.0.7/PKG-INFO
--rw-rw-rw-   0        0        0     7444 2023-04-01 23:44:07.000000 layermake-0.0.7/README.md
-drwxrwxrwx   0        0        0        0 2023-04-10 18:26:46.757850 layermake-0.0.7/layermake/
--rw-rw-rw-   0        0        0      370 2023-04-10 17:31:32.000000 layermake-0.0.7/layermake/__init__.py
--rw-rw-rw-   0        0        0     4367 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/binary.py
--rw-rw-rw-   0        0        0     3827 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/bundler.py
--rw-rw-rw-   0        0        0     7906 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/cli.py
--rw-rw-rw-   0        0        0     6460 2023-04-01 17:29:10.000000 layermake-0.0.7/layermake/cmd.py
--rw-rw-rw-   0        0        0     2143 2023-04-01 14:03:05.000000 layermake-0.0.7/layermake/logger.py
--rw-rw-rw-   0        0        0     2665 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/node.py
--rw-rw-rw-   0        0        0     2549 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/publisher.py
--rw-rw-rw-   0        0        0     2866 2023-04-10 18:12:13.000000 layermake-0.0.7/layermake/python.py
-drwxrwxrwx   0        0        0        0 2023-04-10 18:26:46.768856 layermake-0.0.7/layermake.egg-info/
--rw-rw-rw-   0        0        0     7937 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      407 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       48 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       17 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/requires.txt
--rw-rw-rw-   0        0        0       10 2023-04-10 18:26:46.000000 layermake-0.0.7/layermake.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-10 18:26:46.771856 layermake-0.0.7/setup.cfg
--rw-rw-rw-   0        0        0      868 2023-04-01 14:49:19.000000 layermake-0.0.7/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 23:47:39.658653 layermake-0.0.8/
+-rw-rw-rw-   0        0        0     1061 2023-03-31 17:19:15.000000 layermake-0.0.8/LICENSE.md
+-rw-rw-rw-   0        0        0     7937 2023-04-20 23:47:39.656643 layermake-0.0.8/PKG-INFO
+-rw-rw-rw-   0        0        0     7444 2023-04-01 23:44:07.000000 layermake-0.0.8/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 23:47:39.644622 layermake-0.0.8/layermake/
+-rw-rw-rw-   0        0        0      370 2023-04-20 22:16:29.000000 layermake-0.0.8/layermake/__init__.py
+-rw-rw-rw-   0        0        0     4367 2023-04-10 18:12:13.000000 layermake-0.0.8/layermake/binary.py
+-rw-rw-rw-   0        0        0     3827 2023-04-10 18:12:13.000000 layermake-0.0.8/layermake/bundler.py
+-rw-rw-rw-   0        0        0     7906 2023-04-10 18:12:13.000000 layermake-0.0.8/layermake/cli.py
+-rw-rw-rw-   0        0        0     6460 2023-04-01 17:29:10.000000 layermake-0.0.8/layermake/cmd.py
+-rw-rw-rw-   0        0        0     2143 2023-04-01 14:03:05.000000 layermake-0.0.8/layermake/logger.py
+-rw-rw-rw-   0        0        0     2665 2023-04-10 18:12:13.000000 layermake-0.0.8/layermake/node.py
+-rw-rw-rw-   0        0        0     2549 2023-04-10 18:12:13.000000 layermake-0.0.8/layermake/publisher.py
+-rw-rw-rw-   0        0        0     3382 2023-04-20 23:46:46.000000 layermake-0.0.8/layermake/python.py
+drwxrwxrwx   0        0        0        0 2023-04-20 23:47:39.655136 layermake-0.0.8/layermake.egg-info/
+-rw-rw-rw-   0        0        0     7937 2023-04-20 23:47:39.000000 layermake-0.0.8/layermake.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      407 2023-04-20 23:47:39.000000 layermake-0.0.8/layermake.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 23:47:39.000000 layermake-0.0.8/layermake.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       48 2023-04-20 23:47:39.000000 layermake-0.0.8/layermake.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       17 2023-04-20 23:47:39.000000 layermake-0.0.8/layermake.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       10 2023-04-20 23:47:39.000000 layermake-0.0.8/layermake.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-20 23:47:39.658653 layermake-0.0.8/setup.cfg
+-rw-rw-rw-   0        0        0      868 2023-04-01 14:49:19.000000 layermake-0.0.8/setup.py
```

### Comparing `layermake-0.0.7/LICENSE.md` & `layermake-0.0.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `layermake-0.0.7/PKG-INFO` & `layermake-0.0.8/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layermake
-Version: 0.0.7
+Version: 0.0.8
 Summary: CLI toolkit for bundling AWS Lambda layers
 Home-page: https://github.com/ericmaustin/layermake
 Author: Eric Austin
 Author-email: eric.m.austin@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `layermake-0.0.7/README.md` & `layermake-0.0.8/README.md`

 * *Files identical despite different names*

### Comparing `layermake-0.0.7/layermake/binary.py` & `layermake-0.0.8/layermake/binary.py`

 * *Files identical despite different names*

### Comparing `layermake-0.0.7/layermake/bundler.py` & `layermake-0.0.8/layermake/bundler.py`

 * *Files identical despite different names*

### Comparing `layermake-0.0.7/layermake/cli.py` & `layermake-0.0.8/layermake/cli.py`

 * *Files identical despite different names*

### Comparing `layermake-0.0.7/layermake/cmd.py` & `layermake-0.0.8/layermake/cmd.py`

 * *Files identical despite different names*

### Comparing `layermake-0.0.7/layermake/logger.py` & `layermake-0.0.8/layermake/logger.py`

 * *Files identical despite different names*

### Comparing `layermake-0.0.7/layermake/node.py` & `layermake-0.0.8/layermake/node.py`

 * *Files identical despite different names*

### Comparing `layermake-0.0.7/layermake/publisher.py` & `layermake-0.0.8/layermake/publisher.py`

 * *Files identical despite different names*

### Comparing `layermake-0.0.7/layermake/python.py` & `layermake-0.0.8/layermake/python.py`

 * *Files 8% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 from typing import List
 from string import Template
 from pathlib import Path
 from .bundler import Bundler
-from .cmd import path_copy
+from .cmd import path_copy, rmtree
 from .logger import logger
 
 PYTHON_ECR_TEMPLATE = Template("public.ecr.aws/sam/build-python${runtime}:${version}")
 
 
 def _is_package(path: Path) -> bool:
     """
@@ -46,25 +46,29 @@
             local_dir=local_dir,
             build_artifact=manifest,
             no_zip=no_zip,
         )
 
     def pre_bundle(self):
         container_cmds = []
-        local_src = self._local_path / "src"
-        try:
-            local_src.mkdir(parents=True, exist_ok=True)
-        except Exception as e:
-            logger().fatal_error(f"failed to create directory {local_src} Error: {e}")
-
-        self.add_cleanup_path(local_src)
         build_target = self._local_path / "python"
 
         if self.__artifact_dir and self.__artifact_dir.exists():
+            local_src = self._local_path / "src"
+            try:
+                local_src.mkdir(parents=True, exist_ok=True)
+            except Exception as e:
+                logger().fatal_error(
+                    f"failed to create directory {local_src} Error: {e}"
+                )
+
+            self.add_cleanup_path(local_src)
+
             package_src = local_src / self.__artifact_dir.name
+
             # copy to package source
             path_copy(self.__artifact_dir, package_src)
 
             if (package_src / "requirements.txt").is_file() or (
                 package_src / "setup.py"
             ).is_file():
                 container_cmds.append(f"pip install src/{package_src.name}/. -t python")
@@ -84,8 +88,23 @@
                 cmd += f" -r {Path(self.__manifest).name}"
 
             if self.__packages:
                 cmd += " " + " ".join(self.__packages)
 
             container_cmds.append(cmd)
 
+        container_cmds.extend(
+            ["find python -name '%s' -exec rm -f {} +" % p for p in ["*.pyo", "*.pyc"]]
+        )
+        container_cmds.extend(
+            [
+                "find python -name '%s' -exec rm -rf {} +" % p
+                for p in [
+                    "__pycache__",
+                    ".cache",
+                    ".mypy_cache",
+                    ".pytest_cache",
+                ]
+            ]
+        )
+
         self._container_cmd = "; ".join(container_cmds)
```

### Comparing `layermake-0.0.7/layermake.egg-info/PKG-INFO` & `layermake-0.0.8/layermake.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: layermake
-Version: 0.0.7
+Version: 0.0.8
 Summary: CLI toolkit for bundling AWS Lambda layers
 Home-page: https://github.com/ericmaustin/layermake
 Author: Eric Austin
 Author-email: eric.m.austin@gmail.com
 License: MIT
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
```

### Comparing `layermake-0.0.7/setup.py` & `layermake-0.0.8/setup.py`

 * *Files identical despite different names*

