# Comparing `tmp/ats_case-0.5.1.tar.gz` & `tmp/ats_case-0.5.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "ats_case-0.5.1.tar", last modified: Fri Apr 21 02:34:27 2023, max compression
+gzip compressed data, was "ats_case-0.5.2.tar", last modified: Fri Apr 21 03:49:32 2023, max compression
```

## Comparing `ats_case-0.5.1.tar` & `ats_case-0.5.2.tar`

### file list

```diff
@@ -1,32 +1,32 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.673812 ats_case-0.5.1/
--rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.1/LICENSE
--rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.1/MANIFEST.in
--rw-rw-rw-   0        0        0     1042 2023-04-21 02:34:27.670816 ats_case-0.5.1/PKG-INFO
--rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.1/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.263903 ats_case-0.5.1/ats_case/
--rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.1/ats_case/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.475340 ats_case-0.5.1/ats_case/case/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.1/ats_case/case/__init__.py
--rw-rw-rw-   0        0        0    17435 2023-04-20 09:51:30.000000 ats_case-0.5.1/ats_case/case/command.py
--rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.1/ats_case/case/context.py
--rw-rw-rw-   0        0        0     6444 2023-04-20 08:35:14.000000 ats_case-0.5.1/ats_case/case/executor.py
--rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.1/ats_case/case/translator.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.562106 ats_case-0.5.1/ats_case/common/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.1/ats_case/common/__init__.py
--rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.1/ats_case/common/enum.py
--rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.1/ats_case/common/error.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.629924 ats_case-0.5.1/ats_case/manage/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.1/ats_case/manage/__init__.py
--rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.1/ats_case/manage/core.py
--rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.1/ats_case/manage/start.py
-drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.659844 ats_case-0.5.1/ats_case/template/
--rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.1/ats_case/template/__init__.py
--rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.1/ats_case/template/testcase_v1.tmp
-drwxrwxrwx   0        0        0        0 2023-04-21 02:34:27.349674 ats_case-0.5.1/ats_case.egg-info/
--rw-rw-rw-   0        0        0     1042 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      566 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       39 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/requires.txt
--rw-rw-rw-   0        0        0        9 2023-04-21 02:34:26.000000 ats_case-0.5.1/ats_case.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 02:34:27.674805 ats_case-0.5.1/setup.cfg
--rw-rw-rw-   0        0        0      935 2023-04-21 02:34:20.000000 ats_case-0.5.1/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:49:32.153328 ats_case-0.5.2/
+-rw-rw-rw-   0        0        0      116 2022-09-15 08:18:29.000000 ats_case-0.5.2/LICENSE
+-rw-rw-rw-   0        0        0        0 2023-03-03 08:23:26.000000 ats_case-0.5.2/MANIFEST.in
+-rw-rw-rw-   0        0        0     1042 2023-04-21 03:49:32.151336 ats_case-0.5.2/PKG-INFO
+-rw-rw-rw-   0        0        0      532 2022-06-13 07:56:24.000000 ats_case-0.5.2/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 03:49:31.782241 ats_case-0.5.2/ats_case/
+-rw-rw-rw-   0        0        0        0 2023-01-04 02:21:31.000000 ats_case-0.5.2/ats_case/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:49:31.985736 ats_case-0.5.2/ats_case/case/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:13:48.000000 ats_case-0.5.2/ats_case/case/__init__.py
+-rw-rw-rw-   0        0        0    17423 2023-04-21 02:50:28.000000 ats_case-0.5.2/ats_case/case/command.py
+-rw-rw-rw-   0        0        0     9683 2023-04-20 08:35:14.000000 ats_case-0.5.2/ats_case/case/context.py
+-rw-rw-rw-   0        0        0     6309 2023-04-21 03:45:03.000000 ats_case-0.5.2/ats_case/case/executor.py
+-rw-rw-rw-   0        0        0     5593 2023-04-21 02:33:28.000000 ats_case-0.5.2/ats_case/case/translator.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:49:32.046576 ats_case-0.5.2/ats_case/common/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:22:45.000000 ats_case-0.5.2/ats_case/common/__init__.py
+-rw-rw-rw-   0        0        0      441 2023-04-20 06:40:34.000000 ats_case-0.5.2/ats_case/common/enum.py
+-rw-rw-rw-   0        0        0      640 2023-04-20 02:04:10.000000 ats_case-0.5.2/ats_case/common/error.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:49:32.102724 ats_case-0.5.2/ats_case/manage/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.2/ats_case/manage/__init__.py
+-rw-rw-rw-   0        0        0     1434 2023-03-03 01:15:16.000000 ats_case-0.5.2/ats_case/manage/core.py
+-rw-rw-rw-   0        0        0     2953 2023-04-20 07:40:35.000000 ats_case-0.5.2/ats_case/manage/start.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:49:32.136602 ats_case-0.5.2/ats_case/template/
+-rw-rw-rw-   0        0        0        0 2023-02-07 07:20:58.000000 ats_case-0.5.2/ats_case/template/__init__.py
+-rw-rw-rw-   0        0        0     2067 2023-04-20 00:58:29.000000 ats_case-0.5.2/ats_case/template/testcase_v1.tmp
+drwxrwxrwx   0        0        0        0 2023-04-21 03:49:31.877987 ats_case-0.5.2/ats_case.egg-info/
+-rw-rw-rw-   0        0        0     1042 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      566 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       39 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        9 2023-04-21 03:49:31.000000 ats_case-0.5.2/ats_case.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 03:49:32.153328 ats_case-0.5.2/setup.cfg
+-rw-rw-rw-   0        0        0      935 2023-04-21 03:42:31.000000 ats_case-0.5.2/setup.py
```

### Comparing `ats_case-0.5.1/PKG-INFO` & `ats_case-0.5.2/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats_case
-Version: 0.5.1
+Version: 0.5.2
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.1/README.md` & `ats_case-0.5.2/README.md`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.1/ats_case/case/command.py` & `ats_case-0.5.2/ats_case/case/command.py`

 * *Files 0% similar despite different names*

```diff
@@ -139,16 +139,15 @@
     :param param: desc-测试步骤描述
     :return:
     """
     desc = param.get('desc')
 
     def decorate(callback):
         def fn(*args, **kwargs):
-            client().message(desc).show(args[0])
-            # send(args[0], todo={'app:show': {'msg': desc}})
+            client().message(desc).show(args[0])  # send(args[0], todo={'app:show': {'msg': desc}})
             r = callback(*args, **kwargs)
             return r
         
         return fn
 
     return decorate
```

### Comparing `ats_case-0.5.1/ats_case/case/context.py` & `ats_case-0.5.2/ats_case/case/context.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.1/ats_case/case/executor.py` & `ats_case-0.5.2/ats_case/case/executor.py`

 * *Files 5% similar despite different names*

```diff
@@ -32,75 +32,67 @@
         raise AssertionError(str(e))
 
 
 class Executor(object):
     def __init__(self, context: Context):
         self._context = context
         self._model = None
+        self._steps = []
 
     def exec(self):
-        steps = self.handle()
+        self.handle()
 
         index = 0
-        while index < len(steps):
-            self._context.runtime.step = steps[index]
+        while index < len(self._steps):
+            self._context.runtime.step = self._steps[index]
             if self.loop_meet():
                 self.loop_exec()
             else:
                 self.step_exec()
 
-            if self._context.runtime.step > (index + 1):
-                index = self._context.runtime.step
-            else:
-                index += 1
+            index = self._steps.index(self._context.runtime.step) + 1
 
     def handle(self):
-        return []
+        pass
 
     def is_exec(self):
         ifs = self._context.case.control.get('ifs')
         if ifs is not None and type(ifs) is dict and len(ifs) > 0:
-            for func, values in ifs.items():
-                if command.ats().operation(func).parameter(values).exec(self._context):
+            for fc, values in ifs.items():
+                if command.ats().operation(fc).parameter(values).exec(self._context):
                     return False
         return True
 
     def step_exec(self):
-        try:
-            logger.info('~ @TCC-STEP-> steps[#{}] execute'.format(self._context.runtime.step))
+        logger.info('~ @TCC-STEP-> steps[#{}] execute'.format(self._context.runtime.step))
 
-            if self.is_exec():
-                getattr(self._model, 'step_{}'.format(self._context.runtime.step))(self._context)
-        except Exception as e:
-            raise Exception(str(e))
+        if self.is_exec():
+            getattr(self._model, 'step_{}'.format(self._context.runtime.step))(self._context)
 
     def loop_meet(self):
-        try:
-            loops = self._context.case.control.get('loops')
+        loops = self._context.case.control.get('loops')
 
-            if loops is None or type(loops) is not list or len(loops) <= 0:
-                return False
+        if loops is None or type(loops) is not list or len(loops) <= 0:
+            return False
 
-            if self._context.runtime.loop_sn >= len(loops):
-                return False
-            loop = loops[self._context.runtime.loop_sn]
-            ranges = loop.get('range')
-            count = loop.get('count')
-
-            step_start = int(ranges.split(':')[0])
-            step_end = int(ranges.split(':')[1])
-
-            if step_start <= self._context.runtime.step <= step_end:
-                self._context.runtime.loop_start_step = step_start
-                self._context.runtime.loop_end_step = step_end
-                self._context.runtime.loop_count = int(count)
-                self._context.runtime.loop_index = 0
-                return True
-        except Exception as e:
-            raise Exception(str(e))
+        if self._context.runtime.loop_sn >= len(loops):
+            return False
+        loop = loops[self._context.runtime.loop_sn]
+        ranges = loop.get('range')
+        count = loop.get('count')
+
+        step_start = int(ranges.split(':')[0])
+        step_end = int(ranges.split(':')[1])
+
+        if step_start <= self._context.runtime.step <= step_end:
+            self._context.runtime.loop_start_step = step_start
+            self._context.runtime.loop_end_step = step_end
+            self._context.runtime.loop_count = int(count)
+            self._context.runtime.loop_index = 0
+            return True
 
         return False
 
     def loop_exec(self):
         logger.info('~ @TCC-LOOP-> loops[#{}] start. -range {}:{}  -count {}'.format(
             self._context.runtime.loop_sn, self._context.runtime.loop_start_step,
             self._context.runtime.loop_end_step, self._context.runtime.loop_count))
@@ -116,53 +108,54 @@
             logger.info('~ @TCC-LOOP-> loops[#{}], -count {}, -index {}'.format(
                 self._context.runtime.loop_sn, self._context.runtime.loop_count,
                 self._context.runtime.loop_index))
             command.client().message('循环[#{}], 共{}次, 当前第{}次'.format(
                 self._context.runtime.loop_sn, self._context.runtime.loop_count,
                 self._context.runtime.loop_index)).show(self._context)
 
-            for j in range(self._context.runtime.loop_start_step, self._context.runtime.loop_end_step + 1):
-                self._context.runtime.step = j
-                self.step_exec()
+            for step in range(self._context.runtime.loop_start_step, self._context.runtime.loop_end_step + 1):
+                index = None
+                try:
+                    index = self._steps.index(step)
+                except ValueError as e:
+                    pass
+
+                if index is not None:
+                    self._context.runtime.step = step
+                    self.step_exec()
 
         command.client().message("循环结束...").show(self._context)
         logger.info('~ @TCC-LOOP-> loops[#{}] end.'.format(self._context.runtime.loop_sn))
         self._context.runtime.loop_sn += 1
 
 
 def extract_steps(content: list):
     n_s = []
     for s in content:
         if s.upper().find('STEP_') >= 0:
             num = func.extract_digit(s)
             n_s.append(int(num))
 
-    sorted_n_s = sorted(n_s)
-
-    return sorted_n_s
+    return sorted(n_s)
 
 
 class FormalExecutor(Executor):
     def handle(self):
-        # 分为两种情况: 1. 手动编写脚本 2.自动编写脚本
+        # 分为两种情况: 0. 手动编写脚本 1.自动编写脚本
         if self._context.case.script == ScriptClazz.AUTO:
-            steps = translator.translate(self._context)
+            self._steps = translator.translate(self._context)
             self._model = import_module('script.auto.{}.tsm_{}'.format(self._context.tester.username.lower()
                                                                        , self._context.meter.pos))
         else:
             self._model = import_module('script.manual.formal.{}'.format(self._context.case.steps))
-            steps = extract_steps(dir(self._model))
-
-        return steps
+            self._steps = extract_steps(dir(self._model))
 
 
 class DebugExecutor(Executor):
     def handle(self):
         if self._context.case.script == ScriptClazz.AUTO:
-            steps = translator.translate(self._context)
+            self._steps = translator.translate(self._context)
             self._model = import_module('script.auto.{}.tsm_{}'.format(self._context.tester.username.lower()
                                                                        , self._context.meter.pos))
         else:
             self._model = import_module('script.manual.debug.{}'.format(self._context.case.steps))
-            steps = extract_steps(dir(self._model))
-
-        return steps
+            self._steps = extract_steps(dir(self._model))
```

### Comparing `ats_case-0.5.1/ats_case/case/translator.py` & `ats_case-0.5.2/ats_case/case/translator.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.1/ats_case/common/error.py` & `ats_case-0.5.2/ats_case/common/error.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.1/ats_case/manage/core.py` & `ats_case-0.5.2/ats_case/manage/core.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.1/ats_case/manage/start.py` & `ats_case-0.5.2/ats_case/manage/start.py`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.1/ats_case/template/testcase_v1.tmp` & `ats_case-0.5.2/ats_case/template/testcase_v1.tmp`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.1/ats_case.egg-info/PKG-INFO` & `ats_case-0.5.2/ats_case.egg-info/PKG-INFO`

 * *Files 11% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: ats-case
-Version: 0.5.1
+Version: 0.5.2
 Summary: Test Script Development Library
 Home-page: https://gitee.com/henry9000/ats_case
 Author: zhangyue
 Author-email: zhangyue@techen.cn
 Project-URL: Bug Tracker, https://gitee.com/henry9000/ats_case/issues
 Classifier: Programming Language :: Python :: 3
 Classifier: License :: OSI Approved :: MIT License
```

### Comparing `ats_case-0.5.1/ats_case.egg-info/SOURCES.txt` & `ats_case-0.5.2/ats_case.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `ats_case-0.5.1/setup.py` & `ats_case-0.5.2/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 import setuptools
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setuptools.setup(
     name="ats_case",
-    version="0.5.1",
+    version="0.5.2",
     py_modules=['ats_case'],
     author="zhangyue",
     author_email="zhangyue@techen.cn",
     description="Test Script Development Library",
     long_description=long_description,
     long_description_content_type="text/markdown",
     url="https://gitee.com/henry9000/ats_case",
```

