# Comparing `tmp/dedscumulus-0.0.1.tar.gz` & `tmp/dedscumulus-0.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dedscumulus-0.0.1.tar", last modified: Fri Apr 21 00:58:27 2023, max compression
+gzip compressed data, was "dedscumulus-0.0.3.tar", last modified: Fri Apr 21 01:31:43 2023, max compression
```

## Comparing `dedscumulus-0.0.1.tar` & `dedscumulus-0.0.3.tar`

### file list

```diff
@@ -1,21 +1,21 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 00:58:27.267741 dedscumulus-0.0.1/
--rw-rw-rw-   0        0        0     1091 2023-04-20 20:25:57.000000 dedscumulus-0.0.1/LICENSE
--rw-rw-rw-   0        0        0      527 2023-04-21 00:58:27.267741 dedscumulus-0.0.1/PKG-INFO
--rw-rw-rw-   0        0        0       43 2023-04-21 00:56:16.000000 dedscumulus-0.0.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 00:58:27.249735 dedscumulus-0.0.1/dedscumulus.egg-info/
--rw-rw-rw-   0        0        0      527 2023-04-21 00:58:27.000000 dedscumulus-0.0.1/dedscumulus.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      339 2023-04-21 00:58:27.000000 dedscumulus-0.0.1/dedscumulus.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 00:58:27.000000 dedscumulus-0.0.1/dedscumulus.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        4 2023-04-21 00:58:27.000000 dedscumulus-0.0.1/dedscumulus.egg-info/top_level.txt
--rw-rw-rw-   0        0        0      225 2023-04-21 00:23:51.000000 dedscumulus-0.0.1/pyproject.toml
--rw-rw-rw-   0        0        0      593 2023-04-21 00:58:27.276733 dedscumulus-0.0.1/setup.cfg
--rw-rw-rw-   0        0        0      703 2023-04-21 00:54:15.000000 dedscumulus-0.0.1/setup.py
-drwxrwxrwx   0        0        0        0 2023-04-21 00:58:27.265732 dedscumulus-0.0.1/src/
--rw-rw-rw-   0        0        0      522 2023-02-13 21:12:26.000000 dedscumulus-0.0.1/src/RequestHandler.py
--rw-rw-rw-   0        0        0    14421 2023-02-13 13:17:25.000000 dedscumulus-0.0.1/src/SharePointHandler.py
--rw-rw-rw-   0        0        0     2250 2023-02-20 20:06:50.000000 dedscumulus-0.0.1/src/TableLogHandler.py
--rw-rw-rw-   0        0        0        0 2022-05-17 10:12:58.000000 dedscumulus-0.0.1/src/__init__.py
--rw-rw-rw-   0        0        0     8815 2023-02-21 02:51:22.000000 dedscumulus-0.0.1/src/brzGlobal.py
--rw-rw-rw-   0        0        0     4990 2023-04-18 16:46:19.000000 dedscumulus-0.0.1/src/gbtGlobal.py
--rw-rw-rw-   0        0        0    13474 2023-04-16 12:34:10.000000 dedscumulus-0.0.1/src/mstAst.py
--rw-rw-rw-   0        0        0      823 2023-04-20 21:56:20.000000 dedscumulus-0.0.1/src/mstLog.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:31:43.006254 dedscumulus-0.0.3/
+-rw-rw-rw-   0        0        0     1091 2023-04-20 20:25:57.000000 dedscumulus-0.0.3/LICENSE
+-rw-rw-rw-   0        0        0      527 2023-04-21 01:31:43.006907 dedscumulus-0.0.3/PKG-INFO
+-rw-rw-rw-   0        0        0       43 2023-04-21 00:56:16.000000 dedscumulus-0.0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 01:31:42.911472 dedscumulus-0.0.3/dedscumulus.egg-info/
+-rw-rw-rw-   0        0        0      527 2023-04-21 01:31:42.000000 dedscumulus-0.0.3/dedscumulus.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      339 2023-04-21 01:31:42.000000 dedscumulus-0.0.3/dedscumulus.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 01:31:42.000000 dedscumulus-0.0.3/dedscumulus.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        4 2023-04-21 01:31:42.000000 dedscumulus-0.0.3/dedscumulus.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0      235 2023-04-21 01:29:23.000000 dedscumulus-0.0.3/pyproject.toml
+-rw-rw-rw-   0        0        0      593 2023-04-21 01:31:43.017247 dedscumulus-0.0.3/setup.cfg
+-rw-rw-rw-   0        0        0      703 2023-04-21 01:24:47.000000 dedscumulus-0.0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 01:31:43.003906 dedscumulus-0.0.3/src/
+-rw-rw-rw-   0        0        0      522 2023-02-13 21:12:26.000000 dedscumulus-0.0.3/src/RequestHandler.py
+-rw-rw-rw-   0        0        0    14421 2023-02-13 13:17:25.000000 dedscumulus-0.0.3/src/SharePointHandler.py
+-rw-rw-rw-   0        0        0     2250 2023-02-20 20:06:50.000000 dedscumulus-0.0.3/src/TableLogHandler.py
+-rw-rw-rw-   0        0        0        0 2022-05-17 10:12:58.000000 dedscumulus-0.0.3/src/__init__.py
+-rw-rw-rw-   0        0        0     8815 2023-02-21 02:51:22.000000 dedscumulus-0.0.3/src/brzGlobal.py
+-rw-rw-rw-   0        0        0     4990 2023-04-18 16:46:19.000000 dedscumulus-0.0.3/src/gbtGlobal.py
+-rw-rw-rw-   0        0        0    13474 2023-04-16 12:34:10.000000 dedscumulus-0.0.3/src/mstAst.py
+-rw-rw-rw-   0        0        0      823 2023-04-20 21:56:20.000000 dedscumulus-0.0.3/src/mstLog.py
```

### Comparing `dedscumulus-0.0.1/LICENSE` & `dedscumulus-0.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.0.1/PKG-INFO` & `dedscumulus-0.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedscumulus
-Version: 0.0.1
+Version: 0.0.3
 Summary: Kernel functions for Cumulus
 Home-page: https://github.com/nino-baywa/dedscumulus
 Author: BayWa r.e. Data Services GmbH
 Author-email: no-reply@baywa-re.com
 Project-URL: repository, https://github.com/nino-baywa/dedscumulus
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `dedscumulus-0.0.1/dedscumulus.egg-info/PKG-INFO` & `dedscumulus-0.0.3/dedscumulus.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: dedscumulus
-Version: 0.0.1
+Version: 0.0.3
 Summary: Kernel functions for Cumulus
 Home-page: https://github.com/nino-baywa/dedscumulus
 Author: BayWa r.e. Data Services GmbH
 Author-email: no-reply@baywa-re.com
 Project-URL: repository, https://github.com/nino-baywa/dedscumulus
 Classifier: Programming Language :: Python :: 3
 Classifier: Operating System :: OS Independent
```

### Comparing `dedscumulus-0.0.1/setup.cfg` & `dedscumulus-0.0.3/setup.cfg`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 00000000: 5b6d 6574 6164 6174 615d 0d0a 6e61 6d65  [metadata]..name
 00000010: 203d 2064 6564 7363 756d 756c 7573 0d0a   = dedscumulus..
-00000020: 7665 7273 696f 6e20 3d20 302e 302e 310d  version = 0.0.1.
+00000020: 7665 7273 696f 6e20 3d20 302e 302e 330d  version = 0.0.3.
 00000030: 0a61 7574 686f 7220 3d20 4261 7957 6120  .author = BayWa 
 00000040: 722e 652e 2044 6174 6120 5365 7276 6963  r.e. Data Servic
 00000050: 6573 2047 6d62 480d 0a61 7574 686f 725f  es GmbH..author_
 00000060: 656d 6169 6c20 3d20 6e6f 2d72 6570 6c79  email = no-reply
 00000070: 4062 6179 7761 2d72 652e 636f 6d0d 0a64  @baywa-re.com..d
 00000080: 6573 6372 6970 7469 6f6e 203d 204b 6572  escription = Ker
 00000090: 6e65 6c20 6675 6e63 7469 6f6e 7320 666f  nel functions fo
```

### Comparing `dedscumulus-0.0.1/setup.py` & `dedscumulus-0.0.3/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -2,15 +2,15 @@
 
 with open("README.md", "r") as fh:
     long_description = fh.read()
 
 
 setuptools.setup(
      name='dedscumulus',  
-     version='0.0.1',
+     version='0.0.3',
      author="BayWa r.e. Data Services GmbH",
      author_email="no-reply@baywa-re.com",
      description="Kernel functions for Cumulus",
      long_description=long_description,
      long_description_content_type="text/markdown",
      url="https://github.com/nino-baywa/dedscumulus",
      classifiers=[
```

### Comparing `dedscumulus-0.0.1/src/RequestHandler.py` & `dedscumulus-0.0.3/src/RequestHandler.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.0.1/src/SharePointHandler.py` & `dedscumulus-0.0.3/src/SharePointHandler.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.0.1/src/TableLogHandler.py` & `dedscumulus-0.0.3/src/TableLogHandler.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.0.1/src/brzGlobal.py` & `dedscumulus-0.0.3/src/brzGlobal.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.0.1/src/gbtGlobal.py` & `dedscumulus-0.0.3/src/gbtGlobal.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.0.1/src/mstAst.py` & `dedscumulus-0.0.3/src/mstAst.py`

 * *Files identical despite different names*

### Comparing `dedscumulus-0.0.1/src/mstLog.py` & `dedscumulus-0.0.3/src/mstLog.py`

 * *Files identical despite different names*

