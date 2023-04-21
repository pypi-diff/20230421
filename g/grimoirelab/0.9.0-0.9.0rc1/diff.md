# Comparing `tmp/grimoirelab-0.9.0.tar.gz` & `tmp/grimoirelab-0.9.0rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoirelab-0.9.0.tar", max compression
+gzip compressed data, was "grimoirelab-0.9.0rc1.tar", max compression
```

## Comparing `grimoirelab-0.9.0.tar` & `grimoirelab-0.9.0rc1.tar`

### file list

```diff
@@ -1,7 +1,7 @@
--rw-r--r--   0        0        0    35141 2023-04-21 13:02:18.020269 grimoirelab-0.9.0/LICENSE
--rw-r--r--   0        0        0     8685 2023-04-21 13:02:18.020269 grimoirelab-0.9.0/README.md
--rw-r--r--   0        0        0       34 2023-04-21 13:02:18.104274 grimoirelab-0.9.0/grimoirelab/__init__.py
--rw-r--r--   0        0        0       86 2023-04-21 13:02:18.104274 grimoirelab-0.9.0/grimoirelab/_version.py
--rwxr-xr-x   0        0        0     1844 2023-04-21 13:02:18.104274 grimoirelab-0.9.0/grimoirelab/grimoirelab.py
--rw-r--r--   0        0        0     1841 2023-04-21 13:02:18.108274 grimoirelab-0.9.0/pyproject.toml
--rw-r--r--   0        0        0    10204 1970-01-01 00:00:00.000000 grimoirelab-0.9.0/PKG-INFO
+-rw-r--r--   0        0        0    35141 2023-04-21 11:08:17.133081 grimoirelab-0.9.0rc1/LICENSE
+-rw-r--r--   0        0        0     8685 2023-04-21 11:08:17.133081 grimoirelab-0.9.0rc1/README.md
+-rw-r--r--   0        0        0       34 2023-04-21 11:08:17.209082 grimoirelab-0.9.0rc1/grimoirelab/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-21 11:08:17.209082 grimoirelab-0.9.0rc1/grimoirelab/_version.py
+-rwxr-xr-x   0        0        0     1844 2023-04-21 11:08:17.209082 grimoirelab-0.9.0rc1/grimoirelab/grimoirelab.py
+-rw-r--r--   0        0        0     1906 2023-04-21 11:08:17.209082 grimoirelab-0.9.0rc1/pyproject.toml
+-rw-r--r--   0        0        0    10267 1970-01-01 00:00:00.000000 grimoirelab-0.9.0rc1/PKG-INFO
```

### Comparing `grimoirelab-0.9.0/LICENSE` & `grimoirelab-0.9.0rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoirelab-0.9.0/README.md` & `grimoirelab-0.9.0rc1/README.md`

 * *Files identical despite different names*

### Comparing `grimoirelab-0.9.0/grimoirelab/grimoirelab.py` & `grimoirelab-0.9.0rc1/grimoirelab/grimoirelab.py`

 * *Files identical despite different names*

### Comparing `grimoirelab-0.9.0/pyproject.toml` & `grimoirelab-0.9.0rc1/pyproject.toml`

 * *Files 13% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoirelab"
-version = "0.9.0"
+version = "0.9.0-rc.1"
 description = "Tool set for software development analytics"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
@@ -34,27 +34,27 @@
 
 [tool.poetry.scripts]
 'grimoirelab' = 'grimoirelab.grimoirelab:main'
 
 [tool.poetry.dependencies]
 python = "^3.7.1"
 
-grimoirelab-toolkit = {version = ">=0.3.4", allow-prereleases = true}
-perceval-mozilla = {version = ">=0.3.8", allow-prereleases = true}
-perceval-opnfv = {version = ">=0.2.8", allow-prereleases = true}
-perceval-puppet = {version = ">=0.2.8", allow-prereleases = true}
-perceval-weblate = {version = ">=0.2.8", allow-prereleases = true}
-sortinghat = {version = ">=0.9.0", allow-prereleases = true}
-kidash = {version = ">=0.5.4", allow-prereleases = true}
+grimoirelab-toolkit = {version = ">=0.3.4-rc.1", allow-prereleases = true}
+perceval-mozilla = {version = ">=0.3.8-rc.2", allow-prereleases = true}
+perceval-opnfv = {version = ">=0.2.8-rc.2", allow-prereleases = true}
+perceval-puppet = {version = ">=0.2.8-rc.2", allow-prereleases = true}
+perceval-weblate = {version = ">=0.2.8-rc.2", allow-prereleases = true}
+sortinghat = {version = ">=0.9.0-rc.2", allow-prereleases = true}
+kidash = {version = ">=0.5.4-rc.1", allow-prereleases = true}
 grimoirelab-panels = {version = ">=0.2.0", allow-prereleases = true}
-grimoire-elk = {version = ">=0.104.3", allow-prereleases = true}
-sirmordred = {version = ">=0.7.0", allow-prereleases = true}
-cereslib = {version = ">=0.4.0", allow-prereleases = true}
-graal = {version = ">=0.4.5", allow-prereleases = true}
+grimoire-elk = {version = ">=0.104.3-rc.2", allow-prereleases = true}
+sirmordred = {version = ">=0.7.0-rc.1", allow-prereleases = true}
+cereslib = {version = ">=0.4.0-rc.1", allow-prereleases = true}
+graal = {version = ">=0.4.5-rc.2", allow-prereleases = true}
 statsmodels = "^0.13.2"
-perceval = {version = ">=0.21.4", allow-prereleases = true}
+perceval = {version = ">=0.21.4-rc.2", allow-prereleases = true}
 
 [tool.poetry.dev-dependencies]
 
 [build-system]
 requires = ["poetry-core>=1.0.0"]
 build-backend = "poetry.core.masonry.api"
```

### Comparing `grimoirelab-0.9.0/PKG-INFO` & `grimoirelab-0.9.0rc1/PKG-INFO`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoirelab
-Version: 0.9.0
+Version: 0.9.0rc1
 Summary: Tool set for software development analytics
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7.1,<4.0.0
 Classifier: Development Status :: 5 - Production/Stable
@@ -13,27 +13,27 @@
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3
 Classifier: Topic :: Software Development
-Requires-Dist: cereslib (>=0.4.0)
-Requires-Dist: graal (>=0.4.5)
-Requires-Dist: grimoire-elk (>=0.104.3)
+Requires-Dist: cereslib (>=0.4.0-rc.1)
+Requires-Dist: graal (>=0.4.5-rc.2)
+Requires-Dist: grimoire-elk (>=0.104.3-rc.2)
 Requires-Dist: grimoirelab-panels (>=0.2.0)
-Requires-Dist: grimoirelab-toolkit (>=0.3.4)
-Requires-Dist: kidash (>=0.5.4)
-Requires-Dist: perceval (>=0.21.4)
-Requires-Dist: perceval-mozilla (>=0.3.8)
-Requires-Dist: perceval-opnfv (>=0.2.8)
-Requires-Dist: perceval-puppet (>=0.2.8)
-Requires-Dist: perceval-weblate (>=0.2.8)
-Requires-Dist: sirmordred (>=0.7.0)
-Requires-Dist: sortinghat (>=0.9.0)
+Requires-Dist: grimoirelab-toolkit (>=0.3.4-rc.1)
+Requires-Dist: kidash (>=0.5.4-rc.1)
+Requires-Dist: perceval (>=0.21.4-rc.2)
+Requires-Dist: perceval-mozilla (>=0.3.8-rc.2)
+Requires-Dist: perceval-opnfv (>=0.2.8-rc.2)
+Requires-Dist: perceval-puppet (>=0.2.8-rc.2)
+Requires-Dist: perceval-weblate (>=0.2.8-rc.2)
+Requires-Dist: sirmordred (>=0.7.0-rc.1)
+Requires-Dist: sortinghat (>=0.9.0-rc.2)
 Requires-Dist: statsmodels (>=0.13.2,<0.14.0)
 Project-URL: Bug Tracker, https://github.com/chaoss/grimoirelab/issues
 Project-URL: Repository, https://github.com/chaoss/grimoirelab
 Description-Content-Type: text/markdown
 
 # GrimoireLab
```

