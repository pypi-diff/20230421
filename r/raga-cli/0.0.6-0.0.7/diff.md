# Comparing `tmp/raga-cli-0.0.6.tar.gz` & `tmp/raga-cli-0.0.7.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "raga-cli-0.0.6.tar", last modified: Thu Apr 20 11:36:48 2023, max compression
+gzip compressed data, was "raga-cli-0.0.7.tar", last modified: Fri Apr 21 12:55:59 2023, max compression
```

## Comparing `raga-cli-0.0.6.tar` & `raga-cli-0.0.7.tar`

### file list

```diff
@@ -1,41 +1,41 @@
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.829249 raga-cli-0.0.6/
--rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.0.6/.gitignore
--rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.0.6/LICENSE
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-20 11:36:48.828411 raga-cli-0.0.6/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.6/README.rst
--rw-r--r--   0 manabroy   (501) staff       (20)     2504 2023-04-12 11:10:34.000000 raga-cli-0.0.6/pyproject.toml
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.820402 raga-cli-0.0.6/raga_cli.egg-info/
--rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/PKG-INFO
--rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/SOURCES.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/dependency_links.txt
--rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/entry_points.txt
--rw-r--r--   0 manabroy   (501) staff       (20)     1029 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/requires.txt
--rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-20 11:36:48.000000 raga-cli-0.0.6/raga_cli.egg-info/top_level.txt
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.821416 raga-cli-0.0.6/rc/
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.822805 raga-cli-0.0.6/rc/cli/
--rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/cli/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.0.6/rc/cli/command.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.0.6/rc/cli/parser.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9323 2023-04-20 11:09:18.000000 raga-cli-0.0.6/rc/cli/utils.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.824224 raga-cli-0.0.6/rc/commands/
--rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/commands/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.0.6/rc/commands/list.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.0.6/rc/commands/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)     7737 2023-04-13 09:14:16.000000 raga-cli-0.0.6/rc/commands/repo.py
--rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/exceptions.py
--rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/prompt.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.825804 raga-cli-0.0.6/rc/repo/
--rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/repo/get.py
--rw-r--r--   0 manabroy   (501) staff       (20)     5050 2023-04-20 11:10:27.000000 raga-cli-0.0.6/rc/repo/put.py
--rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/repo/repo.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.826141 raga-cli-0.0.6/rc/stage/
--rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/stage/exceptions.py
-drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-20 11:36:48.827789 raga-cli-0.0.6/rc/utils/
--rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/utils/__init__.py
--rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/utils/auditLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/utils/fileLog.py
--rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.0.6/rc/utils/request.py
--rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/utils/sshKeyGen.py
--rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.0.6/rc/version.py
--rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-20 11:36:48.829350 raga-cli-0.0.6/setup.cfg
--rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.0.6/setup.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.525062 raga-cli-0.0.7/
+-rw-r--r--   0 manabroy   (501) staff       (20)      741 2023-04-10 13:07:16.000000 raga-cli-0.0.7/.gitignore
+-rw-r--r--   0 manabroy   (501) staff       (20)    11350 2023-04-10 13:07:16.000000 raga-cli-0.0.7/LICENSE
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-21 12:55:59.524686 raga-cli-0.0.7/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.7/README.rst
+-rw-r--r--   0 manabroy   (501) staff       (20)     2504 2023-04-21 12:54:24.000000 raga-cli-0.0.7/pyproject.toml
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.516887 raga-cli-0.0.7/raga_cli.egg-info/
+-rw-r--r--   0 manabroy   (501) staff       (20)      957 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/PKG-INFO
+-rw-r--r--   0 manabroy   (501) staff       (20)      612 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/SOURCES.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/dependency_links.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)       35 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/entry_points.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)     1029 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/requires.txt
+-rw-r--r--   0 manabroy   (501) staff       (20)        3 2023-04-21 12:55:59.000000 raga-cli-0.0.7/raga_cli.egg-info/top_level.txt
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.517781 raga-cli-0.0.7/rc/
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.519320 raga-cli-0.0.7/rc/cli/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3473 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/cli/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      292 2023-04-12 12:54:24.000000 raga-cli-0.0.7/rc/cli/command.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2074 2023-04-12 11:10:34.000000 raga-cli-0.0.7/rc/cli/parser.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9323 2023-04-20 11:09:18.000000 raga-cli-0.0.7/rc/cli/utils.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.520892 raga-cli-0.0.7/rc/commands/
+-rw-r--r--   0 manabroy   (501) staff       (20)     3226 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/commands/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1634 2023-04-12 11:10:34.000000 raga-cli-0.0.7/rc/commands/list.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1735 2023-04-13 04:42:45.000000 raga-cli-0.0.7/rc/commands/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     7737 2023-04-13 09:14:16.000000 raga-cli-0.0.7/rc/commands/repo.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     9835 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/exceptions.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     1298 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/prompt.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.522429 raga-cli-0.0.7/rc/repo/
+-rw-r--r--   0 manabroy   (501) staff       (20)      938 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/repo/get.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     5050 2023-04-20 11:10:27.000000 raga-cli-0.0.7/rc/repo/put.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        1 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/repo/repo.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.522729 raga-cli-0.0.7/rc/stage/
+-rw-r--r--   0 manabroy   (501) staff       (20)       85 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/stage/exceptions.py
+drwxr-xr-x   0 manabroy   (501) staff       (20)        0 2023-04-21 12:55:59.524167 raga-cli-0.0.7/rc/utils/
+-rw-r--r--   0 manabroy   (501) staff       (20)     1855 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/utils/__init__.py
+-rw-r--r--   0 manabroy   (501) staff       (20)        0 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/utils/auditLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       46 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/utils/fileLog.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     6464 2023-04-19 07:04:43.000000 raga-cli-0.0.7/rc/utils/request.py
+-rw-r--r--   0 manabroy   (501) staff       (20)     2924 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/utils/sshKeyGen.py
+-rw-r--r--   0 manabroy   (501) staff       (20)      248 2023-04-10 13:07:16.000000 raga-cli-0.0.7/rc/version.py
+-rw-r--r--   0 manabroy   (501) staff       (20)       38 2023-04-21 12:55:59.525146 raga-cli-0.0.7/setup.cfg
+-rw-r--r--   0 manabroy   (501) staff       (20)       47 2023-04-10 13:07:16.000000 raga-cli-0.0.7/setup.py
```

### Comparing `raga-cli-0.0.6/.gitignore` & `raga-cli-0.0.7/.gitignore`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/LICENSE` & `raga-cli-0.0.7/LICENSE`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/PKG-INFO` & `raga-cli-0.0.7/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.0.6/pyproject.toml` & `raga-cli-0.0.7/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = ["setuptools>=61", "setuptools_scm[toml]>=7"]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "raga-cli"
-version = "0.0.6"
+version = "0.0.7"
 description = "Git for data scientists - manage your code and data together"
 readme = "README.rst"
 requires-python = ">=3.7"
 keywords = [
     "data-science",
     "data-version-control",
     "machine-learning",
```

### Comparing `raga-cli-0.0.6/raga_cli.egg-info/PKG-INFO` & `raga-cli-0.0.7/raga_cli.egg-info/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: raga-cli
-Version: 0.0.6
+Version: 0.0.7
 Summary: Git for data scientists - manage your code and data together
 Author-email: Manab Roy <manabr@observancegroup.com>
 Maintainer-email: Manab Roy <support@observancegroup.com>
 License: Apache License 2.0
 Project-URL: Homepage, https://github.com/pypa/sampleproject
 Project-URL: Bug Tracker, https://github.com/pypa/sampleproject/issues
 Keywords: data-science,data-version-control,machine-learning,git,developer-tools,reproducibility,collaboration,ai,raga
```

### Comparing `raga-cli-0.0.6/raga_cli.egg-info/SOURCES.txt` & `raga-cli-0.0.7/raga_cli.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/raga_cli.egg-info/requires.txt` & `raga-cli-0.0.7/raga_cli.egg-info/requires.txt`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/cli/__init__.py` & `raga-cli-0.0.7/rc/cli/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/cli/parser.py` & `raga-cli-0.0.7/rc/cli/parser.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/cli/utils.py` & `raga-cli-0.0.7/rc/cli/utils.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/commands/get.py` & `raga-cli-0.0.7/rc/commands/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/commands/list.py` & `raga-cli-0.0.7/rc/commands/list.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/commands/put.py` & `raga-cli-0.0.7/rc/commands/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/commands/repo.py` & `raga-cli-0.0.7/rc/commands/repo.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/exceptions.py` & `raga-cli-0.0.7/rc/exceptions.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/prompt.py` & `raga-cli-0.0.7/rc/prompt.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/repo/get.py` & `raga-cli-0.0.7/rc/repo/get.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/repo/put.py` & `raga-cli-0.0.7/rc/repo/put.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/utils/__init__.py` & `raga-cli-0.0.7/rc/utils/__init__.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/utils/request.py` & `raga-cli-0.0.7/rc/utils/request.py`

 * *Files identical despite different names*

### Comparing `raga-cli-0.0.6/rc/utils/sshKeyGen.py` & `raga-cli-0.0.7/rc/utils/sshKeyGen.py`

 * *Files identical despite different names*

