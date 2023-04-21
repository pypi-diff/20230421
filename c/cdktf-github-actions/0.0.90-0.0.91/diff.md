# Comparing `tmp/cdktf-github-actions-0.0.90.tar.gz` & `tmp/cdktf-github-actions-0.0.91.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cdktf-github-actions-0.0.90.tar", last modified: Wed Apr 19 00:29:29 2023, max compression
+gzip compressed data, was "cdktf-github-actions-0.0.91.tar", last modified: Thu Apr 20 00:27:51 2023, max compression
```

## Comparing `cdktf-github-actions-0.0.90.tar` & `cdktf-github-actions-0.0.91.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:29:29.718844 cdktf-github-actions-0.0.90/
--rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-19 00:29:17.000000 cdktf-github-actions-0.0.90/LICENSE
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-19 00:29:17.000000 cdktf-github-actions-0.0.90/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-19 00:29:29.714844 cdktf-github-actions-0.0.90/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-19 00:29:17.000000 cdktf-github-actions-0.0.90/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-19 00:29:17.000000 cdktf-github-actions-0.0.90/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-19 00:29:29.718844 cdktf-github-actions-0.0.90/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-19 00:29:17.000000 cdktf-github-actions-0.0.90/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:29:29.714844 cdktf-github-actions-0.0.90/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:29:29.714844 cdktf-github-actions-0.0.90/src/cdktf_github-actions/
--rw-r--r--   0 runner    (1001) docker     (123)   190483 2023-04-19 00:29:17.000000 cdktf-github-actions-0.0.90/src/cdktf_github-actions/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:29:29.714844 cdktf-github-actions-0.0.90/src/cdktf_github-actions/_jsii/
--rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-19 00:29:17.000000 cdktf-github-actions-0.0.90/src/cdktf_github-actions/_jsii/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)   189726 2023-04-19 00:29:17.000000 cdktf-github-actions-0.0.90/src/cdktf_github-actions/_jsii/cdktf-github-actions@0.0.90.jsii.tgz
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:29:17.000000 cdktf-github-actions-0.0.90/src/cdktf_github-actions/py.typed
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 00:29:29.714844 cdktf-github-actions-0.0.90/src/cdktf_github_actions.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-19 00:29:29.000000 cdktf-github-actions-0.0.90/src/cdktf_github_actions.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-19 00:29:29.000000 cdktf-github-actions-0.0.90/src/cdktf_github_actions.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 00:29:29.000000 cdktf-github-actions-0.0.90/src/cdktf_github_actions.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-19 00:29:29.000000 cdktf-github-actions-0.0.90/src/cdktf_github_actions.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-19 00:29:29.000000 cdktf-github-actions-0.0.90/src/cdktf_github_actions.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:27:51.376981 cdktf-github-actions-0.0.91/
+-rw-r--r--   0 runner    (1001) docker     (123)    11358 2023-04-20 00:27:39.000000 cdktf-github-actions-0.0.91/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-20 00:27:39.000000 cdktf-github-actions-0.0.91/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-20 00:27:51.376981 cdktf-github-actions-0.0.91/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2391 2023-04-20 00:27:39.000000 cdktf-github-actions-0.0.91/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      234 2023-04-20 00:27:39.000000 cdktf-github-actions-0.0.91/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-20 00:27:51.376981 cdktf-github-actions-0.0.91/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1880 2023-04-20 00:27:39.000000 cdktf-github-actions-0.0.91/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:27:51.372981 cdktf-github-actions-0.0.91/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:27:51.376981 cdktf-github-actions-0.0.91/src/cdktf_github-actions/
+-rw-r--r--   0 runner    (1001) docker     (123)   190483 2023-04-20 00:27:39.000000 cdktf-github-actions-0.0.91/src/cdktf_github-actions/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:27:51.376981 cdktf-github-actions-0.0.91/src/cdktf_github-actions/_jsii/
+-rw-r--r--   0 runner    (1001) docker     (123)      471 2023-04-20 00:27:39.000000 cdktf-github-actions-0.0.91/src/cdktf_github-actions/_jsii/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)   189725 2023-04-20 00:27:39.000000 cdktf-github-actions-0.0.91/src/cdktf_github-actions/_jsii/cdktf-github-actions@0.0.91.jsii.tgz
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:27:39.000000 cdktf-github-actions-0.0.91/src/cdktf_github-actions/py.typed
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-20 00:27:51.376981 cdktf-github-actions-0.0.91/src/cdktf_github_actions.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3347 2023-04-20 00:27:51.000000 cdktf-github-actions-0.0.91/src/cdktf_github_actions.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      474 2023-04-20 00:27:51.000000 cdktf-github-actions-0.0.91/src/cdktf_github_actions.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-20 00:27:51.000000 cdktf-github-actions-0.0.91/src/cdktf_github_actions.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      149 2023-04-20 00:27:51.000000 cdktf-github-actions-0.0.91/src/cdktf_github_actions.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       21 2023-04-20 00:27:51.000000 cdktf-github-actions-0.0.91/src/cdktf_github_actions.egg-info/top_level.txt
```

### Comparing `cdktf-github-actions-0.0.90/LICENSE` & `cdktf-github-actions-0.0.91/LICENSE`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.90/PKG-INFO` & `cdktf-github-actions-0.0.91/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-github-actions
-Version: 0.0.90
+Version: 0.0.91
 Summary: @awlsring/cdktf-github-actions
 Home-page: https://github.com/awlsring/cdktf-github-actions.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-github-actions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

### Comparing `cdktf-github-actions-0.0.90/README.md` & `cdktf-github-actions-0.0.91/README.md`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.90/setup.py` & `cdktf-github-actions-0.0.91/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import json
 import setuptools
 
 kwargs = json.loads(
     """
 {
     "name": "cdktf-github-actions",
-    "version": "0.0.90",
+    "version": "0.0.91",
     "description": "@awlsring/cdktf-github-actions",
     "license": "Apache-2.0",
     "url": "https://github.com/awlsring/cdktf-github-actions.git",
     "long_description_content_type": "text/markdown",
     "author": "awlsring<mattcanemail@gmail.com>",
     "bdist_wheel": {
         "universal": true
@@ -22,15 +22,15 @@
     },
     "packages": [
         "cdktf_github-actions",
         "cdktf_github-actions._jsii"
     ],
     "package_data": {
         "cdktf_github-actions._jsii": [
-            "cdktf-github-actions@0.0.90.jsii.tgz"
+            "cdktf-github-actions@0.0.91.jsii.tgz"
         ],
         "cdktf_github-actions": [
             "py.typed"
         ]
     },
     "python_requires": "~=3.7",
     "install_requires": [
```

### Comparing `cdktf-github-actions-0.0.90/src/cdktf_github-actions/__init__.py` & `cdktf-github-actions-0.0.91/src/cdktf_github-actions/__init__.py`

 * *Files identical despite different names*

### Comparing `cdktf-github-actions-0.0.90/src/cdktf_github_actions.egg-info/PKG-INFO` & `cdktf-github-actions-0.0.91/src/cdktf_github_actions.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cdktf-github-actions
-Version: 0.0.90
+Version: 0.0.91
 Summary: @awlsring/cdktf-github-actions
 Home-page: https://github.com/awlsring/cdktf-github-actions.git
 Author: awlsring<mattcanemail@gmail.com>
 License: Apache-2.0
 Project-URL: Source, https://github.com/awlsring/cdktf-github-actions.git
 Classifier: Intended Audience :: Developers
 Classifier: Operating System :: OS Independent
```

