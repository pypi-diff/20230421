# Comparing `tmp/dask4dvc-0.2.0.tar.gz` & `tmp/dask4dvc-0.2.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dask4dvc-0.2.0.tar", max compression
+gzip compressed data, was "dask4dvc-0.2.1.tar", max compression
```

## Comparing `dask4dvc-0.2.0.tar` & `dask4dvc-0.2.1.tar`

### file list

```diff
@@ -1,12 +1,12 @@
--rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.2.0/LICENSE
--rw-r--r--   0        0        0     1637 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/README.md
--rw-r--r--   0        0        0      651 2023-04-19 15:02:16.124501 dask4dvc-0.2.0/dask4dvc/__init__.py
--rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.2.0/dask4dvc/cli/__init__.py
--rw-r--r--   0        0        0     2608 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/cli/main.py
--rw-r--r--   0        0        0     3393 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/methods.py
--rw-r--r--   0        0        0      142 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/utils/__init__.py
--rw-r--r--   0        0        0      272 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/utils/config.py
--rw-r--r--   0        0        0     1055 2023-04-13 11:02:16.867293 dask4dvc-0.2.0/dask4dvc/utils/dask.py
--rw-r--r--   0        0        0      136 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/dask4dvc/utils/main.py
--rw-r--r--   0        0        0     1271 2023-04-19 15:36:27.742838 dask4dvc-0.2.0/pyproject.toml
--rw-r--r--   0        0        0     2536 1970-01-01 00:00:00.000000 dask4dvc-0.2.0/PKG-INFO
+-rw-r--r--   0        0        0    13576 2023-01-25 13:10:23.183284 dask4dvc-0.2.1/LICENSE
+-rw-r--r--   0        0        0     1791 2023-04-21 11:17:08.062984 dask4dvc-0.2.1/README.md
+-rw-r--r--   0        0        0      651 2023-04-19 15:02:16.124501 dask4dvc-0.2.1/dask4dvc/__init__.py
+-rw-r--r--   0        0        0       76 2023-01-25 13:44:53.309679 dask4dvc-0.2.1/dask4dvc/cli/__init__.py
+-rw-r--r--   0        0        0     2795 2023-04-21 11:17:08.062984 dask4dvc-0.2.1/dask4dvc/cli/main.py
+-rw-r--r--   0        0        0     4265 2023-04-21 11:17:08.062984 dask4dvc-0.2.1/dask4dvc/methods.py
+-rw-r--r--   0        0        0      142 2023-04-19 15:36:27.742838 dask4dvc-0.2.1/dask4dvc/utils/__init__.py
+-rw-r--r--   0        0        0      272 2023-04-19 15:36:27.742838 dask4dvc-0.2.1/dask4dvc/utils/config.py
+-rw-r--r--   0        0        0     1055 2023-04-13 11:02:16.867293 dask4dvc-0.2.1/dask4dvc/utils/dask.py
+-rw-r--r--   0        0        0      136 2023-04-19 15:36:27.742838 dask4dvc-0.2.1/dask4dvc/utils/main.py
+-rw-r--r--   0        0        0     1256 2023-04-21 11:17:08.072984 dask4dvc-0.2.1/pyproject.toml
+-rw-r--r--   0        0        0     2690 1970-01-01 00:00:00.000000 dask4dvc-0.2.1/PKG-INFO
```

### Comparing `dask4dvc-0.2.0/LICENSE` & `dask4dvc-0.2.1/LICENSE`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.2.0/README.md` & `dask4dvc-0.2.1/README.md`

 * *Files 7% similar despite different names*

```diff
@@ -5,14 +5,16 @@
 
 # Dask4DVC - Distributed Node Exectuion
 [DVC](dvc.org) provides tools for building and executing the computational graph locally through various methods. 
 The `dask4dvc` package combines [Dask Distributed](https://distributed.dask.org/) with DVC to make it easier to use with HPC managers like [Slurm](https://github.com/SchedMD/slurm).
 
 The `dask4dvc` package will try to run the DVC graph in parallel.
 
+> :warning: dask4dvc will disbale a few of the checks that DVC implements. Do not make changes to your workspace during the runtime of `dask4dvc repro`.
+
 ## Usage
 Dask4DVC provides a CLI similar to DVC.
 
 - `dvc repro` becomes `dask4dvc repro`.
 
 ### SLURM Cluster
```

### Comparing `dask4dvc-0.2.0/dask4dvc/__init__.py` & `dask4dvc-0.2.1/dask4dvc/__init__.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.2.0/dask4dvc/cli/main.py` & `dask4dvc-0.2.1/dask4dvc/cli/main.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 """All methods that come directly from 'dask4dvc' CLI interace."""
 
 import importlib.metadata
 import logging
 
 import dask.distributed
 import typer
-
+import typing
 from dask4dvc import methods, utils
 
 
 app = typer.Typer()
 
 log = logging.getLogger(__name__)
 
@@ -31,32 +31,34 @@
         "Maximum number of workers to use. Using '1' will be the same as 'dvc repro' but"
         " slower."
     )
 
 
 @app.command()
 def repro(
+    targets: typing.List[str] = typer.Argument(None),
     address: str = typer.Option(None, help=Help.address),
     leave: bool = typer.Option(True, help=Help.leave),
     config: str = typer.Option(None, help=Help.config),
     max_workers: int = typer.Option(None, help=Help.max_workers),
     retries: int = typer.Option(10, help=Help.retries),
+    force: bool = typer.Option(False, "--force/", "-f/", help="use `dvc repro --force`"),
 ) -> None:
     """Replicate 'dvc repro' command using dask."""
     utils.CONFIG.retries = retries
 
     if config is not None:
         assert address is None, "Can not use address and config file"
         address = utils.dask.get_cluster_from_config(config)
 
     with dask.distributed.Client(address) as client:
         if max_workers is not None:
             client.cluster.adapt(minimum=1, maximum=max_workers)
         log.info(client)
-        results = methods.parallel_submit(client)
+        results = methods.parallel_submit(client, targets=targets, force=force)
 
         utils.dask.wait_for_futures(results)
         if not leave:
             utils.main.wait()
 
 
 @app.command()
```

### Comparing `dask4dvc-0.2.0/dask4dvc/methods.py` & `dask4dvc-0.2.1/dask4dvc/methods.py`

 * *Files 22% similar despite different names*

```diff
@@ -1,16 +1,19 @@
 """Some general 'dask4dvc' methods."""
 
+
+import contextlib
 import typing
 import logging
 
 import dask.distributed
 import dvc.lock
 import dvc.exceptions
 import dvc.repo
+from dvc.repo.reproduce import _get_steps
 import dvc.utils.strictyaml
 import dvc.stage
 from dvc.stage.cache import RunCacheNotFoundError
 import random
 import time
 import subprocess
 
@@ -64,54 +67,79 @@
             repo.stage_cache.restore(stage=stage)
             log.info(
                 f"Stage '{stage.addressing}' is cached - skipping run, checking out"
                 " outputs "
             )
 
 
-def submit_stage(name: str, successors: list) -> str:
+def submit_stage(name: str, force: bool, successors: list) -> str:
     """Submit a stage to the Dask cluster."""
     repo = dvc.repo.Repo()
 
-    # dvc reproduce returns the stages that are not checked out
-    stages = _run_locked_cmd(repo, repo.reproduce, name, dry=True, single_item=True)
+    if force:
+        stages = [repo.stage.get_target(name)]
+    else:
+        # dvc reproduce returns the stages that are not checked out
+        stages = _run_locked_cmd(repo, repo.reproduce, name, dry=True, single_item=True)
 
-    if len(stages) == 0:
+    if len(stages) == 0 and not force:
         # if the stage is already checked out, we don't need to run it
         log.info(f"Stage '{name}' didn't change, skipping")
 
     else:
         if len(stages) > 1:
             # we use single-item, so it should never be more than 1
             raise ValueError("Something went wrong")
 
         for stage in stages:
-            try:
-                # check if the stage is already in the run cache
-                _run_locked_cmd(repo, _load_run_cache, repo, stages[0])
-            except RunCacheNotFoundError:
-                # if not, run the stage
-                log.info(f"Running stage '{name}': \n > {stage.cmd}")
-                subprocess.check_call(stage.cmd, shell=True)
-                # add the stage to the run cache
-                _run_locked_cmd(repo, repo.commit, name, force=True)
+            if not force:
+                with contextlib.suppress(RunCacheNotFoundError):
+                    # check if the stage is already in the run cache
+                    _run_locked_cmd(repo, _load_run_cache, repo, stages[0])
+                    return name
+            # if not, run the stage
+            log.info(f"Running stage '{name}': \n > {stage.cmd}")
+            subprocess.check_call(stage.cmd, shell=True)
+            # add the stage to the run cache
+            _run_locked_cmd(repo, repo.commit, name, force=True)
 
     return name
 
 
 def parallel_submit(
-    client: dask.distributed.Client,
+    client: dask.distributed.Client, targets: list[str], force: bool
 ) -> typing.Dict[str, dask.distributed.Future]:
     """Submit all stages to the Dask cluster."""
     mapping = {}
     repo = dvc.repo.Repo()
 
-    for node in repo.index.graph.nodes:
+    if len(targets) == 0:
+        targets = repo.index.graph.nodes
+    else:
+        targets = [repo.stage.get_target(x) for x in targets]
+
+    nodes = _get_steps(repo.index.graph, targets, downstream=False, single_item=False)
+
+    for node in nodes:
+        if node.cmd is None:
+            # if the stage doesn't have a command, e.g. a dvc tracked file
+            # we don't need to run it
+            mapping[node] = None
+            continue
         successors = [
             mapping[successor] for successor in repo.index.graph.successors(node)
         ]
 
         mapping[node] = client.submit(
-            submit_stage, node.name, successors=successors, pure=False
+            submit_stage,
+            node.addressing,
+            force=force,
+            successors=successors,
+            pure=False,
+            key=node.addressing,
         )
 
+    mapping = {
+        node.addressing: future for node, future in mapping.items() if future is not None
+    }
+
     return mapping
```

### Comparing `dask4dvc-0.2.0/dask4dvc/utils/dask.py` & `dask4dvc-0.2.1/dask4dvc/utils/dask.py`

 * *Files identical despite different names*

### Comparing `dask4dvc-0.2.0/pyproject.toml` & `dask4dvc-0.2.1/pyproject.toml`

 * *Files 12% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "dask4dvc"
-version = "0.2.0"
+version = "0.2.1"
 description = "Use dask to run the DVC graph"
 authors = ["zincwarecode <zincwarecode@gmail.com>"]
 license = "Apache-2.0"
 keywords=["data-science", "HPC", "dask", "DVC"]
 readme = "README.md"
 
 [tool.poetry.urls]
@@ -28,19 +28,18 @@
 black = "^22.6.0"
 isort = "^5.10.1"
 ruff = "^0.0.126"
 pytest = "^7.1.2"
 pytest-xdist = "^2.5.0"
 coverage = "^6.4.2"
 pre-commit = "^2.20.0"
-zntrack = "^0.4.0"	
 pylint = "^2.15.5"
-znlib = {extras = ["zntrack"], version = "^0.1.0"}
 
 # TODO remove znlib here!
+zntrack = {git = "https://github.com/zincware/zntrack"}
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
 
 
 [tool.black]
 line-length = 90
```

### Comparing `dask4dvc-0.2.0/PKG-INFO` & `dask4dvc-0.2.1/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dask4dvc
-Version: 0.2.0
+Version: 0.2.1
 Summary: Use dask to run the DVC graph
 License: Apache-2.0
 Keywords: data-science,HPC,dask,DVC
 Author: zincwarecode
 Author-email: zincwarecode@gmail.com
 Requires-Python: >=3.8,<4.0
 Classifier: License :: OSI Approved :: Apache Software License
@@ -29,14 +29,16 @@
 
 # Dask4DVC - Distributed Node Exectuion
 [DVC](dvc.org) provides tools for building and executing the computational graph locally through various methods. 
 The `dask4dvc` package combines [Dask Distributed](https://distributed.dask.org/) with DVC to make it easier to use with HPC managers like [Slurm](https://github.com/SchedMD/slurm).
 
 The `dask4dvc` package will try to run the DVC graph in parallel.
 
+> :warning: dask4dvc will disbale a few of the checks that DVC implements. Do not make changes to your workspace during the runtime of `dask4dvc repro`.
+
 ## Usage
 Dask4DVC provides a CLI similar to DVC.
 
 - `dvc repro` becomes `dask4dvc repro`.
 
 ### SLURM Cluster
```

