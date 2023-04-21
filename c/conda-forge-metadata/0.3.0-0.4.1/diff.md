# Comparing `tmp/conda-forge-metadata-0.3.0.tar.gz` & `tmp/conda-forge-metadata-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "conda-forge-metadata-0.3.0.tar", last modified: Sun Apr  9 12:25:49 2023, max compression
+gzip compressed data, was "conda-forge-metadata-0.4.1.tar", last modified: Fri Apr 21 21:32:13 2023, max compression
```

## Comparing `conda-forge-metadata-0.3.0.tar` & `conda-forge-metadata-0.4.1.tar`

### file list

```diff
@@ -1,40 +1,46 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:25:49.482450 conda-forge-metadata-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/.flake8
--rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/.git_archival.txt
--rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/.gitattributes
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:25:49.478450 conda-forge-metadata-0.3.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:25:49.478450 conda-forge-metadata-0.3.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/.github/workflows/pypi.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1910 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/.github/workflows/tests.yml
--rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-09 12:25:49.482450 conda-forge-metadata-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:25:49.478450 conda-forge-metadata-0.3.0/conda_forge_metadata/
--rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/conda_forge_metadata/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-09 12:25:49.000000 conda-forge-metadata-0.3.0/conda_forge_metadata/_version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:25:49.478450 conda-forge-metadata-0.3.0/conda_forge_metadata/artifact_info/
--rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/conda_forge_metadata/artifact_info/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1545 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/conda_forge_metadata/artifact_info/info_json.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:25:49.482450 conda-forge-metadata-0.3.0/conda_forge_metadata/autotick_bot/
--rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/conda_forge_metadata/autotick_bot/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1118 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/conda_forge_metadata/autotick_bot/import_to_pkg.py
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/conda_forge_metadata/autotick_bot/pypi_to_conda.py
--rw-r--r--   0 runner    (1001) docker     (123)     5134 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/conda_forge_metadata/libcfgraph.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:25:49.478450 conda-forge-metadata-0.3.0/conda_forge_metadata.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     2296 2023-04-09 12:25:49.000000 conda-forge-metadata-0.3.0/conda_forge_metadata.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      874 2023-04-09 12:25:49.000000 conda-forge-metadata-0.3.0/conda_forge_metadata.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-09 12:25:49.000000 conda-forge-metadata-0.3.0/conda_forge_metadata.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-09 12:25:49.000000 conda-forge-metadata-0.3.0/conda_forge_metadata.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-09 12:25:49.000000 conda-forge-metadata-0.3.0/conda_forge_metadata.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      701 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/requirements-dev.txt
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:25:49.482450 conda-forge-metadata-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-09 12:25:49.482450 conda-forge-metadata-0.3.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/tests/test_alive.py
--rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/tests/test_libcfgraph.py
--rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/tests/test_map_import_to_package.py
--rw-r--r--   0 runner    (1001) docker     (123)      414 2023-04-09 12:25:33.000000 conda-forge-metadata-0.3.0/tests/test_map_pypi_to_conda.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/
+-rw-r--r--   0 runner    (1001) docker     (123)       51 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.flake8
+-rw-r--r--   0 runner    (1001) docker     (123)      111 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.git_archival.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       32 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.gitattributes
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.247955 conda-forge-metadata-0.4.1/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.251955 conda-forge-metadata-0.4.1/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      314 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.github/workflows/pre-commit.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1142 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.github/workflows/pypi.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1811 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.github/workflows/tests.yml
+-rw-r--r--   0 runner    (1001) docker     (123)     1832 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)     1867 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     1505 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       82 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      240 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.251955 conda-forge-metadata-0.4.1/conda_forge_metadata/
+-rw-r--r--   0 runner    (1001) docker     (123)       42 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       22 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/_version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/conda_forge_metadata/artifact_info/
+-rw-r--r--   0 runner    (1001) docker     (123)       57 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/artifact_info/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1829 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/artifact_info/info_json.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/
+-rw-r--r--   0 runner    (1001) docker     (123)      133 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1120 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/import_to_pkg.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1023 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/pypi_to_conda.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2105 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/feedstock_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5117 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/libcfgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3903 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/conda_forge_metadata/oci.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     2316 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1057 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       45 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-21 21:32:13.000000 conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       83 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/requirements-dev.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/requirements.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 21:32:13.255955 conda-forge-metadata-0.4.1/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)      104 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_alive.py
+-rw-r--r--   0 runner    (1001) docker     (123)      288 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_feedstock_outputs.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1131 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_info_json.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1351 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_libcfgraph.py
+-rw-r--r--   0 runner    (1001) docker     (123)      359 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_map_import_to_package.py
+-rw-r--r--   0 runner    (1001) docker     (123)      406 2023-04-21 21:31:50.000000 conda-forge-metadata-0.4.1/tests/test_map_pypi_to_conda.py
```

### Comparing `conda-forge-metadata-0.3.0/.github/workflows/pypi.yml` & `conda-forge-metadata-0.4.1/.github/workflows/pypi.yml`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.3.0/.github/workflows/tests.yml` & `conda-forge-metadata-0.4.1/.github/workflows/tests.yml`

 * *Files 22% similar despite different names*

```diff
@@ -25,22 +25,23 @@
           show-channel-urls: true
           miniforge-version: latest
           miniforge-variant: Mambaforge
           python-version: 3.9
           use-mamba: true
 
       - name: configure conda and install code
-        shell: bash -l {0}
+        shell: bash -el {0}
         run: |
-          mamba install --yes --file=requirements.txt
-          mamba install --yes --file=requirements-dev.txt
+          mamba install --yes \
+            --file=requirements.txt \
+            --file=requirements-dev.txt
           python -m pip install -v --no-deps --no-build-isolation -e .
 
       - name: test versions
-        shell: bash -l {0}
+        shell: bash -el {0}
         run: |
           pip uninstall conda-forge-metadata --yes
           [[ $(python setup.py --version) != "0.0.0" ]] || exit 1
 
           rm -rf dist/*
           python setup.py sdist
           pip install --no-deps --no-build-isolation dist/*.tar.gz
@@ -55,16 +56,11 @@
           pushd ..
           python -c "import conda_forge_metadata; assert conda_forge_metadata.__version__ != '0.0.0'"
           popd
           pip uninstall conda-forge-metadata --yes
 
           python -m pip install -v --no-deps --no-build-isolation -e .
 
-      - name: lint
-        shell: bash -l {0}
-        run: |
-          flake8 conda_forge_metadata
-
       - name: test
-        shell: bash -l {0}
+        shell: bash -el {0}
         run: |
           pytest -vvs tests
```

### Comparing `conda-forge-metadata-0.3.0/.gitignore` & `conda-forge-metadata-0.4.1/.gitignore`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.3.0/LICENSE` & `conda-forge-metadata-0.4.1/LICENSE`

 * *Files identical despite different names*

### Comparing `conda-forge-metadata-0.3.0/PKG-INFO` & `conda-forge-metadata-0.4.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-forge-metadata
-Version: 0.3.0
+Version: 0.4.1
 Summary: programatic access to conda-forge's metadata
 Author-email: conda-forge-tick development team <condaforge@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Re(search) Gro(up)
         
         Redistribution and use in source and binary forms, with or without
@@ -30,13 +30,14 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: home, https://github.com/regro/conda-forge-metadata
 Description-Content-Type: text/markdown
+Provides-Extra: oci
 License-File: LICENSE
 
 # conda-forge-metadata
 [![tests](https://github.com/regro/conda-forge-metadata/actions/workflows/tests.yml/badge.svg)](https://github.com/regro/conda-forge-metadata/actions/workflows/tests.yml)
 
 programatic access to conda-forge's metadata
```

### Comparing `conda-forge-metadata-0.3.0/conda_forge_metadata/artifact_info/info_json.py` & `conda-forge-metadata-0.4.1/conda_forge_metadata/artifact_info/info_json.py`

 * *Files 13% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from conda_forge_metadata.libcfgraph import get_libcfgraph_artifact_data
 
 
-def get_artifact_info_as_json(channel, subdir, artifact):
+def get_artifact_info_as_json(channel, subdir, artifact, backend="libcfgraph"):
     """Get a blob of artifact data from the conda info directory.
 
     Parameters
     ----------
     channel : str
         The channel (e.g., "conda-forge").
     subdir : str
@@ -31,8 +31,15 @@
                 info/recipe/meta.yaml.template - could be
                 the rendered recipe as a string if no template was found
             "conda_build_config": the conda_build_config.yaml used for building
                 the recipe at info/recipe/conda_build_config.yaml
             "files": a list of files in the recipe from info/files with
                 elements ending in .pyc or .txt filtered out.
     """
-    return get_libcfgraph_artifact_data(channel, subdir, artifact)
+    if backend == "libcfgraph":
+        return get_libcfgraph_artifact_data(channel, subdir, artifact)
+    elif backend == "oci":
+        from conda_forge_metadata.oci import get_oci_artifact_data
+
+        return get_oci_artifact_data(channel, subdir, artifact)
+    else:
+        raise ValueError(f"Unknown backend {backend!r}")
```

### Comparing `conda-forge-metadata-0.3.0/conda_forge_metadata/autotick_bot/import_to_pkg.py` & `conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/import_to_pkg.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,18 +1,19 @@
 from functools import lru_cache
+
 import requests
 
 from conda_forge_metadata.libcfgraph import get_libcfgraph_pkgs_for_import
 
 
 @lru_cache(maxsize=1)
 def _ranked_hubs_authorities():
     req = requests.get(
-        'https://raw.githubusercontent.com/regro/cf-graph-countyfair/'
-        'master/ranked_hubs_authorities.json'
+        "https://raw.githubusercontent.com/regro/cf-graph-countyfair/"
+        "master/ranked_hubs_authorities.json"
     )
     req.raise_for_status()
     return req.json()
 
 
 def map_import_to_package(import_name):
     """Map an import name to the most likely package that has it.
@@ -34,9 +35,9 @@
     if found_import_name in supplying_pkgs:
         # heuristic that import scipy comes from scipy
         return found_import_name
     else:
         hubs_auths = _ranked_hubs_authorities()
         return next(
             iter(k for k in hubs_auths if k in supplying_pkgs),
-            found_import_name
+            found_import_name,
         )
```

### Comparing `conda-forge-metadata-0.3.0/conda_forge_metadata/autotick_bot/pypi_to_conda.py` & `conda-forge-metadata-0.4.1/conda_forge_metadata/autotick_bot/pypi_to_conda.py`

 * *Files 23% similar despite different names*

```diff
@@ -1,20 +1,21 @@
 from functools import lru_cache
+
 import requests
-import yaml
+from ruamel import yaml
 
 
 @lru_cache(maxsize=1)
 def get_pypi_name_mapping():
     req = requests.get(
         "https://raw.githubusercontent.com/regro/cf-graph-countyfair/"
         "master/mappings/pypi/name_mapping.yaml"
     )
     req.raise_for_status()
-    return yaml.safe_load(req.text)
+    return yaml.YAML(typ="safe").load(req.text)
 
 
 @lru_cache(maxsize=1)
 def _grayskull_pypi_mapping():
     req = requests.get(
         "https://raw.githubusercontent.com/regro/cf-graph-countyfair/"
         "master/mappings/pypi/grayskull_pypi_mapping.json"
```

### Comparing `conda-forge-metadata-0.3.0/conda_forge_metadata/libcfgraph.py` & `conda-forge-metadata-0.4.1/conda_forge_metadata/libcfgraph.py`

 * *Files 3% similar despite different names*

```diff
@@ -1,8 +1,9 @@
 from functools import lru_cache
+
 import requests
 
 _LIBCFGRAPH_INDEX = None
 
 
 def _download_libcfgraph_index():
     global _LIBCFGRAPH_INDEX
@@ -80,18 +81,15 @@
     #   artifacts/21cmfast/conda-forge/osx-64/21cmfast-3.0.2-py36h13dd421_0.json
     nm_parts = artifact.rsplit("-", 2)
     if artifact.endswith(".tar.bz2"):
         nm = artifact[: -len(".tar.bz2")]
     else:
         nm = artifact[: -len(".conda")]
 
-    libcfgraph_path = (
-        "artifacts/"
-        f"{nm_parts[0]}/{channel}/{subdir}/{nm}.json"
-    )
+    libcfgraph_path = "artifacts/" f"{nm_parts[0]}/{channel}/{subdir}/{nm}.json"
     if libcfgraph_path in get_libcfgraph_index():
         url = (
             "https://raw.githubusercontent.com/regro/libcfgraph/master/"
             + libcfgraph_path
         )
         r = requests.get(url)
         r.raise_for_status()
@@ -99,33 +97,34 @@
     else:
         return None
 
 
 @lru_cache(maxsize=1)
 def _import_to_pkg_maps_num_letters():
     req = requests.get(
-        'https://raw.githubusercontent.com/regro/libcfgraph/master'
-        '/import_to_pkg_maps_meta.json'
+        "https://raw.githubusercontent.com/regro/libcfgraph/master"
+        "/import_to_pkg_maps_meta.json"
     )
     req.raise_for_status()
-    return int(req.json()['num_letters'])
+    return int(req.json()["num_letters"])
 
 
 @lru_cache(maxsize=128)
 def _import_to_pkg_maps_cache(import_first_letters):
     req = requests.get(
-        f'https://raw.githubusercontent.com/regro/libcfgraph'
-        f'/master/import_to_pkg_maps/{import_first_letters.lower()}.json')
+        f"https://raw.githubusercontent.com/regro/libcfgraph"
+        f"/master/import_to_pkg_maps/{import_first_letters.lower()}.json"
+    )
     req.raise_for_status()
-    return {k: set(v['elements']) for k, v in req.json().items()}
+    return {k: set(v["elements"]) for k, v in req.json().items()}
 
 
 def _get_libcfgraph_pkgs_for_import(import_name):
     num_letters = _import_to_pkg_maps_num_letters()
-    fllt = import_name[:min(len(import_name), num_letters)]
+    fllt = import_name[: min(len(import_name), num_letters)]
     import_to_pkg_map = _import_to_pkg_maps_cache(fllt)
     return import_to_pkg_map.get(import_name, None)
 
 
 def get_libcfgraph_pkgs_for_import(import_name):
     """Get a list of possible packages that supply a given import.
 
@@ -149,10 +148,10 @@
         Will return `None` if the import was not found.
     found_import_name : str
         The import name found in the libcfgraph metadata. Only
         valid if `packages` is not None. This name will be the
         top-level import with all subpackages removed (e.g., foo.bar.baz
         will be returned as foo).
     """
-    import_name = import_name.split('.')[0]
+    import_name = import_name.split(".")[0]
     supplying_pkgs = _get_libcfgraph_pkgs_for_import(import_name)
     return supplying_pkgs, import_name
```

### Comparing `conda-forge-metadata-0.3.0/conda_forge_metadata.egg-info/PKG-INFO` & `conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: conda-forge-metadata
-Version: 0.3.0
+Version: 0.4.1
 Summary: programatic access to conda-forge's metadata
 Author-email: conda-forge-tick development team <condaforge@gmail.com>
 License: BSD 3-Clause License
         
         Copyright (c) 2023, Re(search) Gro(up)
         
         Redistribution and use in source and binary forms, with or without
@@ -30,13 +30,14 @@
         SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER
         CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY,
         OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE
         OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
         
 Project-URL: home, https://github.com/regro/conda-forge-metadata
 Description-Content-Type: text/markdown
+Provides-Extra: oci
 License-File: LICENSE
 
 # conda-forge-metadata
 [![tests](https://github.com/regro/conda-forge-metadata/actions/workflows/tests.yml/badge.svg)](https://github.com/regro/conda-forge-metadata/actions/workflows/tests.yml)
 
 programatic access to conda-forge's metadata
```

### Comparing `conda-forge-metadata-0.3.0/conda_forge_metadata.egg-info/SOURCES.txt` & `conda-forge-metadata-0.4.1/conda_forge_metadata.egg-info/SOURCES.txt`

 * *Files 13% similar despite different names*

```diff
@@ -1,30 +1,36 @@
 .flake8
 .git_archival.txt
 .gitattributes
 .gitignore
+.pre-commit-config.yaml
 LICENSE
 MANIFEST.in
 README.md
 pyproject.toml
 requirements-dev.txt
 requirements.txt
 setup.py
+.github/workflows/pre-commit.yml
 .github/workflows/pypi.yml
 .github/workflows/tests.yml
 conda_forge_metadata/__init__.py
 conda_forge_metadata/_version.py
+conda_forge_metadata/feedstock_outputs.py
 conda_forge_metadata/libcfgraph.py
+conda_forge_metadata/oci.py
 conda_forge_metadata.egg-info/PKG-INFO
 conda_forge_metadata.egg-info/SOURCES.txt
 conda_forge_metadata.egg-info/dependency_links.txt
 conda_forge_metadata.egg-info/requires.txt
 conda_forge_metadata.egg-info/top_level.txt
 conda_forge_metadata/artifact_info/__init__.py
 conda_forge_metadata/artifact_info/info_json.py
 conda_forge_metadata/autotick_bot/__init__.py
 conda_forge_metadata/autotick_bot/import_to_pkg.py
 conda_forge_metadata/autotick_bot/pypi_to_conda.py
 tests/test_alive.py
+tests/test_feedstock_outputs.py
+tests/test_info_json.py
 tests/test_libcfgraph.py
 tests/test_map_import_to_package.py
 tests/test_map_pypi_to_conda.py
```

### Comparing `conda-forge-metadata-0.3.0/pyproject.toml` & `conda-forge-metadata-0.4.1/pyproject.toml`

 * *Files 7% similar despite different names*

```diff
@@ -11,21 +11,29 @@
 authors = [
     {name = "conda-forge-tick development team", email = "condaforge@gmail.com"},
 ]
 description = "programatic access to conda-forge's metadata"
 dynamic = ["version"]
 dependencies = [
     "requests",
-    "pyyaml"
+    "ruamel.yaml"
 ]
 license = {file = "LICENSE"}
 readme = "README.md"
 
+[project.optional-dependencies]
+oci = [
+  "conda-oci-mirror"
+]
+
 [project.urls]
 home = "https://github.com/regro/conda-forge-metadata"
 
 [tool.setuptools_scm]
 write_to = "conda_forge_metadata/_version.py"
 write_to_template = "__version__ = '{version}'\n"
 
 [tool.black]
-line-length = 79
+line-length = 88
+
+[tool.isort]
+profile = "black"
```

### Comparing `conda-forge-metadata-0.3.0/tests/test_libcfgraph.py` & `conda-forge-metadata-0.4.1/tests/test_libcfgraph.py`

 * *Ordering differences only*

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 from conda_forge_metadata.libcfgraph import (
-    get_libcfgraph_pkgs_for_import,
-    get_libcfgraph_index,
     get_libcfgraph_artifact_data,
+    get_libcfgraph_index,
+    get_libcfgraph_pkgs_for_import,
 )
 
 
 def test_get_libcfgraph_index():
     lcfi = get_libcfgraph_index()
     assert len(lcfi) > 0
     assert isinstance(lcfi, list)
```

