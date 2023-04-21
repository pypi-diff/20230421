# Comparing `tmp/isee-0.1.8.tar.gz` & `tmp/isee-0.1.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "isee-0.1.8.tar", last modified: Mon Feb  1 20:26:40 2021, max compression
+gzip compressed data, was "isee-0.1.9.tar", last modified: Mon May  3 22:24:55 2021, max compression
```

## Comparing `isee-0.1.8.tar` & `isee-0.1.9.tar`

### file list

```diff
@@ -1,20 +1,20 @@
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-01 20:26:40.534510 isee-0.1.8/
--rw-r--r--   0 runner    (1001) docker     (117)     6092 2021-02-01 20:26:40.534510 isee-0.1.8/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)     5109 2021-02-01 20:26:16.000000 isee-0.1.8/README.md
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-01 20:26:40.530511 isee-0.1.8/isee/
--rw-r--r--   0 runner    (1001) docker     (117)      815 2021-02-01 20:26:16.000000 isee-0.1.8/isee/__init__.py
--rw-r--r--   0 runner    (1001) docker     (117)      707 2021-02-01 20:26:16.000000 isee-0.1.8/isee/common.py
--rw-r--r--   0 runner    (1001) docker     (117)     1788 2021-02-01 20:26:16.000000 isee-0.1.8/isee/file_modification_utils.py
--rw-r--r--   0 runner    (1001) docker     (117)     1506 2021-02-01 20:26:16.000000 isee-0.1.8/isee/generation_utils.py
--rw-r--r--   0 runner    (1001) docker     (117)     1038 2021-02-01 20:26:16.000000 isee-0.1.8/isee/git_utils.py
--rw-r--r--   0 runner    (1001) docker     (117)      429 2021-02-01 20:26:16.000000 isee-0.1.8/isee/pip_utils.py
-drwxr-xr-x   0 runner    (1001) docker     (117)        0 2021-02-01 20:26:40.534510 isee-0.1.8/isee.egg-info/
--rw-r--r--   0 runner    (1001) docker     (117)     6092 2021-02-01 20:26:40.000000 isee-0.1.8/isee.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (117)      350 2021-02-01 20:26:40.000000 isee-0.1.8/isee.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-01 20:26:40.000000 isee-0.1.8/isee.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (117)       36 2021-02-01 20:26:40.000000 isee-0.1.8/isee.egg-info/entry_points.txt
--rw-r--r--   0 runner    (1001) docker     (117)        1 2021-02-01 20:26:17.000000 isee-0.1.8/isee.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (117)       23 2021-02-01 20:26:40.000000 isee-0.1.8/isee.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (117)        5 2021-02-01 20:26:40.000000 isee-0.1.8/isee.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (117)      585 2021-02-01 20:26:40.534510 isee-0.1.8/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (117)       91 2021-02-01 20:26:16.000000 isee-0.1.8/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 22:24:55.732744 isee-0.1.9/
+-rw-r--r--   0 runner    (1001) docker     (121)     6092 2021-05-03 22:24:55.732744 isee-0.1.9/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)     5109 2021-05-03 22:24:30.000000 isee-0.1.9/README.md
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 22:24:55.732744 isee-0.1.9/isee/
+-rw-r--r--   0 runner    (1001) docker     (121)      815 2021-05-03 22:24:30.000000 isee-0.1.9/isee/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (121)      707 2021-05-03 22:24:30.000000 isee-0.1.9/isee/common.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1802 2021-05-03 22:24:30.000000 isee-0.1.9/isee/file_modification_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1506 2021-05-03 22:24:30.000000 isee-0.1.9/isee/generation_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)     1038 2021-05-03 22:24:30.000000 isee-0.1.9/isee/git_utils.py
+-rw-r--r--   0 runner    (1001) docker     (121)      429 2021-05-03 22:24:30.000000 isee-0.1.9/isee/pip_utils.py
+drwxr-xr-x   0 runner    (1001) docker     (121)        0 2021-05-03 22:24:55.732744 isee-0.1.9/isee.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (121)     6092 2021-05-03 22:24:55.000000 isee-0.1.9/isee.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (121)      350 2021-05-03 22:24:55.000000 isee-0.1.9/isee.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-03 22:24:55.000000 isee-0.1.9/isee.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (121)       36 2021-05-03 22:24:55.000000 isee-0.1.9/isee.egg-info/entry_points.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        1 2021-05-03 22:24:30.000000 isee-0.1.9/isee.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (121)       23 2021-05-03 22:24:55.000000 isee-0.1.9/isee.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (121)        5 2021-05-03 22:24:55.000000 isee-0.1.9/isee.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (121)      585 2021-05-03 22:24:55.732744 isee-0.1.9/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (121)       91 2021-05-03 22:24:30.000000 isee-0.1.9/setup.py
```

### Comparing `isee-0.1.8/PKG-INFO` & `isee-0.1.9/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isee
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python continuous integration (CI) support tools.
 Home-page: https://github.com/i2mint/isee
 Author: OtoSense
 License: mit
 Description: # Introduction
         Python continuous integration (CI) support tools.
```

### Comparing `isee-0.1.8/README.md` & `isee-0.1.9/README.md`

 * *Files identical despite different names*

### Comparing `isee-0.1.8/isee/__init__.py` & `isee-0.1.9/isee/__init__.py`

 * *Files identical despite different names*

### Comparing `isee-0.1.8/isee/common.py` & `isee-0.1.9/isee/common.py`

 * *Files identical despite different names*

### Comparing `isee-0.1.8/isee/file_modification_utils.py` & `isee-0.1.9/isee/file_modification_utils.py`

 * *Files 11% similar despite different names*

```diff
@@ -1,36 +1,36 @@
 import re
 
 from isee.common import get_env_var, get_file_path
 
 
 def update_helm_tpl():
     def update_helpers_tpl(root_path):
-        aws_hostname = get_env_var('AWS_HOSTNAME')
-        app_name = get_env_var('APP_NAME')
+        hostname = get_env_var('AWS_HOSTNAME')
+        repository = get_env_var('AWS_REPOSITORY')
         image_version = get_env_var('IMAGE_VERSION')
         path = get_file_path('_helpers.tpl', root_path)
-        pattern = rf'({{{{- define "{app_name}.image" }}}}{aws_hostname}\/{app_name}:)[\d.]+({{{{- end -}}}})'
+        pattern = rf'({{{{- define "{repository}.image" }}}}{hostname}\/{repository}:)[\d.]+({{{{- end -}}}})'
         _update_file(path, pattern, rf'\g<1>{image_version}\g<2>')
 
     def update_chart_config(root_path):
         chart_version = get_env_var('CHART_VERSION')
         path = get_file_path('Chart.yaml', root_path)
         _update_file(path, r'version: [\d.]+', f'version: {chart_version}')
 
     root_path = get_env_var('HELM_TPL_DIR')
     update_helpers_tpl(root_path)
     update_chart_config(root_path)
 
 
 def update_manifest(manifest_path: str):
-    app_name = get_env_var('APP_NAME')
+    repository = get_env_var('AWS_REPOSITORY')
     chart_version = get_env_var('CHART_VERSION')
     pattern = (
-        rf'("chartName":"adi\/{app_name}",(\n\s*)?"chartVersion":")[\d.]+'
+        rf'("chartName":"adi\/{repository}",(\n\s*)?"chartVersion":")[\d.]+'
     )
     _update_file(manifest_path, pattern, rf'\g<1>{chart_version}')
 
 
 def update_setup_cfg(project_dir=None, version=None):
     if not project_dir:
         project_dir = get_env_var('GITHUB_WORKSPACE')
```

### Comparing `isee-0.1.8/isee/generation_utils.py` & `isee-0.1.9/isee/generation_utils.py`

 * *Files identical despite different names*

### Comparing `isee-0.1.8/isee/git_utils.py` & `isee-0.1.9/isee/git_utils.py`

 * *Files identical despite different names*

### Comparing `isee-0.1.8/isee.egg-info/PKG-INFO` & `isee-0.1.9/isee.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: isee
-Version: 0.1.8
+Version: 0.1.9
 Summary: Python continuous integration (CI) support tools.
 Home-page: https://github.com/i2mint/isee
 Author: OtoSense
 License: mit
 Description: # Introduction
         Python continuous integration (CI) support tools.
```

### Comparing `isee-0.1.8/setup.cfg` & `isee-0.1.9/setup.cfg`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = isee
-version = 0.1.8
+version = 0.1.9
 url = https://github.com/i2mint/isee
 platforms = any
 description_file = README.md
 root_url = https://github.com/i2mint/
 license = mit
 author = OtoSense
 description = Python continuous integration (CI) support tools.
```

