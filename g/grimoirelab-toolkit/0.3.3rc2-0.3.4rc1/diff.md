# Comparing `tmp/grimoirelab_toolkit-0.3.3rc2.tar.gz` & `tmp/grimoirelab_toolkit-0.3.4rc1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "grimoirelab_toolkit-0.3.3rc2.tar", max compression
+gzip compressed data, was "grimoirelab_toolkit-0.3.4rc1.tar", max compression
```

## Comparing `grimoirelab_toolkit-0.3.3rc2.tar` & `grimoirelab_toolkit-0.3.4rc1.tar`

### file list

```diff
@@ -1,16 +1,15 @@
--rw-r--r--   0        0        0      229 2023-02-01 08:41:10.853552 grimoirelab_toolkit-0.3.3rc2/AUTHORS
--rw-r--r--   0        0        0    35147 2023-02-01 08:41:10.853552 grimoirelab_toolkit-0.3.3rc2/LICENSE
--rw-r--r--   0        0        0      911 2023-02-01 08:41:10.853552 grimoirelab_toolkit-0.3.3rc2/NEWS
--rw-r--r--   0        0        0     2091 2023-02-01 08:41:10.853552 grimoirelab_toolkit-0.3.3rc2/README.md
--rw-r--r--   0        0        0     1011 2023-02-01 08:41:10.853552 grimoirelab_toolkit-0.3.3rc2/grimoirelab_toolkit/__init__.py
--rw-r--r--   0        0        0       91 2023-02-01 08:41:10.853552 grimoirelab_toolkit-0.3.3rc2/grimoirelab_toolkit/_version.py
--rw-r--r--   0        0        0     5606 2023-02-01 08:41:10.853552 grimoirelab_toolkit-0.3.3rc2/grimoirelab_toolkit/datetime.py
--rw-r--r--   0        0        0     3846 2023-02-01 08:41:10.853552 grimoirelab_toolkit-0.3.3rc2/grimoirelab_toolkit/introspect.py
--rw-r--r--   0        0        0     1383 2023-02-01 08:41:10.857552 grimoirelab_toolkit-0.3.3rc2/grimoirelab_toolkit/uris.py
--rw-r--r--   0        0        0     1119 2023-02-01 08:41:10.857552 grimoirelab_toolkit-0.3.3rc2/pyproject.toml
--rwxr-xr-x   0        0        0     1063 2023-02-01 08:41:10.857552 grimoirelab_toolkit-0.3.3rc2/tests/run_tests.py
--rw-r--r--   0        0        0    10186 2023-02-01 08:41:10.857552 grimoirelab_toolkit-0.3.3rc2/tests/test_datetime.py
--rw-r--r--   0        0        0     7078 2023-02-01 08:41:10.857552 grimoirelab_toolkit-0.3.3rc2/tests/test_introspect.py
--rw-r--r--   0        0        0     2678 2023-02-01 08:41:10.857552 grimoirelab_toolkit-0.3.3rc2/tests/test_uris.py
--rw-r--r--   0        0        0     2866 1970-01-01 00:00:00.000000 grimoirelab_toolkit-0.3.3rc2/setup.py
--rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 grimoirelab_toolkit-0.3.3rc2/PKG-INFO
+-rw-r--r--   0        0        0      229 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/AUTHORS
+-rw-r--r--   0        0        0    35147 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/LICENSE
+-rw-r--r--   0        0        0     1002 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/NEWS
+-rw-r--r--   0        0        0     2091 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/README.md
+-rw-r--r--   0        0        0     1011 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/__init__.py
+-rw-r--r--   0        0        0       91 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/_version.py
+-rw-r--r--   0        0        0     5606 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/datetime.py
+-rw-r--r--   0        0        0     3846 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/introspect.py
+-rw-r--r--   0        0        0     1383 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/uris.py
+-rw-r--r--   0        0        0     1119 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/pyproject.toml
+-rwxr-xr-x   0        0        0     1063 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/tests/run_tests.py
+-rw-r--r--   0        0        0    10186 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/tests/test_datetime.py
+-rw-r--r--   0        0        0     7078 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/tests/test_introspect.py
+-rw-r--r--   0        0        0     2678 2023-04-20 14:54:24.751743 grimoirelab_toolkit-0.3.4rc1/tests/test_uris.py
+-rw-r--r--   0        0        0     3103 1970-01-01 00:00:00.000000 grimoirelab_toolkit-0.3.4rc1/PKG-INFO
```

### Comparing `grimoirelab_toolkit-0.3.3rc2/LICENSE` & `grimoirelab_toolkit-0.3.4rc1/LICENSE`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/NEWS` & `grimoirelab_toolkit-0.3.4rc1/NEWS`

 * *Files 8% similar despite different names*

```diff
@@ -1,9 +1,13 @@
 # Releases
 
+  ## grimoirelab-toolkit 0.3.3 - (2023-02-01)
+  
+  * Update Poetry's package dependencies
+
   ## grimoirelab-toolkit 0.3.2 - (2022-10-31)
   
   * Update Poetry's package dependencies
 
 ## grimoirelab-toolkit 0.3.0 - (2022-05-31)
 
 **Feature removals:**
```

### Comparing `grimoirelab_toolkit-0.3.3rc2/README.md` & `grimoirelab_toolkit-0.3.4rc1/README.md`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/grimoirelab_toolkit/__init__.py` & `grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/__init__.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/grimoirelab_toolkit/datetime.py` & `grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/datetime.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/grimoirelab_toolkit/introspect.py` & `grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/introspect.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/grimoirelab_toolkit/uris.py` & `grimoirelab_toolkit-0.3.4rc1/grimoirelab_toolkit/uris.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/pyproject.toml` & `grimoirelab_toolkit-0.3.4rc1/pyproject.toml`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "grimoirelab-toolkit"
-version = "0.3.3-rc.2"
+version = "0.3.4-rc.1"
 description = "Toolkit of common functions used across GrimoireLab"
 authors = [
     "GrimoireLab Developers"
 ]
 license = "GPL-3.0+"
 
 readme = "README.md"
```

### Comparing `grimoirelab_toolkit-0.3.3rc2/tests/run_tests.py` & `grimoirelab_toolkit-0.3.4rc1/tests/run_tests.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/tests/test_datetime.py` & `grimoirelab_toolkit-0.3.4rc1/tests/test_datetime.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/tests/test_introspect.py` & `grimoirelab_toolkit-0.3.4rc1/tests/test_introspect.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/tests/test_uris.py` & `grimoirelab_toolkit-0.3.4rc1/tests/test_uris.py`

 * *Files identical despite different names*

### Comparing `grimoirelab_toolkit-0.3.3rc2/PKG-INFO` & `grimoirelab_toolkit-0.3.4rc1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: grimoirelab-toolkit
-Version: 0.3.3rc2
+Version: 0.3.4rc1
 Summary: Toolkit of common functions used across GrimoireLab
 Home-page: https://chaoss.github.io/grimoirelab/
 License: GPL-3.0+
 Keywords: development,grimoirelab
 Author: GrimoireLab Developers
 Requires-Python: >=3.7,<4.0
 Classifier: Development Status :: 4 - Beta
```

