# Comparing `tmp/pyXhUtils-1.0.0.tar.gz` & `tmp/pyXhUtils-1.0.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyXhUtils-1.0.0.tar", last modified: Fri Apr 21 03:56:55 2023, max compression
+gzip compressed data, was "pyXhUtils-1.0.1.tar", last modified: Fri Apr 21 04:32:27 2023, max compression
```

## Comparing `pyXhUtils-1.0.0.tar` & `pyXhUtils-1.0.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/
--rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/LICENSE.txt
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/README.md
--rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/pyproject.toml
--rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/setup.cfg
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:56:55.715045 pyXhUtils-1.0.0/src/
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/src/pyXhUtils.egg-info/
--rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-21 03:56:55.000000 pyXhUtils-1.0.0/src/pyXhUtils.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-21 03:56:55.000000 pyXhUtils-1.0.0/src/pyXhUtils.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 03:56:55.000000 pyXhUtils-1.0.0/src/pyXhUtils.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 03:56:55.000000 pyXhUtils-1.0.0/src/pyXhUtils.egg-info/top_level.txt
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/src/xh_utils_apache_log/
--rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_apache_log/ApacheLog.py
--rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_apache_log/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/src/xh_utils_file_changes/
--rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_file_changes/FileChanges.py
--rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_file_changes/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/src/xh_utils_ip/
--rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_ip/IpHostFinder.py
--rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_ip/IpTools.py
--rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_ip/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/src/xh_utils_progress/
--rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_progress/ProgressPinger.py
--rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_progress/__init__.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/src/xh_utils_script_file_writer/
--rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_script_file_writer/__init__.py
--rw-r--r--   0 runner    (1001) docker     (123)      727 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_script_file_writer/script_writer.py
-drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 03:56:55.719045 pyXhUtils-1.0.0/src/xh_utils_string/
--rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_string/StringUtils.py
--rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 03:56:44.000000 pyXhUtils-1.0.0/src/xh_utils_string/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:32:27.295980 pyXhUtils-1.0.1/
+-rw-r--r--   0 runner    (1001) docker     (123)    35148 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/LICENSE.txt
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-21 04:32:27.295980 pyXhUtils-1.0.1/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)     2926 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/README.md
+-rw-r--r--   0 runner    (1001) docker     (123)      581 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/pyproject.toml
+-rw-r--r--   0 runner    (1001) docker     (123)       38 2023-04-21 04:32:27.295980 pyXhUtils-1.0.1/setup.cfg
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:32:27.291980 pyXhUtils-1.0.1/src/
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:32:27.291980 pyXhUtils-1.0.1/src/pyXhUtils.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (123)     3431 2023-04-21 04:32:27.000000 pyXhUtils-1.0.1/src/pyXhUtils.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (123)      657 2023-04-21 04:32:27.000000 pyXhUtils-1.0.1/src/pyXhUtils.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (123)        1 2023-04-21 04:32:27.000000 pyXhUtils-1.0.1/src/pyXhUtils.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (123)      116 2023-04-21 04:32:27.000000 pyXhUtils-1.0.1/src/pyXhUtils.egg-info/top_level.txt
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:32:27.291980 pyXhUtils-1.0.1/src/xh_utils_apache_log/
+-rw-r--r--   0 runner    (1001) docker     (123)     5989 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_apache_log/ApacheLog.py
+-rw-r--r--   0 runner    (1001) docker     (123)       49 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_apache_log/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:32:27.295980 pyXhUtils-1.0.1/src/xh_utils_file_changes/
+-rw-r--r--   0 runner    (1001) docker     (123)     5998 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_file_changes/FileChanges.py
+-rw-r--r--   0 runner    (1001) docker     (123)      130 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_file_changes/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:32:27.295980 pyXhUtils-1.0.1/src/xh_utils_ip/
+-rw-r--r--   0 runner    (1001) docker     (123)      442 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_ip/IpHostFinder.py
+-rw-r--r--   0 runner    (1001) docker     (123)     1739 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_ip/IpTools.py
+-rw-r--r--   0 runner    (1001) docker     (123)      123 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_ip/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:32:27.295980 pyXhUtils-1.0.1/src/xh_utils_progress/
+-rw-r--r--   0 runner    (1001) docker     (123)     1089 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_progress/ProgressPinger.py
+-rw-r--r--   0 runner    (1001) docker     (123)       59 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_progress/__init__.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:32:27.295980 pyXhUtils-1.0.1/src/xh_utils_script_file_writer/
+-rw-r--r--   0 runner    (1001) docker     (123)       67 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_script_file_writer/__init__.py
+-rw-r--r--   0 runner    (1001) docker     (123)      747 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_script_file_writer/script_writer.py
+drwxr-xr-x   0 runner    (1001) docker     (123)        0 2023-04-21 04:32:27.295980 pyXhUtils-1.0.1/src/xh_utils_string/
+-rw-r--r--   0 runner    (1001) docker     (123)      978 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_string/StringUtils.py
+-rw-r--r--   0 runner    (1001) docker     (123)       65 2023-04-21 04:32:15.000000 pyXhUtils-1.0.1/src/xh_utils_string/__init__.py
```

### Comparing `pyXhUtils-1.0.0/LICENSE.txt` & `pyXhUtils-1.0.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.0.0/PKG-INFO` & `pyXhUtils-1.0.1/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyXhUtils
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev-py/xhUtils
 Project-URL: Bug Tracker, https://github.com/xh-dev-py/xhUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyXhUtils-1.0.0/README.md` & `pyXhUtils-1.0.1/README.md`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.0.0/pyproject.toml` & `pyXhUtils-1.0.1/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 [build-system]
 requires = [ "setuptools>=61.0",]
 build-backend = "setuptools.build_meta"
 
 [project]
 name = "pyXhUtils"
-version = "1.0.0"
+version = "1.0.1"
 description = "A collection of self dev py library"
 readme = "README.md"
 requires-python = ">=3.6"
 classifiers = [ "Programming Language :: Python :: 3", "License :: OSI Approved :: MIT License", "Operating System :: OS Independent",]
 dependencies = []
 [[project.authors]]
 name = "xethhung"
```

### Comparing `pyXhUtils-1.0.0/src/pyXhUtils.egg-info/PKG-INFO` & `pyXhUtils-1.0.1/src/pyXhUtils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: pyXhUtils
-Version: 1.0.0
+Version: 1.0.1
 Summary: A collection of self dev py library
 Author-email: xethhung <pypi@xethh.dev>
 Project-URL: Homepage, https://github.com/xh-dev-py/xhUtils
 Project-URL: Bug Tracker, https://github.com/xh-dev-py/xhUtils/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
```

### Comparing `pyXhUtils-1.0.0/src/pyXhUtils.egg-info/SOURCES.txt` & `pyXhUtils-1.0.1/src/pyXhUtils.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.0.0/src/xh_utils_apache_log/ApacheLog.py` & `pyXhUtils-1.0.1/src/xh_utils_apache_log/ApacheLog.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.0.0/src/xh_utils_file_changes/FileChanges.py` & `pyXhUtils-1.0.1/src/xh_utils_file_changes/FileChanges.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.0.0/src/xh_utils_ip/IpTools.py` & `pyXhUtils-1.0.1/src/xh_utils_ip/IpTools.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.0.0/src/xh_utils_progress/ProgressPinger.py` & `pyXhUtils-1.0.1/src/xh_utils_progress/ProgressPinger.py`

 * *Files identical despite different names*

### Comparing `pyXhUtils-1.0.0/src/xh_utils_script_file_writer/script_writer.py` & `pyXhUtils-1.0.1/src/xh_utils_script_file_writer/script_writer.py`

 * *Files 8% similar despite different names*

```diff
@@ -9,14 +9,15 @@
         with open(file_name, "w") as f:
             op(f)
 
         if executable:
             st = os.stat(file_name)
             os.chmod(file_name, st.st_mode | stat.S_IEXEC)
 
-    def write_script_text(self, file_name: str, text: str, executable: bool = False):
-        self.write_script(file_name, lambda f: f.write(text), executable=executable)
+    @staticmethod
+    def write_script_text(file_name: str, text: str, executable: bool = False):
+        ScriptWriter.write_script(file_name, lambda f: f.write(text), executable=executable)
 
 
 if __name__ == '__main__':
     ScriptWriter.write_script("test.txt", lambda f: f.write("hi"))
     ScriptWriter.write_script("test.sh", lambda f: f.write("echo hi"), executable=True)
```

### Comparing `pyXhUtils-1.0.0/src/xh_utils_string/StringUtils.py` & `pyXhUtils-1.0.1/src/xh_utils_string/StringUtils.py`

 * *Files identical despite different names*

