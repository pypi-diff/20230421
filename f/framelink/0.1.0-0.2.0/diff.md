# Comparing `tmp/framelink-0.1.0.tar.gz` & `tmp/framelink-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "framelink-0.1.0.tar", last modified: Thu Mar 23 23:13:17 2023, max compression
+gzip compressed data, was "framelink-0.2.0.tar", last modified: Fri Apr 21 02:45:32 2023, max compression
```

## Comparing `framelink-0.1.0.tar` & `framelink-0.2.0.tar`

### file list

```diff
@@ -1,28 +1,42 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:13:17.321096 framelink-0.1.0/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:13:17.317096 framelink-0.1.0/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:13:17.321096 framelink-0.1.0/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)     1666 2023-03-23 23:12:37.000000 framelink-0.1.0/.github/workflows/lint_test_build.yml
--rw-r--r--   0 runner    (1001) docker     (123)      162 2023-03-23 23:12:37.000000 framelink-0.1.0/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)      582 2023-03-23 23:12:37.000000 framelink-0.1.0/.pre-commit-config.yaml
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-23 23:13:17.321096 framelink-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      105 2023-03-23 23:12:37.000000 framelink-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:13:17.321096 framelink-0.1.0/data/
--rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-03-23 23:12:37.000000 framelink-0.1.0/data/divy_trips_limited.csv
--rw-r--r--   0 runner    (1001) docker     (123)   102165 2023-03-23 23:12:37.000000 framelink-0.1.0/pdm.lock
--rw-r--r--   0 runner    (1001) docker     (123)     1095 2023-03-23 23:12:37.000000 framelink-0.1.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)    18217 2023-03-23 23:12:37.000000 framelink-0.1.0/requirements.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-03-23 23:13:17.321096 framelink-0.1.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:13:17.317096 framelink-0.1.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:13:17.321096 framelink-0.1.0/src/framelink/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 23:12:37.000000 framelink-0.1.0/src/framelink/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      160 2023-03-23 23:13:17.000000 framelink-0.1.0/src/framelink/__version__.py
--rw-r--r--   0 runner    (1001) docker     (123)     4147 2023-03-23 23:12:37.000000 framelink-0.1.0/src/framelink/core.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:13:17.321096 framelink-0.1.0/src/framelink.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-03-23 23:13:17.000000 framelink-0.1.0/src/framelink.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      455 2023-03-23 23:13:17.000000 framelink-0.1.0/src/framelink.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-03-23 23:13:17.000000 framelink-0.1.0/src/framelink.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      222 2023-03-23 23:13:17.000000 framelink-0.1.0/src/framelink.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       10 2023-03-23 23:13:17.000000 framelink-0.1.0/src/framelink.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-03-23 23:13:17.321096 framelink-0.1.0/tests/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-03-23 23:12:37.000000 framelink-0.1.0/tests/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     1884 2023-03-23 23:12:37.000000 framelink-0.1.0/tests/test_core_model.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.235062 framelink-0.2.0/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)     1743 2023-04-21 02:44:18.000000 framelink-0.2.0/.github/workflows/lint_test_build.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      255 2023-04-21 02:44:18.000000 framelink-0.2.0/.gitignore
+-rw-r--r--   0 runner    (1001) docker     (123)      577 2023-04-21 02:44:18.000000 framelink-0.2.0/.pre-commit-config.yaml
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-21 02:45:32.235062 framelink-0.2.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     4078 2023-04-21 02:44:18.000000 framelink-0.2.0/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/data/
+-rw-r--r--   0 runner    (1001) docker     (123)    19808 2023-04-21 02:44:18.000000 framelink-0.2.0/data/divy_trips_limited.csv
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/examples/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/examples/notebooks/
+-rw-r--r--   0 runner    (1001) docker     (123)    52351 2023-04-21 02:44:18.000000 framelink-0.2.0/examples/notebooks/basic_pandas.ipynb
+-rw-r--r--   0 runner    (1001) docker     (123)   336847 2023-04-21 02:44:18.000000 framelink-0.2.0/pdm.lock
+-rw-r--r--   0 runner    (1001) docker     (123)     1299 2023-04-21 02:44:18.000000 framelink-0.2.0/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 02:45:32.235062 framelink-0.2.0/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.227062 framelink-0.2.0/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.231062 framelink-0.2.0/src/framelink/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:44:18.000000 framelink-0.2.0/src/framelink/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      160 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink/__version__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      694 2023-04-21 02:44:18.000000 framelink-0.2.0/src/framelink/_util.py
+-rw-r--r--   0 runner    (1001) docker     (123)    12820 2023-04-21 02:44:18.000000 framelink-0.2.0/src/framelink/core.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.231062 framelink-0.2.0/src/framelink.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     4346 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      752 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      342 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       10 2023-04-21 02:45:32.000000 framelink-0.2.0/src/framelink.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.231062 framelink-0.2.0/tests/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1238 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/conftest.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 02:45:32.235062 framelink-0.2.0/tests/core/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)       92 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_cache.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2222 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_dag.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1738 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_logging.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5608 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_model.py
+-rw-r--r--   0 runner    (1001) docker     (123)      717 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_model_parsing.py
+-rw-r--r--   0 runner    (1001) docker     (123)      318 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_persistance.py
+-rw-r--r--   0 runner    (1001) docker     (123)     3845 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_pipeline_metas.py
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/core/test_run.py
+-rw-r--r--   0 runner    (1001) docker     (123)      272 2023-04-21 02:44:18.000000 framelink-0.2.0/tests/readme.md
```

### Comparing `framelink-0.1.0/.github/workflows/lint_test_build.yml` & `framelink-0.2.0/.github/workflows/lint_test_build.yml`

 * *Files 20% similar despite different names*

```diff
@@ -15,23 +15,24 @@
       - name: Checkout code
         uses: actions/checkout@v3
       - name: Setup python ${{ matrix.python_version }}
         uses: actions/setup-python@v4
         with:
           python-version: ${{ matrix.python_version }}
           cache: 'pip'
+          cache-dependency-path: 'pdm.lock'
       - name: Install dependencies
         run: pip install .[dev]
       - name: black
-        run: black . --check
+        run: black . --check -v
       - name: ruff
         run: ruff check .
-      - name: Run tests
-        run: pytest --cov src --cov-report xml --cov-report term
-      - name: Codecov
+      - name: pytest
+        run: pytest --cov=framelink --cov-report=xml --cov-report=term
+      - name: Upload coverage reports to Codecov
         uses: codecov/codecov-action@v3
         with:
           token: ${{ secrets.CODECOV_TOKEN }}
           files: coverage.xml
           verbose: true
       - name: Build application
         run: python -m build .
```

### Comparing `framelink-0.1.0/.pre-commit-config.yaml` & `framelink-0.2.0/.pre-commit-config.yaml`

 * *Files 18% similar despite different names*

```diff
@@ -13,13 +13,13 @@
       - id: ruff
         args: [ --fix, --exit-non-zero-on-fix ]
 
   - repo: https://github.com/psf/black
     rev: 22.12.0
     hooks:
       - id: black
-        types: [ "python" ]
 
   - repo: https://github.com/pre-commit/mirrors-mypy
     rev: 'v1.0.1'
     hooks:
       - id: mypy
+        exclude: tests
```

### Comparing `framelink-0.1.0/data/divy_trips_limited.csv` & `framelink-0.2.0/data/divy_trips_limited.csv`

 * *Files identical despite different names*

### Comparing `framelink-0.1.0/pyproject.toml` & `framelink-0.2.0/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,52 +1,72 @@
 [project]
 authors = [
     { name = "Toby Devlin", email = "toby@tobydevlin.com" },
 ]
-requires-python = ">=3.9,<4.0"
+requires-python = ">=3.8,<4.0"
 name = "framelink"
 description = ""
 readme = "README.md"
 dynamic = ["version"]
 
 dependencies = [
-    "pandas<2.0.0,>=1.5.3",
-    "polars<1.0.0,>=0.16.7",
-    "networkx<4.0,>=3.0",
-    "openlineage-python>=0.21.1",
-    "setuptools-scm>=7.1.0",
-    "pytest-cov>=4.0.0",
+    "networkx>=3.0"
 ]
+
 [project.optional-dependencies]
+viz = [
+    "matplotlib>=3.7.1",
+    "graphviz>=0.20.1",
+    "pydot>=1.4.2"
+]
+
 dev = [
-    "mypy>=1.1.1",
+    "framelink",
+    "framelink[viz]",
+    "openlineage-python>=0.21.1",
+    "setuptools-scm>=7.1.0",
     "pytest>=7.2.2",
-    "pre-commit>=3.2.0",
+    "pytest-cov>=4.0.0",
+    "mypy>=1.1.1",
     "ruff>=0.0.258",
-    "build>=0.10.0",
     "black>=23.1.0",
+    "build>=0.10.0",
+    # more for testing and the like
+    "pandas<2.0.0,>=1.5.3",
+    "polars<1.0.0,>=0.16.7",
+    "pre-commit>=3.2.0",
+    "pyment>=0.3.3",
+    "pyarrow>=11.0.0",
+    "jupyter>=1.0.0",
 ]
 
 [project.urls]
 github = "https://github.com/GitToby/framelink"
 
 [build-system]
 requires = ["setuptools>=45", "setuptools_scm[toml]>=6.2"]
 
 [tool.setuptools_scm]
 write_to = "src/framelink/__version__.py"
 
 [tool.ruff]
-# Enable Pyflakes `E` and `F` codes by default.
 select = ["E", "F"]
-# Allow autofix for all enabled rules (when `--fix`) is provided.
 fixable = ["E", "F"]
 line-length = 120
 
 [tool.ruff.mccabe]
-# Unlike Flake8, default to a complexity level of 10.
 max-complexity = 10
 
+[tool.black]
+line-length = 120
+target_versions = ['py38', 'py39', 'py310', 'py311']
+
 [tool.mypy]
 ignore_missing_imports = true
 
+[tool.pytest.ini_options]
+addopts = "-ra"
+testpaths = [
+    "tests",
+]
+
 [tool.pdm]
```

