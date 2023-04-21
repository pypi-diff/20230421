# Comparing `tmp/module_qc_database_tools-0.0.1.tar.gz` & `tmp/module_qc_database_tools-0.1.0.tar.gz`

## Comparing `module_qc_database_tools-0.0.1.tar` & `module_qc_database_tools-0.1.0.tar`

### file list

```diff
@@ -1,19 +1,24 @@
--rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/.env.template
--rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/.gitlab-ci.yml
--rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/tbump.toml
--rw-r--r--   0        0        0      319 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/src/module_qc_database_tools/__init__.py
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/src/module_qc_database_tools/_version.py
--rw-r--r--   0        0        0      144 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/src/module_qc_database_tools/cli/__init__.py
--rw-r--r--   0        0        0       93 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/src/module_qc_database_tools/cli/__main__.py
--rw-r--r--   0        0        0    15476 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/src/module_qc_database_tools/cli/generate_yarr_config.py
--rw-r--r--   0        0        0     1180 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/src/module_qc_database_tools/cli/main.py
--rw-r--r--   0        0        0     1694 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/src/module_qc_database_tools/cli/register_component.py
--rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/src/module_qc_database_tools/data/componentConfigs.json
--rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/src/module_qc_database_tools/data/YARR/chip_template.json
--rw-r--r--   0        0        0      707 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/tests/test_cli.py
--rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/tests/test_package.py
--rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/.gitignore
--rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/README.md
--rw-r--r--   0        0        0     4585 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/pyproject.toml
--rw-r--r--   0        0        0     4032 2020-02-02 00:00:00.000000 module_qc_database_tools-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0       99 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/.env.template
+-rw-r--r--   0        0        0     3119 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/.gitlab-ci.yml
+-rw-r--r--   0        0        0     2252 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      893 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tbump.toml
+-rw-r--r--   0        0        0      283 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/__init__.py
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/_version.py
+-rw-r--r--   0        0        0     9998 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/chip_config_api.py
+-rw-r--r--   0        0        0    12566 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/core.py
+-rw-r--r--   0        0        0     1168 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/utils.py
+-rw-r--r--   0        0        0      108 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/__init__.py
+-rw-r--r--   0        0        0       57 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/__main__.py
+-rw-r--r--   0        0        0     4394 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/generate_yarr_config.py
+-rw-r--r--   0        0        0     1146 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/main.py
+-rw-r--r--   0        0        0     1629 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/register_component.py
+-rw-r--r--   0        0        0      713 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/data/componentConfigs.json
+-rw-r--r--   0        0        0      378 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/src/module_qc_database_tools/data/YARR/chip_template.json
+-rw-r--r--   0        0        0     2203 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tests/test_cli.py
+-rw-r--r--   0        0        0     1249 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tests/test_config_api.py
+-rw-r--r--   0        0        0      120 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tests/test_package.py
+-rw-r--r--   0        0        0      348 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/tests/test_utils.py
+-rw-r--r--   0        0        0     2156 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/.gitignore
+-rw-r--r--   0        0        0     2431 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/README.md
+-rw-r--r--   0        0        0     4594 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/pyproject.toml
+-rw-r--r--   0        0        0     4079 2020-02-02 00:00:00.000000 module_qc_database_tools-0.1.0/PKG-INFO
```

### Comparing `module_qc_database_tools-0.0.1/.gitlab-ci.yml` & `module_qc_database_tools-0.1.0/.gitlab-ci.yml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.0.1/.pre-commit-config.yaml` & `module_qc_database_tools-0.1.0/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.0.1/tbump.toml` & `module_qc_database_tools-0.1.0/tbump.toml`

 * *Files 17% similar despite different names*

```diff
@@ -1,9 +1,9 @@
 00000000: 5b76 6572 7369 6f6e 5d0a 6375 7272 656e  [version].curren
-00000010: 7420 3d20 2230 2e30 2e31 220a 0a23 2045  t = "0.0.1"..# E
+00000010: 7420 3d20 2230 2e31 2e30 220a 0a23 2045  t = "0.1.0"..# E
 00000020: 7861 6d70 6c65 206f 6620 6120 7365 6d76  xample of a semv
 00000030: 6572 2072 6567 6578 702e 0a23 204d 616b  er regexp..# Mak
 00000040: 6520 7375 7265 2074 6869 7320 6d61 7463  e sure this matc
 00000050: 6865 7320 6375 7272 656e 745f 7665 7273  hes current_vers
 00000060: 696f 6e20 6265 666f 7265 0a23 2075 7369  ion before.# usi
 00000070: 6e67 2074 6275 6d70 0a72 6567 6578 203d  ng tbump.regex =
 00000080: 2027 2727 0a20 2028 3f50 3c6d 616a 6f72   '''.  (?P<major
@@ -14,16 +14,16 @@
 000000d0: 6361 6e64 6964 6174 653e 5c64 2b29 0a20  candidate>\d+). 
 000000e0: 2029 3f0a 2020 2727 270a 0a5b 6769 745d   )?.  '''..[git]
 000000f0: 0a23 2054 6865 2063 7572 7265 6e74 2076  .# The current v
 00000100: 6572 7369 6f6e 2077 696c 6c20 6765 7420  ersion will get 
 00000110: 7570 6461 7465 6420 7768 656e 2074 6275  updated when tbu
 00000120: 6d70 2069 7320 7275 6e0a 6d65 7373 6167  mp is run.messag
 00000130: 655f 7465 6d70 6c61 7465 203d 2022 4275  e_template = "Bu
-00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 302e  mp version: 0.0.
-00000150: 3120 e286 9220 7b6e 6577 5f76 6572 7369  1 ... {new_versi
+00000140: 6d70 2076 6572 7369 6f6e 3a20 302e 312e  mp version: 0.1.
+00000150: 3020 e286 9220 7b6e 6577 5f76 6572 7369  0 ... {new_versi
 00000160: 6f6e 7d22 0a74 6167 5f74 656d 706c 6174  on}".tag_templat
 00000170: 6520 3d20 2276 7b6e 6577 5f76 6572 7369  e = "v{new_versi
 00000180: 6f6e 7d22 0a0a 2320 466f 7220 6561 6368  on}"..# For each
 00000190: 2066 696c 6520 746f 2070 6174 6368 2c20   file to patch, 
 000001a0: 6164 6420 6120 5b5b 6669 6c65 5d5d 2063  add a [[file]] c
 000001b0: 6f6e 6669 670a 2320 7365 6374 696f 6e20  onfig.# section 
 000001c0: 636f 6e74 6169 6e69 6e67 2074 6865 2070  containing the p
```

### Comparing `module_qc_database_tools-0.0.1/src/module_qc_database_tools/cli/main.py` & `module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/main.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 """
 Top-level entrypoint for the command line interface.
 """
-from __future__ import annotations
+
 
 import typer
 
 import module_qc_database_tools
 from module_qc_database_tools.cli.generate_yarr_config import (
     main as generate_yarr_config,
 )
```

### Comparing `module_qc_database_tools-0.0.1/src/module_qc_database_tools/cli/register_component.py` & `module_qc_database_tools-0.1.0/src/module_qc_database_tools/cli/register_component.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,9 +1,7 @@
-from __future__ import annotations
-
 import json
 import os
 from pathlib import Path
 
 import itkdb
 import typer
 
@@ -32,16 +30,15 @@
         help="Component to register",
     ),
     institution: str = typer.Option("", "-i", "--institution", help="Institution"),
 ):
     """
     Main executable for registering components.
     """
-    with config_path.open() as fpointer:
-        config = json.load(fpointer)[component]
+    config = json.loads(config_path.read_text())[component]
 
     institution = institution or os.environ.get("INSTITUTION")
     if not institution:
         msg = "Must specify institution from commandline or set the appropriate environment variable."
         raise ValueError(msg)
 
     client = itkdb.Client()
```

### Comparing `module_qc_database_tools-0.0.1/src/module_qc_database_tools/data/componentConfigs.json` & `module_qc_database_tools-0.1.0/src/module_qc_database_tools/data/componentConfigs.json`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.0.1/.gitignore` & `module_qc_database_tools-0.1.0/.gitignore`

 * *Files identical despite different names*

### Comparing `module_qc_database_tools-0.0.1/README.md` & `module_qc_database_tools-0.1.0/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# Module QC Database Tools v0.0.1
+# Module QC Database Tools v0.1.0
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

### Comparing `module_qc_database_tools-0.0.1/pyproject.toml` & `module_qc_database_tools-0.1.0/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -40,14 +40,16 @@
     "Development Status :: 1 - Planning",
 ]
 
 dependencies = [
     "itkdb>=0.4.0",  # for interface with production database
     "pandas",
     "typer",
+    "pymongo",
+    "jsondiff",
     "importlib_resources>=1.4.0; python_version < '3.9'",  # for resources
 ]
 
 [project.urls]
 Homepage = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools"
 "Bug Tracker" = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues"
 Source = "https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools"
@@ -92,15 +94,15 @@
 # pylint and pytest needs to be installed into package environment
 detached = false
 dependencies = [
     "pytest >=6",
 ]
 
 [tool.hatch.envs.dev.scripts]
-test = "pytest -ra"
+test = "pytest -ra {args}"
 
 [[tool.hatch.envs.dev.matrix]]
 python = ["3.7", "3.8", "3.9", "3.10", "3.11", "pypy3.8"]
 
 [tool.ruff]
 select = [
   "E", "F", "W", # flake8
@@ -124,15 +126,15 @@
   "YTT",         # flake8-2020
 ]
 extend-ignore = ["PLR", "E501"]
 target-version = "py37"
 src = ["src"]
 unfixable = ["T20", "F841"]
 exclude = []
-isort.required-imports = ["from __future__ import annotations"]
+# isort.required-imports = [""]
 
 [tool.ruff.per-file-ignores]
 "src/module_qc_database_tools/cli/generate_yarr_config.py" = ["B008"]
 "src/module_qc_database_tools/cli/main.py" = ["B008"]
 "src/module_qc_database_tools/cli/register_component.py" = ["B008"]
 
 [tool.pylint]
@@ -143,15 +145,15 @@
 messages_control.disable = [
   "design",
   "fixme",
   "line-too-long",
   "missing-module-docstring",
   "wrong-import-position",
 ]
-good-names="kB,PC_NTC,DeltaT"
+good-names="kB,PC_NTC,DeltaT,rx"
 
 [tool.pytest.ini_options]
 minversion = "6.0"
 addopts = ["-ra", "--showlocals", "--strict-markers", "--strict-config"]
 xfail_strict = true
 filterwarnings = ["error"]
 testpaths = [
```

### Comparing `module_qc_database_tools-0.0.1/PKG-INFO` & `module_qc_database_tools-0.1.0/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: module-qc-database-tools
-Version: 0.0.1
+Version: 0.1.0
 Summary: Python wrapper to interface with LocalDB and Production DB for common tasks for pixel modules.
 Project-URL: Homepage, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Project-URL: Bug Tracker, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools/issues
 Project-URL: Source, https://gitlab.cern.ch/atlas-itk/pixel/module/module-qc-database-tools
 Author-email: Jay Chan <jay.chan@cern.ch>
 Maintainer-email: Giordon Stark <kratsg@gmail.com>, Elisabetta Pianori <elisabetta.pianori@cern.ch>, Lingxin Meng <lingxin.meng@cern.ch>
 Classifier: Development Status :: 1 - Planning
@@ -21,19 +21,21 @@
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Topic :: Scientific/Engineering
 Requires-Python: >=3.7
 Requires-Dist: importlib-resources>=1.4.0; python_version < '3.9'
 Requires-Dist: itkdb>=0.4.0
+Requires-Dist: jsondiff
 Requires-Dist: pandas
+Requires-Dist: pymongo
 Requires-Dist: typer
 Description-Content-Type: text/markdown
 
-# Module QC Database Tools v0.0.1
+# Module QC Database Tools v0.1.0
 
 The package to regisiter ITkPixV1.1 modules, and generate YARR configs from ITk
 production database using `itkdb` API.
 
 ## Set-Up and First-time Installation
 
 A minimum of python version 3.7+ is required.
```

