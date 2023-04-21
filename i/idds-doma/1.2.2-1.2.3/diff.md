# Comparing `tmp/idds-doma-1.2.2.tar.gz` & `tmp/idds-doma-1.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "idds-doma-1.2.2.tar", last modified: Wed Apr 19 10:36:00 2023, max compression
+gzip compressed data, was "idds-doma-1.2.3.tar", last modified: Fri Apr 21 12:33:21 2023, max compression
```

## Comparing `idds-doma-1.2.2.tar` & `idds-doma-1.2.3.tar`

### file list

```diff
@@ -1,30 +1,30 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/
--rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-19 10:35:37.000000 idds-doma-1.2.2/LICENSE.rst
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-19 10:36:00.554242 idds-doma-1.2.2/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-19 10:35:37.000000 idds-doma-1.2.2/README.md
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/bin/
--rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-04-19 10:35:37.000000 idds-doma-1.2.2/bin/setup_panda_token
--rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-04-19 10:35:37.000000 idds-doma-1.2.2/bin/setup_panda_token.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/lib/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/lib/idds/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 10:35:37.000000 idds-doma-1.2.2/lib/idds/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/lib/idds/doma/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 10:35:37.000000 idds-doma-1.2.2/lib/idds/doma/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-19 10:35:53.000000 idds-doma-1.2.2/lib/idds/doma/version.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/lib/idds/doma/workflow/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 10:35:37.000000 idds-doma-1.2.2/lib/idds/doma/workflow/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-04-19 10:35:37.000000 idds-doma-1.2.2/lib/idds/doma/workflow/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/lib/idds/doma/workflowv2/
--rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-19 10:35:37.000000 idds-doma-1.2.2/lib/idds/doma/workflowv2/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)    68326 2023-04-19 10:35:37.000000 idds-doma-1.2.2/lib/idds/doma/workflowv2/domapandawork.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/lib/idds_doma.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-19 10:36:00.000000 idds-doma-1.2.2/lib/idds_doma.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-19 10:36:00.000000 idds-doma-1.2.2/lib/idds_doma.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-19 10:36:00.000000 idds-doma-1.2.2/lib/idds_doma.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-19 10:36:00.000000 idds-doma-1.2.2/lib/idds_doma.egg-info/requires.txt
--rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-19 10:36:00.000000 idds-doma-1.2.2/lib/idds_doma.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-19 10:36:00.554242 idds-doma-1.2.2/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-19 10:35:37.000000 idds-doma-1.2.2/setup.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/tools/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-19 10:36:00.554242 idds-doma-1.2.2/tools/env/
--rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-19 10:35:53.000000 idds-doma-1.2.2/tools/env/environment.yml
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.298720 idds-doma-1.2.3/
+-rw-r--r--   0 runner    (1001) docker     (123)      569 2023-04-21 12:33:07.000000 idds-doma-1.2.3/LICENSE.rst
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-21 12:33:21.298720 idds-doma-1.2.3/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      132 2023-04-21 12:33:07.000000 idds-doma-1.2.3/README.md
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.294720 idds-doma-1.2.3/bin/
+-rwxr-xr-x   0 runner    (1001) docker     (123)      747 2023-04-21 12:33:07.000000 idds-doma-1.2.3/bin/setup_panda_token
+-rwxr-xr-x   0 runner    (1001) docker     (123)    10028 2023-04-21 12:33:07.000000 idds-doma-1.2.3/bin/setup_panda_token.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.294720 idds-doma-1.2.3/lib/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.294720 idds-doma-1.2.3/lib/idds/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 12:33:07.000000 idds-doma-1.2.3/lib/idds/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.294720 idds-doma-1.2.3/lib/idds/doma/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 12:33:07.000000 idds-doma-1.2.3/lib/idds/doma/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      333 2023-04-21 12:33:15.000000 idds-doma-1.2.3/lib/idds/doma/version.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.294720 idds-doma-1.2.3/lib/idds/doma/workflow/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 12:33:07.000000 idds-doma-1.2.3/lib/idds/doma/workflow/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    56124 2023-04-21 12:33:07.000000 idds-doma-1.2.3/lib/idds/doma/workflow/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.294720 idds-doma-1.2.3/lib/idds/doma/workflowv2/
+-rw-r--r--   0 runner    (1001) docker     (123)      298 2023-04-21 12:33:07.000000 idds-doma-1.2.3/lib/idds/doma/workflowv2/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)    68326 2023-04-21 12:33:07.000000 idds-doma-1.2.3/lib/idds/doma/workflowv2/domapandawork.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.298720 idds-doma-1.2.3/lib/idds_doma.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)      705 2023-04-21 12:33:21.000000 idds-doma-1.2.3/lib/idds_doma.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      523 2023-04-21 12:33:21.000000 idds-doma-1.2.3/lib/idds_doma.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 12:33:21.000000 idds-doma-1.2.3/lib/idds_doma.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)       99 2023-04-21 12:33:21.000000 idds-doma-1.2.3/lib/idds_doma.egg-info/requires.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        5 2023-04-21 12:33:21.000000 idds-doma-1.2.3/lib/idds_doma.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      138 2023-04-21 12:33:21.298720 idds-doma-1.2.3/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (123)     3521 2023-04-21 12:33:07.000000 idds-doma-1.2.3/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.294720 idds-doma-1.2.3/tools/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 12:33:21.298720 idds-doma-1.2.3/tools/env/
+-rw-r--r--   0 runner    (1001) docker     (123)      437 2023-04-21 12:33:15.000000 idds-doma-1.2.3/tools/env/environment.yml
```

### Comparing `idds-doma-1.2.2/LICENSE.rst` & `idds-doma-1.2.3/LICENSE.rst`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.2/PKG-INFO` & `idds-doma-1.2.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.2.2
+Version: 1.2.3
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.2.2/bin/setup_panda_token` & `idds-doma-1.2.3/bin/setup_panda_token`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.2/bin/setup_panda_token.py` & `idds-doma-1.2.3/bin/setup_panda_token.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.2/lib/idds/doma/workflow/domapandawork.py` & `idds-doma-1.2.3/lib/idds/doma/workflow/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.2/lib/idds/doma/workflowv2/domapandawork.py` & `idds-doma-1.2.3/lib/idds/doma/workflowv2/domapandawork.py`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.2/lib/idds_doma.egg-info/PKG-INFO` & `idds-doma-1.2.3/lib/idds_doma.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: idds-doma
-Version: 1.2.2
+Version: 1.2.3
 Summary: intelligent Data Delivery Service(iDDS) Package
 Author: IRIS-HEP Team
 Author-email: atlas-adc-panda@cern.ch
 License: GPL
 Project-URL: Documentation, https://github.com/HSF/iDDS/wiki
 Project-URL: Source, https://github.com/HSF/iDDS
 Classifier: Development Status :: 5 - Production/Stable
```

### Comparing `idds-doma-1.2.2/lib/idds_doma.egg-info/SOURCES.txt` & `idds-doma-1.2.3/lib/idds_doma.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `idds-doma-1.2.2/setup.py` & `idds-doma-1.2.3/setup.py`

 * *Files identical despite different names*

