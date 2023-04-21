# Comparing `tmp/skyagi-0.0.6.tar.gz` & `tmp/skyagi-0.0.8.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "skyagi-0.0.6.tar", last modified: Tue Apr 18 06:27:03 2023, max compression
+gzip compressed data, was "skyagi-0.0.8.tar", last modified: Fri Apr 21 10:47:59 2023, max compression
```

## Comparing `skyagi-0.0.6.tar` & `skyagi-0.0.8.tar`

### file list

```diff
@@ -1,33 +1,47 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:27:03.554813 skyagi-0.0.6/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:27:03.550813 skyagi-0.0.6/.github/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:27:03.550813 skyagi-0.0.6/.github/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-18 06:26:54.000000 skyagi-0.0.6/.github/scripts/release.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:27:03.550813 skyagi-0.0.6/.github/workflows/
--rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-18 06:26:54.000000 skyagi-0.0.6/.github/workflows/publish.yml
--rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-18 06:26:54.000000 skyagi-0.0.6/.github/workflows/release.yml
--rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-18 06:26:54.000000 skyagi-0.0.6/.gitignore
--rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-18 06:26:54.000000 skyagi-0.0.6/CODEOWNERS
--rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-18 06:26:54.000000 skyagi-0.0.6/Makefile
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 06:27:03.554813 skyagi-0.0.6/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       27 2023-04-18 06:26:54.000000 skyagi-0.0.6/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-18 06:26:54.000000 skyagi-0.0.6/pyproject.toml
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:27:03.550813 skyagi-0.0.6/scripts/
--rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-18 06:26:54.000000 skyagi-0.0.6/scripts/format-staged-files.sh
--rwxr-xr-x   0 runner    (1001) docker     (123)      703 2023-04-18 06:26:54.000000 skyagi-0.0.6/scripts/pre-commit
--rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-04-18 06:26:54.000000 skyagi-0.0.6/scripts/pre-push
--rw-r--r--   0 runner    (1001) docker     (123)     1033 2023-04-18 06:27:03.554813 skyagi-0.0.6/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:27:03.550813 skyagi-0.0.6/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:27:03.550813 skyagi-0.0.6/src/skyagi/
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:26:54.000000 skyagi-0.0.6/src/skyagi/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)     3984 2023-04-18 06:26:54.000000 skyagi-0.0.6/src/skyagi/cli.py
--rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-18 06:26:54.000000 skyagi-0.0.6/src/skyagi/config.py
--rw-r--r--   0 runner    (1001) docker     (123)     2041 2023-04-18 06:26:54.000000 skyagi-0.0.6/src/skyagi/skyagi.py
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-18 06:26:54.000000 skyagi-0.0.6/src/skyagi/tui.py
--rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-18 06:26:54.000000 skyagi-0.0.6/src/skyagi/util.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-18 06:27:03.554813 skyagi-0.0.6/src/skyagi.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      557 2023-04-18 06:27:03.000000 skyagi-0.0.6/src/skyagi.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      545 2023-04-18 06:27:03.000000 skyagi-0.0.6/src/skyagi.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-18 06:27:03.000000 skyagi-0.0.6/src/skyagi.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-18 06:27:03.000000 skyagi-0.0.6/src/skyagi.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (123)      251 2023-04-18 06:27:03.000000 skyagi-0.0.6/src/skyagi.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-18 06:27:03.000000 skyagi-0.0.6/src/skyagi.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.266903 skyagi-0.0.8/.github/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/.github/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     1398 2023-04-21 10:47:50.000000 skyagi-0.0.8/.github/scripts/release.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/.github/workflows/
+-rw-r--r--   0 runner    (1001) docker     (123)      602 2023-04-21 10:47:50.000000 skyagi-0.0.8/.github/workflows/publish.yml
+-rw-r--r--   0 runner    (1001) docker     (123)      408 2023-04-21 10:47:50.000000 skyagi-0.0.8/.github/workflows/release.yml
+-rw-r--r--   0 runner    (1001) docker     (123)       54 2023-04-21 10:47:50.000000 skyagi-0.0.8/.gitignore
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/.vscode/
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-21 10:47:50.000000 skyagi-0.0.8/.vscode/settings.json
+-rw-r--r--   0 runner    (1001) docker     (123)       16 2023-04-21 10:47:50.000000 skyagi-0.0.8/CODEOWNERS
+-rw-r--r--   0 runner    (1001) docker     (123)      323 2023-04-21 10:47:50.000000 skyagi-0.0.8/Makefile
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 10:47:59.274903 skyagi-0.0.8/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)       28 2023-04-21 10:47:50.000000 skyagi-0.0.8/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/examples/
+-rw-r--r--   0 runner    (1001) docker     (123)      296 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/agent.json
+-rw-r--r--   0 runner    (1001) docker     (123)     2909 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/hailey.json
+-rw-r--r--   0 runner    (1001) docker     (123)     3397 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/justin.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1569 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/selena.json
+-rw-r--r--   0 runner    (1001) docker     (123)     1064 2023-04-21 10:47:50.000000 skyagi-0.0.8/examples/zayn.json
+-rw-r--r--   0 runner    (1001) docker     (123)      171 2023-04-21 10:47:50.000000 skyagi-0.0.8/pyproject.toml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/scripts/
+-rw-r--r--   0 runner    (1001) docker     (123)     2239 2023-04-21 10:47:50.000000 skyagi-0.0.8/scripts/format-staged-files.sh
+-rwxr-xr-x   0 runner    (1001) docker     (123)      703 2023-04-21 10:47:50.000000 skyagi-0.0.8/scripts/pre-commit
+-rwxr-xr-x   0 runner    (1001) docker     (123)      378 2023-04-21 10:47:50.000000 skyagi-0.0.8/scripts/pre-push
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 10:47:50.000000 skyagi-0.0.8/scripts/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1065 2023-04-21 10:47:59.274903 skyagi-0.0.8/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.270903 skyagi-0.0.8/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/src/skyagi/
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5356 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/cli.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1094 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/config.py
+-rw-r--r--   0 runner    (1001) docker     (123)      615 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/context.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/src/skyagi/simulation/
+-rw-r--r--   0 runner    (1001) docker     (123)    14685 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/simulation/agent.py
+-rw-r--r--   0 runner    (1001) docker     (123)     5413 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/simulation/run.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2766 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/simulation/simulation.py
+-rw-r--r--   0 runner    (1001) docker     (123)     6393 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/skyagi.py
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/tui.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1535 2023-04-21 10:47:50.000000 skyagi-0.0.8/src/skyagi/util.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 10:47:59.274903 skyagi-0.0.8/src/skyagi.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      558 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      802 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      280 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        7 2023-04-21 10:47:59.000000 skyagi-0.0.8/src/skyagi.egg-info/top_level.txt
```

### Comparing `skyagi-0.0.6/.github/scripts/release.py` & `skyagi-0.0.8/.github/scripts/release.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.6/.github/workflows/publish.yml` & `skyagi-0.0.8/.github/workflows/publish.yml`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.6/PKG-INFO` & `skyagi-0.0.8/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: skyagi
-Version: 0.0.6
+Version: 0.0.8
 Summary: AGI
 Home-page: https://github.com/litanlitudan/skyagi
 Author: Tan Li
 Author-email: tan@tanli.dev
 Project-URL: Bug Tracker, https://github.com/litanlitudan/skyagi/issues
 Project-URL: Changelog, https://github.com/litanlitudan/skyagi/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # SkyAGI: Sky is the Limit
+
```

### Comparing `skyagi-0.0.6/scripts/format-staged-files.sh` & `skyagi-0.0.8/scripts/format-staged-files.sh`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.6/scripts/pre-commit` & `skyagi-0.0.8/scripts/pre-commit`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.6/setup.cfg` & `skyagi-0.0.8/setup.cfg`

 * *Files 10% similar despite different names*

```diff
@@ -27,22 +27,25 @@
 	markdown
 	networkx
 	psutil
 	rich
 	textual
 	typer
 	uvicorn[standard]
+	termcolor
+	tiktoken
 	datasets
 	faiss-cpu
 	openai
 	pinecone-client
 	sacremoses
 	sentence-transformers
 	transformers
 	txtai
+	langchain
 
 [options.extras_require]
 dev = 
 	black
 	Faker
 	flake8
 	isort
```

### Comparing `skyagi-0.0.6/src/skyagi/config.py` & `skyagi-0.0.8/src/skyagi/config.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.6/src/skyagi/util.py` & `skyagi-0.0.8/src/skyagi/util.py`

 * *Files identical despite different names*

### Comparing `skyagi-0.0.6/src/skyagi.egg-info/PKG-INFO` & `skyagi-0.0.8/src/skyagi.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,17 +1,18 @@
 Metadata-Version: 2.1
 Name: skyagi
-Version: 0.0.6
+Version: 0.0.8
 Summary: AGI
 Home-page: https://github.com/litanlitudan/skyagi
 Author: Tan Li
 Author-email: tan@tanli.dev
 Project-URL: Bug Tracker, https://github.com/litanlitudan/skyagi/issues
 Project-URL: Changelog, https://github.com/litanlitudan/skyagi/releases
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Requires-Python: >=3.8
 Description-Content-Type: text/markdown
 Provides-Extra: dev
 
 # SkyAGI: Sky is the Limit
+
```

### Comparing `skyagi-0.0.6/src/skyagi.egg-info/SOURCES.txt` & `skyagi-0.0.8/src/skyagi.egg-info/SOURCES.txt`

 * *Files 15% similar despite different names*

```diff
@@ -3,22 +3,33 @@
 Makefile
 README.md
 pyproject.toml
 setup.cfg
 .github/scripts/release.py
 .github/workflows/publish.yml
 .github/workflows/release.yml
+.vscode/settings.json
+examples/agent.json
+examples/hailey.json
+examples/justin.json
+examples/selena.json
+examples/zayn.json
 scripts/format-staged-files.sh
 scripts/pre-commit
 scripts/pre-push
+scripts/run.py
 src/skyagi/__init__.py
 src/skyagi/cli.py
 src/skyagi/config.py
+src/skyagi/context.py
 src/skyagi/skyagi.py
 src/skyagi/tui.py
 src/skyagi/util.py
 src/skyagi.egg-info/PKG-INFO
 src/skyagi.egg-info/SOURCES.txt
 src/skyagi.egg-info/dependency_links.txt
 src/skyagi.egg-info/entry_points.txt
 src/skyagi.egg-info/requires.txt
-src/skyagi.egg-info/top_level.txt
+src/skyagi.egg-info/top_level.txt
+src/skyagi/simulation/agent.py
+src/skyagi/simulation/run.py
+src/skyagi/simulation/simulation.py
```

