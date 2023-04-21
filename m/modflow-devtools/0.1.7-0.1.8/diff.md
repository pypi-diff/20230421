# Comparing `tmp/modflow-devtools-0.1.7.tar.gz` & `tmp/modflow-devtools-0.1.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "modflow-devtools-0.1.7.tar", last modified: Tue Apr 18 21:06:43 2023, max compression
+gzip compressed data, was "modflow-devtools-0.1.8.tar", last modified: Fri Apr 21 19:45:24 2023, max compression
```

## Comparing `modflow-devtools-0.1.7.tar` & `modflow-devtools-0.1.8.tar`

### file list

```diff
@@ -1,37 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:43.617777 modflow-devtools-0.1.7/
--rwxr-xr-x   0 runner    (1001) docker     (123)     1627 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/LICENSE.md
--rw-r--r--   0 runner    (1001) docker     (123)      163 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-18 21:06:43.617777 modflow-devtools-0.1.7/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     3856 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:43.613777 modflow-devtools-0.1.7/modflow_devtools/
--rw-r--r--   0 runner    (1001) docker     (123)      248 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      984 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1029 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/case.py
--rw-r--r--   0 runner    (1001) docker     (123)     7352 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/context.py
--rw-r--r--   0 runner    (1001) docker     (123)    17531 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/download.py
--rw-r--r--   0 runner    (1001) docker     (123)     2487 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/executables.py
--rw-r--r--   0 runner    (1001) docker     (123)    10981 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)     1732 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/markers.py
--rw-r--r--   0 runner    (1001) docker     (123)    10007 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/misc.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:43.617777 modflow-devtools-0.1.7/modflow_devtools/test/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1163 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_build.py
--rw-r--r--   0 runner    (1001) docker     (123)     1788 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_case.py
--rw-r--r--   0 runner    (1001) docker     (123)     3606 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_download.py
--rw-r--r--   0 runner    (1001) docker     (123)     1148 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_executables.py
--rw-r--r--   0 runner    (1001) docker     (123)     8043 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_fixtures.py
--rw-r--r--   0 runner    (1001) docker     (123)      904 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_markers.py
--rw-r--r--   0 runner    (1001) docker     (123)     8053 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_misc.py
--rw-r--r--   0 runner    (1001) docker     (123)     2663 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/test/test_zip.py
--rw-r--r--   0 runner    (1001) docker     (123)     5708 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/modflow_devtools/zip.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 21:06:43.613777 modflow-devtools-0.1.7/modflow_devtools.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     5069 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      913 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 21:06:31.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)      235 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       17 2023-04-18 21:06:43.000000 modflow-devtools-0.1.7/modflow_devtools.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)     2182 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 21:06:43.617777 modflow-devtools-0.1.7/setup.cfg
--rwxr-xr-x   0 runner    (1001) docker     (123)       61 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/setup.py
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-18 21:06:17.000000 modflow-devtools-0.1.7/version.txt
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-04-21 19:45:24.210920 modflow-devtools-0.1.8/
+-rwxr-xr-x   0 wes        (501) staff       (20)     1627 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/LICENSE.md
+-rw-r--r--   0 wes        (501) staff       (20)      163 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/MANIFEST.in
+-rw-r--r--   0 wes        (501) staff       (20)     5069 2023-04-21 19:45:24.210424 modflow-devtools-0.1.8/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)     3856 2023-04-18 20:59:23.000000 modflow-devtools-0.1.8/README.md
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-04-21 19:45:24.165680 modflow-devtools-0.1.8/modflow_devtools/
+-rw-r--r--   0 wes        (501) staff       (20)      248 2023-04-21 13:48:06.000000 modflow-devtools-0.1.8/modflow_devtools/__init__.py
+-rw-r--r--   0 wes        (501) staff       (20)      984 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/build.py
+-rw-r--r--   0 wes        (501) staff       (20)     1029 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/case.py
+-rw-r--r--   0 wes        (501) staff       (20)     7352 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/context.py
+-rw-r--r--   0 wes        (501) staff       (20)    17531 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/download.py
+-rw-r--r--   0 wes        (501) staff       (20)     2487 2023-04-18 20:59:23.000000 modflow-devtools-0.1.8/modflow_devtools/executables.py
+-rw-r--r--   0 wes        (501) staff       (20)    11854 2023-04-21 19:36:54.000000 modflow-devtools-0.1.8/modflow_devtools/fixtures.py
+-rw-r--r--   0 wes        (501) staff       (20)     1732 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/markers.py
+-rw-r--r--   0 wes        (501) staff       (20)    10007 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/misc.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-04-21 19:45:24.207602 modflow-devtools-0.1.8/modflow_devtools/test/
+-rw-r--r--   0 wes        (501) staff       (20)        0 2022-11-03 17:55:40.000000 modflow-devtools-0.1.8/modflow_devtools/test/__init__.py
+-rw-r--r--   0 wes        (501) staff       (20)     1163 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_build.py
+-rw-r--r--   0 wes        (501) staff       (20)     1788 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_case.py
+-rw-r--r--   0 wes        (501) staff       (20)     3606 2023-04-21 19:36:54.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_download.py
+-rw-r--r--   0 wes        (501) staff       (20)     1148 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_executables.py
+-rw-r--r--   0 wes        (501) staff       (20)     8043 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_fixtures.py
+-rw-r--r--   0 wes        (501) staff       (20)      904 2022-11-03 18:33:54.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_markers.py
+-rw-r--r--   0 wes        (501) staff       (20)     8053 2023-04-21 16:21:19.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_misc.py
+-rw-r--r--   0 wes        (501) staff       (20)     2663 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/test/test_zip.py
+-rw-r--r--   0 wes        (501) staff       (20)     5708 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/modflow_devtools/zip.py
+drwxr-xr-x   0 wes        (501) staff       (20)        0 2023-04-21 19:45:24.171718 modflow-devtools-0.1.8/modflow_devtools.egg-info/
+-rw-r--r--   0 wes        (501) staff       (20)     5069 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/PKG-INFO
+-rw-r--r--   0 wes        (501) staff       (20)      913 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/SOURCES.txt
+-rw-r--r--   0 wes        (501) staff       (20)        1 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/dependency_links.txt
+-rw-r--r--   0 wes        (501) staff       (20)        1 2022-07-22 15:19:26.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/not-zip-safe
+-rw-r--r--   0 wes        (501) staff       (20)      235 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/requires.txt
+-rw-r--r--   0 wes        (501) staff       (20)       17 2023-04-21 19:45:24.000000 modflow-devtools-0.1.8/modflow_devtools.egg-info/top_level.txt
+-rw-r--r--   0 wes        (501) staff       (20)     2182 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/pyproject.toml
+-rw-r--r--   0 wes        (501) staff       (20)       38 2023-04-21 19:45:24.211042 modflow-devtools-0.1.8/setup.cfg
+-rwxr-xr-x   0 wes        (501) staff       (20)       61 2023-02-11 16:50:42.000000 modflow-devtools-0.1.8/setup.py
+-rw-r--r--   0 wes        (501) staff       (20)        5 2023-04-21 13:48:06.000000 modflow-devtools-0.1.8/version.txt
```

### Comparing `modflow-devtools-0.1.7/LICENSE.md` & `modflow-devtools-0.1.8/LICENSE.md`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/PKG-INFO` & `modflow-devtools-0.1.8/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
```

### Comparing `modflow-devtools-0.1.7/README.md` & `modflow-devtools-0.1.8/README.md`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/build.py` & `modflow-devtools-0.1.8/modflow_devtools/build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/case.py` & `modflow-devtools-0.1.8/modflow_devtools/case.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/context.py` & `modflow-devtools-0.1.8/modflow_devtools/context.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/download.py` & `modflow-devtools-0.1.8/modflow_devtools/download.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/executables.py` & `modflow-devtools-0.1.8/modflow_devtools/executables.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/fixtures.py` & `modflow-devtools-0.1.8/modflow_devtools/fixtures.py`

 * *Files 8% similar despite different names*

```diff
@@ -186,79 +186,97 @@
 
     # user can specify a path to folder containing model repos
     repos_path = environ.get("REPOS_PATH")
     if repos_path is not None:
         repos_path = Path(repos_path)
     else:
         # by default, assume external repositories are
-        # in the same directory as the current project
-        # and tests are run from <proj root>/autotest.
-        # if no models are found, tests requesting the
-        # fixtures will be skipped.
+        # level (side-by-side) on the filesystem with
+        # the consuming project. also assume tests are
+        # run from <proj root>/autotest.
+        #
+        # external model repo directories are expected
+        # to be named identically to the GitHub repos,
+        # e.g. "modflow6-testmodels", with an optional
+        # ".git" suffix appended to the directory name.
+        #
+        # if model repositories are not found in either
+        # the default location or in REPOS_PATH, tests
+        # requesting these fixtures will be skipped.
         repos_path = Path.cwd().parent.parent
 
+    def get_repo_path(repo_name: str) -> Optional[Path]:
+        """Get the path for the repository with the given name
+        (optionally with .git suffix), or None if not found"""
+        repo_path = repos_path / repo_name
+        if not repo_path.is_dir():
+            repo_path = repos_path / (repo_name + ".git")
+        if not repo_path.is_dir():
+            repo_path = None
+        return repo_path
+
     key = "test_model_mf6"
     if key in metafunc.fixturenames:
-        repo_path = repos_path / "modflow6-testmodels"
+        repo_path = get_repo_path("modflow6-testmodels")
         namefile_paths = (
             get_namefile_paths(
                 repo_path / "mf6",
                 prefix="test",
                 excluded=[],
                 selected=models_selected,
                 packages=packages_selected,
             )
-            if repo_path.is_dir()
+            if repo_path
             else []
         )
         metafunc.parametrize(
             key, namefile_paths, ids=[str(m) for m in namefile_paths]
         )
 
     key = "test_model_mf5to6"
     if key in metafunc.fixturenames:
-        repo_path = repos_path / "modflow6-testmodels"
+        repo_path = get_repo_path("modflow6-testmodels")
         namefile_paths = (
             get_namefile_paths(
                 repo_path / "mf5to6",
                 prefix="test",
                 namefile="*.nam",
                 excluded=[],
                 selected=models_selected,
                 packages=packages_selected,
             )
-            if repo_path.is_dir()
+            if repo_path
             else []
         )
         metafunc.parametrize(
             key, namefile_paths, ids=[str(m) for m in namefile_paths]
         )
 
     key = "large_test_model"
     if key in metafunc.fixturenames:
-        repo_path = repos_path / "modflow6-largetestmodels"
+        repo_path = get_repo_path("modflow6-largetestmodels")
         namefile_paths = (
             get_namefile_paths(
                 repo_path,
                 prefix="test",
                 namefile="mfsim.nam",
                 excluded=[],
                 selected=models_selected,
                 packages=packages_selected,
             )
-            if repo_path.is_dir()
+            if repo_path
             else []
         )
         metafunc.parametrize(
             key, namefile_paths, ids=[str(m) for m in namefile_paths]
         )
 
     key = "example_scenario"
     if key in metafunc.fixturenames:
-        repo_path = repos_path / "modflow6-examples"
+        repo_path = get_repo_path("modflow6-examples")
 
         def is_nested(namfile_path: PathLike) -> bool:
             p = Path(namfile_path)
             if not p.is_file() or not p.name.endswith(".nam"):
                 raise ValueError(f"Expected namefile path, got {p}")
 
             return p.parent.parent.name != "examples"
@@ -287,15 +305,20 @@
 
                 d[name] = nfpaths
 
             return d
 
         def get_examples():
             # find MODFLOW 6 namfiles
-            namfiles = [p for p in (repo_path / "examples").rglob("mfsim.nam")]
+            examples_path = repo_path / "examples"
+            namfiles = (
+                [p for p in examples_path.rglob("mfsim.nam")]
+                if examples_path.is_dir()
+                else []
+            )
 
             # group by scenario
             examples = group_examples(namfiles)
 
             # filter by example name (optional)
             if models_selected:
                 examples = {
@@ -330,13 +353,13 @@
                 name: nfps
                 for name, nfps in examples.items()
                 if name not in ["mf6gwf", "mf6gwt"]
             }
 
             return examples
 
-        example_scenarios = get_examples() if repo_path.is_dir() else dict()
+        example_scenarios = get_examples() if repo_path else dict()
         metafunc.parametrize(
             key,
             [(name, nfps) for name, nfps in example_scenarios.items()],
             ids=[name for name, ex in example_scenarios.items()],
         )
```

### Comparing `modflow-devtools-0.1.7/modflow_devtools/markers.py` & `modflow-devtools-0.1.8/modflow_devtools/markers.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/misc.py` & `modflow-devtools-0.1.8/modflow_devtools/misc.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/test/test_build.py` & `modflow-devtools-0.1.8/modflow_devtools/test/test_build.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/test/test_case.py` & `modflow-devtools-0.1.8/modflow_devtools/test/test_case.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/test/test_download.py` & `modflow-devtools-0.1.8/modflow_devtools/test/test_download.py`

 * *Files 0% similar despite different names*

```diff
@@ -65,15 +65,15 @@
 @pytest.mark.parametrize("name", [None, "rtd-files", "run-time-comparison"])
 @pytest.mark.parametrize("per_page", [None, 100])
 def test_list_artifacts(tmp_path, name, per_page):
     artifacts = list_artifacts(
         "MODFLOW-USGS/modflow6",
         name=name,
         per_page=per_page,
-        max_pages=3,
+        max_pages=2,
         verbose=True,
     )
 
     if any(artifacts) and name:
         assert all(name == a["name"] for a in artifacts)
```

### Comparing `modflow-devtools-0.1.7/modflow_devtools/test/test_executables.py` & `modflow-devtools-0.1.8/modflow_devtools/test/test_executables.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/test/test_fixtures.py` & `modflow-devtools-0.1.8/modflow_devtools/test/test_fixtures.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/test/test_markers.py` & `modflow-devtools-0.1.8/modflow_devtools/test/test_markers.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/test/test_misc.py` & `modflow-devtools-0.1.8/modflow_devtools/test/test_misc.py`

 * *Files 0% similar despite different names*

```diff
@@ -158,15 +158,15 @@
 
 
 @pytest.mark.skipif(
     not any(_largetestmodel_paths) or not any(_example_paths),
     reason="repos not found",
 )
 @pytest.mark.parametrize(
-    "models", [(_examples_path, 63), (_largetestmodels_repo_path, 15)]
+    "models", [(_examples_path, 63), (_largetestmodels_repo_path, 16)]
 )
 def test_get_model_paths_exclude_patterns(models):
     path, expected_count = models
     paths = get_model_paths(path, excluded=["gwt"])
     assert len(paths) == expected_count
 
 
@@ -201,15 +201,15 @@
 
 
 @pytest.mark.skipif(
     not any(_largetestmodel_paths) or not any(_example_paths),
     reason="repos not found",
 )
 @pytest.mark.parametrize(
-    "models", [(_examples_path, 43), (_largetestmodels_repo_path, 18)]
+    "models", [(_examples_path, 43), (_largetestmodels_repo_path, 19)]
 )
 def test_get_namefile_paths_exclude_patterns(models):
     path, expected_count = models
     paths = get_namefile_paths(path, excluded=["gwf"])
     assert len(paths) == expected_count
```

### Comparing `modflow-devtools-0.1.7/modflow_devtools/test/test_zip.py` & `modflow-devtools-0.1.8/modflow_devtools/test/test_zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools/zip.py` & `modflow-devtools-0.1.8/modflow_devtools/zip.py`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/modflow_devtools.egg-info/PKG-INFO` & `modflow-devtools-0.1.8/modflow_devtools.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: modflow-devtools
-Version: 0.1.7
+Version: 0.1.8
 Summary: Python tools for MODFLOW development
 Author-email: "Joseph D. Hughes" <modflow@usgs.gov>
 Maintainer-email: "Joseph D. Hughes" <modflow@usgs.gov>
 License: CC0
 Project-URL: Documentation, https://modflow-devtools.readthedocs.io/en/latest/
 Project-URL: Bug Tracker, https://github.com/MODFLOW-USGS/modflow-devtools/issues
 Project-URL: Source Code, https://github.com/MODFLOW-USGS/modflow-devtools
```

### Comparing `modflow-devtools-0.1.7/modflow_devtools.egg-info/SOURCES.txt` & `modflow-devtools-0.1.8/modflow_devtools.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `modflow-devtools-0.1.7/pyproject.toml` & `modflow-devtools-0.1.8/pyproject.toml`

 * *Files identical despite different names*

