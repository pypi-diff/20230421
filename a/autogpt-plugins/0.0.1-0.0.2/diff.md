# Comparing `tmp/autogpt_plugins-0.0.1.tar.gz` & `tmp/autogpt_plugins-0.0.2.tar.gz`

## Comparing `autogpt_plugins-0.0.1.tar` & `autogpt_plugins-0.0.2.tar`

### file list

```diff
@@ -1,17 +1,17 @@
--rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/.editorconfig
--rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/.flake8
--rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/.pre-commit-config.yaml
--rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/Makefile
--rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/helpers.sh
--rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/pylintrc
--rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/requirements.txt
--rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/run_pylint.py
--rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/sourcery.yaml
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/src/autogpt_plugins/__init__.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/src/autogpt_plugins/create_plugins_here
--rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/src/autogpt_plugins/twitter/__init__.py
--rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/.gitignore
--rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/LICENSE
--rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/README.md
--rw-r--r--   0        0        0      898 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/pyproject.toml
--rw-r--r--   0        0        0      936 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.1/PKG-INFO
+-rw-r--r--   0        0        0      556 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/.editorconfig
+-rw-r--r--   0        0        0      168 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/.flake8
+-rw-r--r--   0        0        0      923 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/.pre-commit-config.yaml
+-rw-r--r--   0        0        0      399 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/Makefile
+-rw-r--r--   0        0        0      913 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/helpers.sh
+-rw-r--r--   0        0        0    14455 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/pylintrc
+-rw-r--r--   0        0        0       81 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/requirements.txt
+-rw-r--r--   0        0        0      439 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/run_pylint.py
+-rw-r--r--   0        0        0     1779 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/sourcery.yaml
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/src/autogpt_plugins/__init__.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/src/autogpt_plugins/create_plugins_here
+-rw-r--r--   0        0        0     7594 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/src/autogpt_plugins/twitter/__init__.py
+-rw-r--r--   0        0        0     1928 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/.gitignore
+-rw-r--r--   0        0        0     1098 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/LICENSE
+-rw-r--r--   0        0        0      382 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/README.md
+-rw-r--r--   0        0        0      865 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/pyproject.toml
+-rw-r--r--   0        0        0      903 2020-02-02 00:00:00.000000 autogpt_plugins-0.0.2/PKG-INFO
```

### Comparing `autogpt_plugins-0.0.1/.editorconfig` & `autogpt_plugins-0.0.2/.editorconfig`

 * *Files identical despite different names*

### Comparing `autogpt_plugins-0.0.1/.pre-commit-config.yaml` & `autogpt_plugins-0.0.2/.pre-commit-config.yaml`

 * *Files identical despite different names*

### Comparing `autogpt_plugins-0.0.1/helpers.sh` & `autogpt_plugins-0.0.2/helpers.sh`

 * *Files identical despite different names*

### Comparing `autogpt_plugins-0.0.1/pylintrc` & `autogpt_plugins-0.0.2/pylintrc`

 * *Files identical despite different names*

### Comparing `autogpt_plugins-0.0.1/sourcery.yaml` & `autogpt_plugins-0.0.2/sourcery.yaml`

 * *Files identical despite different names*

### Comparing `autogpt_plugins-0.0.1/src/autogpt_plugins/twitter/__init__.py` & `autogpt_plugins-0.0.2/src/autogpt_plugins/twitter/__init__.py`

 * *Files identical despite different names*

### Comparing `autogpt_plugins-0.0.1/.gitignore` & `autogpt_plugins-0.0.2/.gitignore`

 * *Files identical despite different names*

### Comparing `autogpt_plugins-0.0.1/LICENSE` & `autogpt_plugins-0.0.2/LICENSE`

 * *Files identical despite different names*

### Comparing `autogpt_plugins-0.0.1/pyproject.toml` & `autogpt_plugins-0.0.2/pyproject.toml`

 * *Files 24% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 [build-system]
 requires = ["hatchling"]
 build-backend = "hatchling.build"
 
 [project]
 name = "autogpt_plugins"
-version = "0.0.1"
+version = "0.0.2"
 authors = [
-  { name="Torantulino", email="34168009+BillSchumacher@users.noreply.github.com" },
+  { name="Torantulino", email="support@agpt.co" },
 ]
 description = "The plugins for Auto-GPT."
 readme = "README.md"
 requires-python = ">=3.8"
 classifiers = [
     "Programming Language :: Python :: 3",
     "License :: OSI Approved :: MIT License",
```

### Comparing `autogpt_plugins-0.0.1/PKG-INFO` & `autogpt_plugins-0.0.2/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 Metadata-Version: 2.1
 Name: autogpt_plugins
-Version: 0.0.1
+Version: 0.0.2
 Summary: The plugins for Auto-GPT.
 Project-URL: Homepage, https://github.com/Torantulino/Auto-GPT
 Project-URL: Bug Tracker, https://github.com/Torantulino/Auto-GPT
-Author-email: Torantulino <34168009+BillSchumacher@users.noreply.github.com>
+Author-email: Torantulino <support@agpt.co>
 License-File: LICENSE
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
 Classifier: Programming Language :: Python :: 3
 Requires-Python: >=3.8
 Requires-Dist: abstract-singleton
 Description-Content-Type: text/markdown
```

