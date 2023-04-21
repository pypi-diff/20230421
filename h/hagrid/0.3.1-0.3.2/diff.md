# Comparing `tmp/hagrid-0.3.1.tar.gz` & `tmp/hagrid-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "hagrid-0.3.1.tar", last modified: Tue Apr 18 05:38:12 2023, max compression
+gzip compressed data, was "hagrid-0.3.2.tar", last modified: Fri Apr 21 03:26:01 2023, max compression
```

## Comparing `hagrid-0.3.1.tar` & `hagrid-0.3.2.tar`

### file list

```diff
@@ -1,45 +1,45 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:38:12.228451 hagrid-0.3.1/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-18 05:38:12.228451 hagrid-0.3.1/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-18 05:35:57.000000 hagrid-0.3.1/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:38:12.228451 hagrid-0.3.1/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/art.py
--rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/auth.py
--rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/azure.py
--rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/cache.py
--rw-r--r--   0 runner    (1001) docker     (123)   134699 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/deps.py
--rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/exceptions.py
--rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/file.py
--rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/git_check.py
--rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/grammar.py
--rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/land.py
--rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/launch.py
--rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/lib.py
--rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-18 05:36:12.000000 hagrid-0.3.1/hagrid/manifest_template.yml
--rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/mode.py
--rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/names.py
--rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/nb_output.py
--rw-r--r--   0 runner    (1001) docker     (123)     7866 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/orchestra.py
--rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/parse_template.py
--rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/quickstart_ui.py
--rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/rand_sec.py
--rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/style.py
--rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/util.py
--rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-18 05:36:12.000000 hagrid-0.3.1/hagrid/version.py
--rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/win_bootstrap.py
--rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-18 05:35:57.000000 hagrid-0.3.1/hagrid/wizard_ui.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:38:12.228451 hagrid-0.3.1/hagrid.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-18 05:38:12.000000 hagrid-0.3.1/hagrid.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-18 05:38:12.000000 hagrid-0.3.1/hagrid.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 05:38:12.000000 hagrid-0.3.1/hagrid.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-18 05:38:12.000000 hagrid-0.3.1/hagrid.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-18 05:38:12.000000 hagrid-0.3.1/hagrid.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-18 05:38:12.000000 hagrid-0.3.1/hagrid.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 05:38:12.228451 hagrid-0.3.1/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-18 05:36:12.000000 hagrid-0.3.1/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:38:12.228451 hagrid-0.3.1/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 05:35:57.000000 hagrid-0.3.1/tests/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 05:38:12.228451 hagrid-0.3.1/tests/hagrid/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 05:35:57.000000 hagrid-0.3.1/tests/hagrid/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-18 05:35:57.000000 hagrid-0.3.1/tests/hagrid/cli_test.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 03:26:01.325923 hagrid-0.3.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     7377 2023-04-21 03:23:42.000000 hagrid-0.3.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5882 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/art.py
+-rw-r--r--   0 runner    (1001) docker     (123)      617 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/auth.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1796 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/azure.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2159 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)   134691 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)    30059 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/deps.py
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/exceptions.py
+-rw-r--r--   0 runner    (1001) docker     (123)      180 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/file.py
+-rw-r--r--   0 runner    (1001) docker     (123)      365 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/git_check.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12046 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/grammar.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1504 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/land.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3079 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/launch.py
+-rw-r--r--   0 runner    (1001) docker     (123)    13857 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/lib.py
+-rw-r--r--   0 runner    (1001) docker     (123)      882 2023-04-21 03:23:57.000000 hagrid-0.3.2/hagrid/manifest_template.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      960 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/mode.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2825 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/names.py
+-rw-r--r--   0 runner    (1001) docker     (123)      393 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/nb_output.py
+-rw-r--r--   0 runner    (1001) docker     (123)     8198 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/orchestra.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6043 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/parse_template.py
+-rw-r--r--   0 runner    (1001) docker     (123)    10203 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/quickstart_ui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2819 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/rand_sec.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1429 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/style.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1714 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/util.py
+-rw-r--r--   0 runner    (1001) docker     (123)      113 2023-04-21 03:23:57.000000 hagrid-0.3.2/hagrid/version.py
+-rw-r--r--   0 runner    (1001) docker     (123)     7950 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/win_bootstrap.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2008 2023-04-21 03:23:42.000000 hagrid-0.3.2/hagrid/wizard_ui.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/hagrid.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      232 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      758 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      210 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       13 2023-04-21 03:26:01.000000 hagrid-0.3.2/hagrid.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 03:26:01.325923 hagrid-0.3.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1216 2023-04-21 03:23:57.000000 hagrid-0.3.2/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:23:42.000000 hagrid-0.3.2/tests/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:26:01.325923 hagrid-0.3.2/tests/hagrid/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 03:23:42.000000 hagrid-0.3.2/tests/hagrid/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6784 2023-04-21 03:23:42.000000 hagrid-0.3.2/tests/hagrid/cli_test.py
```

### Comparing `hagrid-0.3.1/README.md` & `hagrid-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/__init__.py` & `hagrid-0.3.2/hagrid/__init__.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/art.py` & `hagrid-0.3.2/hagrid/art.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/auth.py` & `hagrid-0.3.2/hagrid/auth.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/azure.py` & `hagrid-0.3.2/hagrid/azure.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/cache.py` & `hagrid-0.3.2/hagrid/cache.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/cli.py` & `hagrid-0.3.2/hagrid/cli.py`

 * *Files 0% similar despite different names*

```diff
@@ -1926,15 +1926,15 @@
         "TRAEFIK_TAG": str(tag),
         "NODE_NAME": str(snake_name),
         "NODE_TYPE": str(node_type.input),
         "TRAEFIK_PUBLIC_NETWORK_IS_EXTERNAL": "False",
         "VERSION": version_string,
         "VERSION_HASH": version_hash,
         "USE_BLOB_STORAGE": str(use_blob_storage),
-        "FRONTEND_TARGET": "grid-ui-development",
+        "FRONTEND_TARGET": "grid-ui-production",
         "STACK_API_KEY": str(
             generate_sec_random_password(length=48, special_chars=False)
         ),
         "ENABLE_OBLV": str(enable_oblv).lower(),
     }
 
     if "trace" in kwargs and kwargs["trace"] is True:
@@ -2976,15 +2976,15 @@
 
 def create_land_docker_cmd(verb: GrammarVerb) -> str:
     node_name = verb.get_named_term_type(name="node_name")
     snake_name = str(node_name.snake_input)
     containers = shell("docker ps --format '{{.Names}}' | " + f"grep {snake_name}")
 
     # Check if the container name belongs to worker container
-    if "celeryworker" in containers:
+    if "proxy" in containers:
         path = GRID_SRC_PATH
         env_var = ";export $(cat .env | sed 's/#.*//g' | xargs);"
     else:
         path = GRID_SRC_PATH + "/worker"
         env_var = ";export $(cat ../.env | sed 's/#.*//g' | xargs);"
 
     cmd = ""
```

### Comparing `hagrid-0.3.1/hagrid/deps.py` & `hagrid-0.3.2/hagrid/deps.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/grammar.py` & `hagrid-0.3.2/hagrid/grammar.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/land.py` & `hagrid-0.3.2/hagrid/land.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/launch.py` & `hagrid-0.3.2/hagrid/launch.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/lib.py` & `hagrid-0.3.2/hagrid/lib.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/manifest_template.yml` & `hagrid-0.3.2/hagrid/manifest_template.yml`

 * *Files 9% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 manifestVersion: 0.1
-hagrid_version: 0.3.1
+hagrid_version: 0.3.2
 syft_version: 0.8.0-beta.8
 dockerTag: 0.8.0-beta.8
 baseUrl: https://raw.githubusercontent.com/OpenMined/PySyft/
-hash: 18b42582d723ff812ea9afe3d542b93ffb648c98
+hash: 1c8d04be94dbcf5f9db7e288073dd811ce56f183
 target_dir: ~/.hagrid/PySyft/
 files:
   grid:
     path: packages/grid/
     common:
     - rabbitmq/rabbitmq.conf
     - redis/redis.conf
```

### Comparing `hagrid-0.3.1/hagrid/mode.py` & `hagrid-0.3.2/hagrid/mode.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/names.py` & `hagrid-0.3.2/hagrid/names.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/orchestra.py` & `hagrid-0.3.2/hagrid/orchestra.py`

 * *Files 3% similar despite different names*

```diff
@@ -12,14 +12,15 @@
 from typing import Optional
 
 # third party
 import gevent
 
 # relative
 from .cli import str_to_bool
+from .deps import LATEST_STABLE_SYFT
 from .grammar import find_available_port
 from .names import random_name
 from .util import shell
 
 # Gevent used instead of threading module ,as we monkey patch gevent in syft
 # and this causes context switch error when we use normal threading in hagrid
 
@@ -120,29 +121,30 @@
         name: Optional[str] = None,
         node_type: Optional[str] = None,
         dev_mode: bool = False,
         cmd: bool = False,
         reset: bool = False,
         tail: bool = False,
         port: Optional[int] = None,
-        host: Optional[str] = None,
+        host: Optional[str] = "0.0.0.0",  # nosec
         processes: int = 1,  # temporary work around for jax in subprocess
         local_db: bool = False,
+        tag: Optional[str] = "latest",
     ) -> Optional[NodeHandle]:
         dev_mode = str_to_bool(os.environ.get("DEV_MODE", f"{dev_mode}"))
 
         default_port = 8080
         node_type_enum: Optional[NodeType] = get_node_type(node_type=node_type)
         if not node_type_enum:
             return None
 
         if node_type_enum == NodeType.PYTHON:
             sy = get_syft_client()
             if port:
-                start, stop = sy.bind_worker(  # type: ignore
+                start, stop = sy.serve_node(  # type: ignore
                     name=name,
                     host=host,
                     port=port,
                     reset=reset,
                     dev_mode=dev_mode,
                     tail=tail,
                 )
@@ -151,15 +153,15 @@
                     node_type=node_type_enum,
                     name=name,
                     port=port,
                     url="http://localhost",
                     shutdown=stop,
                 )
             else:
-                worker = sy.Worker.named(name, processes=processes, reset=reset, local_db=local_db)  # type: ignore
+                worker = sy.Domain.named(name, processes=processes, reset=reset, local_db=local_db)  # type: ignore
                 return NodeHandle(
                     node_type=node_type_enum, name=name, python_node=worker
                 )
 
         # Currently by default we launch in dev mode
         if reset:
             Orchestra.reset(name, node_type)
@@ -190,14 +192,21 @@
 
         if cmd:
             commands.append("--cmd")
 
         if tail:
             commands.append("--tail")
 
+        if tag:
+            commands.append(f"--tag={tag}")
+            if tag == "beta":
+                commands.append("--build-src=dev")
+            if tag == "latest":
+                commands.append(f"--build-src={LATEST_STABLE_SYFT}")
+
         # needed for building containers
         USER = os.environ.get("USER", getpass.getuser())
         env = os.environ.copy()
         env["USER"] = USER
 
         process = subprocess.Popen(  # nosec
             commands, stdout=subprocess.PIPE, stderr=subprocess.PIPE, text=True, env=env
@@ -233,15 +242,15 @@
             else:
                 print(f"❌ Unable to remove container: {snake_name} :{land_output}")
 
     @staticmethod
     def reset(name: str, node_type_enum: NodeType) -> None:
         if node_type_enum == NodeType.PYTHON:
             sy = get_syft_client()
-            _ = sy.Worker.named(name, processes=1, reset=True)  # type: ignore
+            _ = sy.Domain.named(name, processes=1, reset=True)  # type: ignore
         else:
             snake_name = to_snake_case(name)
 
             volume_output = shell(
                 f"docker volume rm {snake_name}_credentials-data --force || true"
             )
```

### Comparing `hagrid-0.3.1/hagrid/parse_template.py` & `hagrid-0.3.2/hagrid/parse_template.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/quickstart_ui.py` & `hagrid-0.3.2/hagrid/quickstart_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/rand_sec.py` & `hagrid-0.3.2/hagrid/rand_sec.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/style.py` & `hagrid-0.3.2/hagrid/style.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/util.py` & `hagrid-0.3.2/hagrid/util.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/win_bootstrap.py` & `hagrid-0.3.2/hagrid/win_bootstrap.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid/wizard_ui.py` & `hagrid-0.3.2/hagrid/wizard_ui.py`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/hagrid.egg-info/SOURCES.txt` & `hagrid-0.3.2/hagrid.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `hagrid-0.3.1/setup.py` & `hagrid-0.3.2/setup.py`

 * *Files 2% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # stdlib
 import platform
 
 # third party
 from setuptools import find_packages
 from setuptools import setup
 
-__version__ = "0.3.1"
+__version__ = "0.3.2"
 
 DATA_FILES = {"img": ["hagrid/img/*.png"], "hagrid": ["*.yml"]}
 
 packages = [
     "ascii_magic",
     "click>=7.1",
     "cryptography>=37.0.2",
```

### Comparing `hagrid-0.3.1/tests/hagrid/cli_test.py` & `hagrid-0.3.2/tests/hagrid/cli_test.py`

 * *Files identical despite different names*

