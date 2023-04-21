# Comparing `tmp/cloudpss-3.2.0a1.tar.gz` & `tmp/cloudpss-3.2.0a2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\cloudpss-3.2.0a1.tar", last modified: Mon Aug  1 05:02:42 2022, max compression
+gzip compressed data, was "dist\cloudpss-3.2.0a2.tar", last modified: Mon Aug  1 08:13:49 2022, max compression
```

## Comparing `cloudpss-3.2.0a1.tar` & `cloudpss-3.2.0a2.tar`

### file list

```diff
@@ -1,47 +1,47 @@
-drwxrwxrwx   0        0        0        0 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/
--rw-rw-rw-   0        0        0     2364 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/PKG-INFO
--rw-rw-rw-   0        0        0     1760 2022-08-01 03:22:41.000000 cloudpss-3.2.0a1/README.md
-drwxrwxrwx   0        0        0        0 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss/
--rw-rw-rw-   0        0        0      669 2022-08-01 05:02:23.000000 cloudpss-3.2.0a1/cloudpss/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss/function/
--rw-rw-rw-   0        0        0     1386 2022-07-31 14:18:50.000000 cloudpss-3.2.0a1/cloudpss/function/__init__.py
--rw-rw-rw-   0        0        0       29 2022-01-20 05:13:06.000000 cloudpss-3.2.0a1/cloudpss/function/function.py
--rw-rw-rw-   0        0        0    14737 2022-08-01 04:53:29.000000 cloudpss-3.2.0a1/cloudpss/function/functionExecution.py
--rw-rw-rw-   0        0        0    13162 2022-07-31 12:40:10.000000 cloudpss-3.2.0a1/cloudpss/function/job.py
-drwxrwxrwx   0        0        0        0 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss/model/
--rw-rw-rw-   0        0        0      151 2021-12-29 02:28:37.000000 cloudpss-3.2.0a1/cloudpss/model/__init__.py
-drwxrwxrwx   0        0        0        0 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss/model/implements/
--rw-rw-rw-   0        0        0       67 2021-12-29 06:40:28.000000 cloudpss-3.2.0a1/cloudpss/model/implements/__init__.py
--rw-rw-rw-   0        0        0      734 2021-12-24 02:31:09.000000 cloudpss-3.2.0a1/cloudpss/model/implements/component.py
--rw-rw-rw-   0        0        0     1063 2021-12-24 02:31:09.000000 cloudpss-3.2.0a1/cloudpss/model/implements/diagram.py
--rw-rw-rw-   0        0        0      954 2021-12-29 06:40:28.000000 cloudpss-3.2.0a1/cloudpss/model/implements/implement.py
--rw-rw-rw-   0        0        0     2755 2021-12-29 06:40:28.000000 cloudpss-3.2.0a1/cloudpss/model/jobDefinitions.py
--rw-rw-rw-   0        0        0    16144 2022-01-19 08:08:22.000000 cloudpss-3.2.0a1/cloudpss/model/model.py
--rw-rw-rw-   0        0        0     3682 2021-12-29 11:23:01.000000 cloudpss-3.2.0a1/cloudpss/model/revision.py
--rw-rw-rw-   0        0        0     2234 2021-12-29 11:22:22.000000 cloudpss-3.2.0a1/cloudpss/model/topology.py
-drwxrwxrwx   0        0        0        0 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss/project/
--rw-rw-rw-   0        0        0       51 2022-01-06 03:40:26.000000 cloudpss-3.2.0a1/cloudpss/project/__init__.py
--rw-rw-rw-   0        0        0    17721 2022-01-19 08:08:20.000000 cloudpss-3.2.0a1/cloudpss/project/project.py
-drwxrwxrwx   0        0        0        0 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss/runner/
--rw-rw-rw-   0        0        0      241 2021-08-18 04:07:17.000000 cloudpss-3.2.0a1/cloudpss/runner/__init__.py
--rw-rw-rw-   0        0        0     4073 2022-04-07 06:45:11.000000 cloudpss-3.2.0a1/cloudpss/runner/receiver.py
--rw-rw-rw-   0        0        0    11495 2022-01-05 08:46:05.000000 cloudpss-3.2.0a1/cloudpss/runner/result.py
--rw-rw-rw-   0        0        0     3434 2022-08-01 04:58:40.000000 cloudpss-3.2.0a1/cloudpss/runner/runner.py
--rw-rw-rw-   0        0        0     4162 2021-12-29 06:40:28.000000 cloudpss-3.2.0a1/cloudpss/runner/storage.py
--rw-rw-rw-   0        0        0    11613 2021-08-16 11:17:24.000000 cloudpss-3.2.0a1/cloudpss/runner/transform.py
-drwxrwxrwx   0        0        0        0 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss/utils/
--rw-rw-rw-   0        0        0      291 2021-12-24 02:31:13.000000 cloudpss-3.2.0a1/cloudpss/utils/__init__.py
--rw-rw-rw-   0        0        0      885 2021-12-24 03:16:00.000000 cloudpss-3.2.0a1/cloudpss/utils/dataEncoder.py
--rw-rw-rw-   0        0        0      255 2022-01-06 03:40:44.000000 cloudpss-3.2.0a1/cloudpss/utils/graphqlUtil.py
--rw-rw-rw-   0        0        0     1321 2022-01-06 04:32:27.000000 cloudpss-3.2.0a1/cloudpss/utils/httprequests.py
--rw-rw-rw-   0        0        0      795 2021-08-13 08:49:11.000000 cloudpss-3.2.0a1/cloudpss/utils/matlab.py
--rw-rw-rw-   0        0        0     2885 2021-12-24 03:16:00.000000 cloudpss-3.2.0a1/cloudpss/utils/yamlLoader.py
--rw-rw-rw-   0        0        0      810 2021-12-24 03:16:24.000000 cloudpss-3.2.0a1/cloudpss/verify.py
-drwxrwxrwx   0        0        0        0 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss.egg-info/
--rw-rw-rw-   0        0        0     2364 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0     1025 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       96 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/cloudpss.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-08-01 05:02:42.000000 cloudpss-3.2.0a1/setup.cfg
--rw-rw-rw-   0        0        0      801 2022-01-06 04:37:02.000000 cloudpss-3.2.0a1/setup.py
+drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/
+-rw-rw-rw-   0        0        0     2364 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/PKG-INFO
+-rw-rw-rw-   0        0        0     1760 2022-08-01 03:22:41.000000 cloudpss-3.2.0a2/README.md
+drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/
+-rw-rw-rw-   0        0        0      669 2022-08-01 08:13:05.000000 cloudpss-3.2.0a2/cloudpss/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/function/
+-rw-rw-rw-   0        0        0     1629 2022-08-01 08:12:21.000000 cloudpss-3.2.0a2/cloudpss/function/__init__.py
+-rw-rw-rw-   0        0        0       29 2022-01-20 05:13:06.000000 cloudpss-3.2.0a2/cloudpss/function/function.py
+-rw-rw-rw-   0        0        0    14737 2022-08-01 04:53:29.000000 cloudpss-3.2.0a2/cloudpss/function/functionExecution.py
+-rw-rw-rw-   0        0        0    13162 2022-07-31 12:40:10.000000 cloudpss-3.2.0a2/cloudpss/function/job.py
+drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/model/
+-rw-rw-rw-   0        0        0      151 2021-12-29 02:28:37.000000 cloudpss-3.2.0a2/cloudpss/model/__init__.py
+drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/model/implements/
+-rw-rw-rw-   0        0        0       67 2021-12-29 06:40:28.000000 cloudpss-3.2.0a2/cloudpss/model/implements/__init__.py
+-rw-rw-rw-   0        0        0      734 2021-12-24 02:31:09.000000 cloudpss-3.2.0a2/cloudpss/model/implements/component.py
+-rw-rw-rw-   0        0        0     1063 2021-12-24 02:31:09.000000 cloudpss-3.2.0a2/cloudpss/model/implements/diagram.py
+-rw-rw-rw-   0        0        0      954 2021-12-29 06:40:28.000000 cloudpss-3.2.0a2/cloudpss/model/implements/implement.py
+-rw-rw-rw-   0        0        0     2755 2021-12-29 06:40:28.000000 cloudpss-3.2.0a2/cloudpss/model/jobDefinitions.py
+-rw-rw-rw-   0        0        0    16144 2022-01-19 08:08:22.000000 cloudpss-3.2.0a2/cloudpss/model/model.py
+-rw-rw-rw-   0        0        0     3682 2021-12-29 11:23:01.000000 cloudpss-3.2.0a2/cloudpss/model/revision.py
+-rw-rw-rw-   0        0        0     2234 2021-12-29 11:22:22.000000 cloudpss-3.2.0a2/cloudpss/model/topology.py
+drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/project/
+-rw-rw-rw-   0        0        0       51 2022-01-06 03:40:26.000000 cloudpss-3.2.0a2/cloudpss/project/__init__.py
+-rw-rw-rw-   0        0        0    17721 2022-01-19 08:08:20.000000 cloudpss-3.2.0a2/cloudpss/project/project.py
+drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/runner/
+-rw-rw-rw-   0        0        0      241 2021-08-18 04:07:17.000000 cloudpss-3.2.0a2/cloudpss/runner/__init__.py
+-rw-rw-rw-   0        0        0     4073 2022-04-07 06:45:11.000000 cloudpss-3.2.0a2/cloudpss/runner/receiver.py
+-rw-rw-rw-   0        0        0    11495 2022-01-05 08:46:05.000000 cloudpss-3.2.0a2/cloudpss/runner/result.py
+-rw-rw-rw-   0        0        0     3434 2022-08-01 04:58:40.000000 cloudpss-3.2.0a2/cloudpss/runner/runner.py
+-rw-rw-rw-   0        0        0     4162 2021-12-29 06:40:28.000000 cloudpss-3.2.0a2/cloudpss/runner/storage.py
+-rw-rw-rw-   0        0        0    11613 2021-08-16 11:17:24.000000 cloudpss-3.2.0a2/cloudpss/runner/transform.py
+drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss/utils/
+-rw-rw-rw-   0        0        0      291 2021-12-24 02:31:13.000000 cloudpss-3.2.0a2/cloudpss/utils/__init__.py
+-rw-rw-rw-   0        0        0      885 2021-12-24 03:16:00.000000 cloudpss-3.2.0a2/cloudpss/utils/dataEncoder.py
+-rw-rw-rw-   0        0        0      255 2022-01-06 03:40:44.000000 cloudpss-3.2.0a2/cloudpss/utils/graphqlUtil.py
+-rw-rw-rw-   0        0        0     1321 2022-01-06 04:32:27.000000 cloudpss-3.2.0a2/cloudpss/utils/httprequests.py
+-rw-rw-rw-   0        0        0      795 2021-08-13 08:49:11.000000 cloudpss-3.2.0a2/cloudpss/utils/matlab.py
+-rw-rw-rw-   0        0        0     2885 2021-12-24 03:16:00.000000 cloudpss-3.2.0a2/cloudpss/utils/yamlLoader.py
+-rw-rw-rw-   0        0        0      810 2021-12-24 03:16:24.000000 cloudpss-3.2.0a2/cloudpss/verify.py
+drwxrwxrwx   0        0        0        0 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/cloudpss.egg-info/
+-rw-rw-rw-   0        0        0     2364 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0     1025 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       96 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2022-08-01 08:13:47.000000 cloudpss-3.2.0a2/cloudpss.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2022-08-01 08:13:49.000000 cloudpss-3.2.0a2/setup.cfg
+-rw-rw-rw-   0        0        0      801 2022-01-06 04:37:02.000000 cloudpss-3.2.0a2/setup.py
```

### Comparing `cloudpss-3.2.0a1/PKG-INFO` & `cloudpss-3.2.0a2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpss
-Version: 3.2.0a1
+Version: 3.2.0a2
 Summary: cloudpss sdk
 Home-page: https://www.cloudpss.net
 Author: cloudpss
 Author-email: zhangdaming@cloudpss.net
 License: MIT Licence
 Description: 
         CloudPSS SDK
```

### Comparing `cloudpss-3.2.0a1/README.md` & `cloudpss-3.2.0a2/README.md`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/__init__.py` & `cloudpss-3.2.0a2/cloudpss/__init__.py`

 * *Files 1% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 from .function import FunctionExecution
 
 __all__ = [
     'setToken', 'Model', 'ModelRevision', 'ModelTopology', 'Runner', 'Result',
     'PowerFlowResult', 'EMTResult', 'MatlabDataEncoder', 'DateTimeEncode',
     'function', 'Project', 'currentJob'
 ]
-__version__ = '3.2.0.alpha.1'
+__version__ = '3.2.0.alpha.2'
 
 
 def currentJob():
     """
         获取当前的 currentExecution 实例
     """
     return FunctionExecution.current()
```

### Comparing `cloudpss-3.2.0a1/cloudpss/function/__init__.py` & `cloudpss-3.2.0a2/cloudpss/function/__init__.py`

 * *Files 15% similar despite different names*

```diff
@@ -13,15 +13,19 @@
 
 
 @deprecated(
     version='3.0',
     reason="该类将在 5.0 版本移除，请使用 cloudpss.currentJob() 方法代替",
 )
 def currentJob():
-    return Job.current()
+    job = Job.current()
+    job.message(
+        "DeprecationWarning: Call to deprecated function (or staticmethod) cloudpss.function.currentJob(). (该类将在 5.0 版本移除，请使用 cloudpss.currentJob() 方法代替",
+        level='warning')
+    return job
     pass
 
 
 def currentExecutor():
     """
         获取表示当前执行的 FunctionExecution 单例
     """
```

### Comparing `cloudpss-3.2.0a1/cloudpss/function/functionExecution.py` & `cloudpss-3.2.0a2/cloudpss/function/functionExecution.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/function/job.py` & `cloudpss-3.2.0a2/cloudpss/function/job.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/model/implements/component.py` & `cloudpss-3.2.0a2/cloudpss/model/implements/component.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/model/implements/diagram.py` & `cloudpss-3.2.0a2/cloudpss/model/implements/diagram.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/model/implements/implement.py` & `cloudpss-3.2.0a2/cloudpss/model/implements/implement.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/model/jobDefinitions.py` & `cloudpss-3.2.0a2/cloudpss/model/jobDefinitions.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/model/model.py` & `cloudpss-3.2.0a2/cloudpss/model/model.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/model/revision.py` & `cloudpss-3.2.0a2/cloudpss/model/revision.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/model/topology.py` & `cloudpss-3.2.0a2/cloudpss/model/topology.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/project/project.py` & `cloudpss-3.2.0a2/cloudpss/project/project.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/runner/receiver.py` & `cloudpss-3.2.0a2/cloudpss/runner/receiver.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/runner/result.py` & `cloudpss-3.2.0a2/cloudpss/runner/result.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/runner/runner.py` & `cloudpss-3.2.0a2/cloudpss/runner/runner.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/runner/storage.py` & `cloudpss-3.2.0a2/cloudpss/runner/storage.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/runner/transform.py` & `cloudpss-3.2.0a2/cloudpss/runner/transform.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/utils/dataEncoder.py` & `cloudpss-3.2.0a2/cloudpss/utils/dataEncoder.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/utils/httprequests.py` & `cloudpss-3.2.0a2/cloudpss/utils/httprequests.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/utils/matlab.py` & `cloudpss-3.2.0a2/cloudpss/utils/matlab.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/utils/yamlLoader.py` & `cloudpss-3.2.0a2/cloudpss/utils/yamlLoader.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss/verify.py` & `cloudpss-3.2.0a2/cloudpss/verify.py`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/cloudpss.egg-info/PKG-INFO` & `cloudpss-3.2.0a2/cloudpss.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cloudpss
-Version: 3.2.0a1
+Version: 3.2.0a2
 Summary: cloudpss sdk
 Home-page: https://www.cloudpss.net
 Author: cloudpss
 Author-email: zhangdaming@cloudpss.net
 License: MIT Licence
 Description: 
         CloudPSS SDK
```

### Comparing `cloudpss-3.2.0a1/cloudpss.egg-info/SOURCES.txt` & `cloudpss-3.2.0a2/cloudpss.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `cloudpss-3.2.0a1/setup.py` & `cloudpss-3.2.0a2/setup.py`

 * *Files identical despite different names*

