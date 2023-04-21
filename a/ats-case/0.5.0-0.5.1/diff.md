# Comparing `tmp/ats_case-0.5.0.tar.gz` & `tmp/ats_case-0.5.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.5.0.tar", last modified: Thu Apr 20 08:36:57 2023, max compression
+gzip compressed data, was "ats_case-0.5.1.tar", last modified: Fri Apr 21 02:34:27 2023, max compression
```

## Comparing `ats_case-0.5.0.tar` & `ats_case-0.5.1.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.648786 ats_case-0.5.0/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.0/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.0/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-20 08:36:57.644797 ats_case-0.5.0/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.111681 ats_case-0.5.0/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.0/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.344051 ats_case-0.5.0/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.0/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17372 2023-04-20 03:36:42.000000 ats_case-0.5.0/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.0/ats_case/case/context.py
--rw-rw-rw-   0        0        0     6444 2023-04-20 08:35:14.000000 ats_case-0.5.0/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5591 2023-04-20 08:34:36.000000 ats_case-0.5.0/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.423838 ats_case-0.5.0/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.0/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.0/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.0/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.539533 ats_case-0.5.0/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.0/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.0/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.0/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.588949 ats_case-0.5.0/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.0/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.0/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-20 08:36:57.212926 ats_case-0.5.0/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-20 08:36:56.000000 ats_case-0.5.0/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-20 08:36:57.648786 ats_case-0.5.0/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-20 05:29:46.000000 ats_case-0.5.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.673812 ats_case-0.5.1/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.1/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.1/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-21 02:34:27.670816 ats_case-0.5.1/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.263903 ats_case-0.5.1/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.1/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.475340 ats_case-0.5.1/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.1/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17435 2023-04-20 09:51:30.000000 ats_case-0.5.1/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.1/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     6444 2023-04-20 08:35:14.000000 ats_case-0.5.1/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.1/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.562106 ats_case-0.5.1/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.1/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.1/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.1/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.629924 ats_case-0.5.1/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.1/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.1/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.1/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.659844 ats_case-0.5.1/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.1/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.1/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.349674 ats_case-0.5.1/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 02:34:27.674805 ats_case-0.5.1/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-21 02:34:20.000000 ats_case-0.5.1/setup.py
```

### Comparing `ats_case-0.5.0/PKG-INFO` & `ats_case-0.5.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.5.0
+Version: 0.5.1
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.0/README.md` & `ats_case-0.5.1/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.0/ats_case/case/command.py` & `ats_case-0.5.1/ats_case/case/command.py`

 * *Files 1% similar despite different names*

```diff
@@ -140,14 +140,15 @@
     :return:
     """
     desc = param.get('desc')
 
     def decorate(callback):
         def fn(*args, **kwargs):
             client().message(desc).show(args[0])
+            # send(args[0], todo={'app:show': {'msg': desc}})
             r = callback(*args, **kwargs)
             return r
         
         return fn
 
     return decorate
```

### Comparing `ats_case-0.5.0/ats_case/case/context.py` & `ats_case-0.5.1/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.0/ats_case/case/executor.py` & `ats_case-0.5.1/ats_case/case/executor.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.0/ats_case/case/translator.py` & `ats_case-0.5.1/ats_case/case/translator.py`

 * *Files 0% similar despite different names*

```diff
@@ -47,15 +47,15 @@
 
         return script_file
 
     def _gen_import(self):
         return 'from ats_case.case import command' + self.LINE + 'from ats_case.case.context import Context' + self.LINE
 
     def _gen_step(self, step: int, op: dict):
-        return '@command.step_annotation(desc={}){}'.format(op.get('desc', ''), self.LINE) + \
+        return '@command.step_annotation(desc={}){}'.format(op.get('desc', '""'), self.LINE) + \
                'def step_{}(context: Context):{}'.format(step, self.LINE)
 
     def _gen_tab(self, count: int):
         ts = ''
         for i in range(count):
             ts += self.TAB
```

### Comparing `ats_case-0.5.0/ats_case/common/error.py` & `ats_case-0.5.1/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.0/ats_case/manage/core.py` & `ats_case-0.5.1/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.0/ats_case/manage/start.py` & `ats_case-0.5.1/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.0/ats_case/template/testcase_v1.tmp` & `ats_case-0.5.1/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.0/ats_case.egg-info/PKG-INFO` & `ats_case-0.5.1/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.5.0
+Version: 0.5.1
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.0/ats_case.egg-info/SOURCES.txt` & `ats_case-0.5.1/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.0/setup.py` & `ats_case-0.5.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.5.0",
+    version="0.5.1",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

