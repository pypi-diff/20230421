# Comparing `tmp/netbox-network-diagram-0.1.0.tar.gz` & `tmp/netbox-network-diagram-0.1.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "netbox-network-diagram-0.1.0.tar", last modified: Fri Apr 21 08:35:16 2023, max compression
+gzip compressed data, was "netbox-network-diagram-0.1.2.tar", last modified: Fri Apr 21 15:42:16 2023, max compression
```

## Comparing `netbox-network-diagram-0.1.0.tar` & `netbox-network-diagram-0.1.2.tar`

### file list

```diff
@@ -1,36 +1,37 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.666735 netbox-network-diagram-0.1.0/
--rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-21 08:35:16.666735 netbox-network-diagram-0.1.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)       73 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.662735 netbox-network-diagram-0.1.0/netbox_network_diagram/
--rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.662735 netbox-network-diagram-0.1.0/netbox_network_diagram/api/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/api/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.662735 netbox-network-diagram-0.1.0/netbox_network_diagram/migrations/
--rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/migrations/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/navigation.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.662735 netbox-network-diagram-0.1.0/netbox_network_diagram/static/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.662735 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.662735 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/css/
--rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/css/style.css
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.666735 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/img/
--rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/img/ix.png
--rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/img/nat.png
--rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/img/router.png
--rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/img/switch.png
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.666735 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/js/
--rw-r--r--   0 runner    (1001) docker     (123)    79546 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/js/cola.min.js
--rw-r--r--   0 runner    (1001) docker     (123)    34426 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/js/inet-henge.min.js
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.662735 netbox-network-diagram-0.1.0/netbox_network_diagram/templates/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.666735 netbox-network-diagram-0.1.0/netbox_network_diagram/templates/netbox_network_diagram/
--rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/templates/netbox_network_diagram/index.html
--rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/urls.py
--rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/netbox_network_diagram/views.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 08:35:16.662735 netbox-network-diagram-0.1.0/netbox_network_diagram.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      683 2023-04-21 08:35:16.000000 netbox-network-diagram-0.1.0/netbox_network_diagram.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     1020 2023-04-21 08:35:16.000000 netbox-network-diagram-0.1.0/netbox_network_diagram.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:35:16.000000 netbox-network-diagram-0.1.0/netbox_network_diagram.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 08:35:16.000000 netbox-network-diagram-0.1.0/netbox_network_diagram.egg-info/not-zip-safe
--rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 08:35:16.000000 netbox-network-diagram-0.1.0/netbox_network_diagram.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 08:35:16.666735 netbox-network-diagram-0.1.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)      998 2023-04-21 08:35:05.000000 netbox-network-diagram-0.1.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.811503 netbox-network-diagram-0.1.2/
+-rw-r--r--   0 runner    (1001) docker     (123)    10174 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (123)      194 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-21 15:42:16.811503 netbox-network-diagram-0.1.2/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      202 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.807503 netbox-network-diagram-0.1.2/netbox_network_diagram/
+-rw-r--r--   0 runner    (1001) docker     (123)      353 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.807503 netbox-network-diagram-0.1.2/netbox_network_diagram/api/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/api/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.807503 netbox-network-diagram-0.1.2/netbox_network_diagram/migrations/
+-rw-r--r--   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/migrations/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      360 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/navigation.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.807503 netbox-network-diagram-0.1.2/netbox_network_diagram/static/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.807503 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.807503 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/css/
+-rw-r--r--   0 runner    (1001) docker     (123)      808 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/css/style.css
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.811503 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/img/
+-rw-r--r--   0 runner    (1001) docker     (123)     9087 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/img/ix.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15736 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/img/nat.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15505 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/img/router.png
+-rw-r--r--   0 runner    (1001) docker     (123)    15648 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/img/switch.png
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.811503 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/js/
+-rw-r--r--   0 runner    (1001) docker     (123)    79546 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/js/cola.min.js
+-rw-r--r--   0 runner    (1001) docker     (123)    34426 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/js/inet-henge.min.js
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.807503 netbox-network-diagram-0.1.2/netbox_network_diagram/templates/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.811503 netbox-network-diagram-0.1.2/netbox_network_diagram/templates/netbox_network_diagram/
+-rw-r--r--   0 runner    (1001) docker     (123)      958 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/templates/netbox_network_diagram/index.html
+-rw-r--r--   0 runner    (1001) docker     (123)      182 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/urls.py
+-rw-r--r--   0 runner    (1001) docker     (123)     2183 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/netbox_network_diagram/views.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 15:42:16.807503 netbox-network-diagram-0.1.2/netbox_network_diagram.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      849 2023-04-21 15:42:16.000000 netbox-network-diagram-0.1.2/netbox_network_diagram.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     1028 2023-04-21 15:42:16.000000 netbox-network-diagram-0.1.2/netbox_network_diagram.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:42:16.000000 netbox-network-diagram-0.1.2/netbox_network_diagram.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 15:42:16.000000 netbox-network-diagram-0.1.2/netbox_network_diagram.egg-info/not-zip-safe
+-rw-r--r--   0 runner    (1001) docker     (123)       23 2023-04-21 15:42:16.000000 netbox-network-diagram-0.1.2/netbox_network_diagram.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 15:42:16.811503 netbox-network-diagram-0.1.2/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     1013 2023-04-21 15:42:02.000000 netbox-network-diagram-0.1.2/setup.py
```

### Comparing `netbox-network-diagram-0.1.0/PKG-INFO` & `netbox-network-diagram-0.1.2/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: netbox-network-diagram
-Version: 0.1.0
+Version: 0.1.2
 Summary: A plugin to render network diagram in NetBox.
 Home-page: https://github.com/entooone/netbox-network-diagram
 Author: entooone
 Author-email: entooone@gmail.com
-License: MIT
+License: Apache License 2.0
 Project-URL: Source, https://github.com/entooone/netbox-network-diagram
 Project-URL: Tracker, https://github.com/entooone/netbox-network-diagram/issues
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## netbox-network-diagram
 
+[![Version](https://img.shields.io/pypi/v/netbox-network-diagram?color=blue)](https://pypi.org/project/netbox-network-diagram/)
+
 A plugin to render network diagram in NetBox.
```

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/css/style.css` & `netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/css/style.css`

 * *Files identical despite different names*

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/img/ix.png` & `netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/img/ix.png`

 * *Files identical despite different names*

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/img/nat.png` & `netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/img/nat.png`

 * *Files identical despite different names*

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/img/router.png` & `netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/img/router.png`

 * *Files identical despite different names*

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/img/switch.png` & `netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/img/switch.png`

 * *Files identical despite different names*

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/js/cola.min.js` & `netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/js/cola.min.js`

 * *Files identical despite different names*

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram/static/netbox_network_diagram/js/inet-henge.min.js` & `netbox-network-diagram-0.1.2/netbox_network_diagram/static/netbox_network_diagram/js/inet-henge.min.js`

 * *Files identical despite different names*

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram/templates/netbox_network_diagram/index.html` & `netbox-network-diagram-0.1.2/netbox_network_diagram/templates/netbox_network_diagram/index.html`

 * *Files identical despite different names*

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram/views.py` & `netbox-network-diagram-0.1.2/netbox_network_diagram/views.py`

 * *Files identical despite different names*

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram.egg-info/PKG-INFO` & `netbox-network-diagram-0.1.2/netbox_network_diagram.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,19 +1,22 @@
 Metadata-Version: 2.1
 Name: netbox-network-diagram
-Version: 0.1.0
+Version: 0.1.2
 Summary: A plugin to render network diagram in NetBox.
 Home-page: https://github.com/entooone/netbox-network-diagram
 Author: entooone
 Author-email: entooone@gmail.com
-License: MIT
+License: Apache License 2.0
 Project-URL: Source, https://github.com/entooone/netbox-network-diagram
 Project-URL: Tracker, https://github.com/entooone/netbox-network-diagram/issues
 Keywords: netbox-plugin
 Classifier: Programming Language :: Python
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3 :: Only
 Description-Content-Type: text/markdown
+License-File: LICENSE
 
 ## netbox-network-diagram
 
+[![Version](https://img.shields.io/pypi/v/netbox-network-diagram?color=blue)](https://pypi.org/project/netbox-network-diagram/)
+
 A plugin to render network diagram in NetBox.
```

### Comparing `netbox-network-diagram-0.1.0/netbox_network_diagram.egg-info/SOURCES.txt` & `netbox-network-diagram-0.1.2/netbox_network_diagram.egg-info/SOURCES.txt`

 * *Files 0% similar despite different names*

```diff
@@ -1,7 +1,8 @@
+LICENSE
 MANIFEST.in
 README.md
 setup.py
 netbox_network_diagram/__init__.py
 netbox_network_diagram/navigation.py
 netbox_network_diagram/urls.py
 netbox_network_diagram/views.py
```

### Comparing `netbox-network-diagram-0.1.0/setup.py` & `netbox-network-diagram-0.1.2/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,24 +1,24 @@
 #!/usr/bin/env python
 
 from setuptools import find_packages, setup
 
-with open('README.md') as readme_file:
+with open("README.md") as readme_file:
     long_description = readme_file.read()
 
 setup(
-    name='netbox-network-diagram',
-    version='0.1.0',
-    description='A plugin to render network diagram in NetBox.',
+    name="netbox-network-diagram",
+    version="0.1.2",
+    description="A plugin to render network diagram in NetBox.",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://github.com/entooone/netbox-network-diagram",
     author="entooone",
     author_email="entooone@gmail.com",
-    license='MIT',
+    license="Apache License 2.0",
     install_requires=[],
     keywords=["netbox-plugin"],
     packages=find_packages(),
     classifiers=[
         "Programming Language :: Python",
         "Programming Language :: Python :: 3",
         "Programming Language :: Python :: 3 :: Only",
```

