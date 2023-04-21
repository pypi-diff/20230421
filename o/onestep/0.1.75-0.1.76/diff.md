# Comparing `tmp/onestep-0.1.75.tar.gz` & `tmp/onestep-0.1.76.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "onestep-0.1.75.tar", max compression
+gzip compressed data, was "onestep-0.1.76.tar", max compression
```

## Comparing `onestep-0.1.75.tar` & `onestep-0.1.76.tar`

### file list

```diff
@@ -1,22 +1,22 @@
--rw-r--r--   0        0        0     1362 2023-04-11 09:07:40.588934 onestep-0.1.75/README.md
--rw-r--r--   0        0        0      704 2023-04-11 09:07:40.588934 onestep-0.1.75/pyproject.toml
--rw-r--r--   0        0        0     1374 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/__init__.py
--rw-r--r--   0        0        0      221 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/broker/__init__.py
--rw-r--r--   0        0        0     4310 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/broker/base.py
--rw-r--r--   0        0        0      957 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/broker/cron.py
--rw-r--r--   0        0        0      151 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/broker/memory.py
--rw-r--r--   0        0        0     1997 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/broker/rabbitmq.py
--rw-r--r--   0        0        0     2144 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/broker/webhook.py
--rw-r--r--   0        0        0      610 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/exception.py
--rw-r--r--   0        0        0     4005 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/message.py
--rw-r--r--   0        0        0      286 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/middleware/__init__.py
--rw-r--r--   0        0        0      521 2023-04-11 09:07:40.588934 onestep-0.1.75/src/onestep/middleware/base.py
--rw-r--r--   0        0        0     2438 2023-04-11 09:07:40.592934 onestep-0.1.75/src/onestep/middleware/config.py
--rw-r--r--   0        0        0     6350 2023-04-11 09:07:40.592934 onestep-0.1.75/src/onestep/onestep.py
--rw-r--r--   0        0        0     2699 2023-04-11 09:07:40.592934 onestep-0.1.75/src/onestep/retry.py
--rw-r--r--   0        0        0      293 2023-04-11 09:07:40.592934 onestep-0.1.75/src/onestep/signal.py
--rw-r--r--   0        0        0      618 2023-04-11 09:07:40.592934 onestep-0.1.75/src/onestep/state.py
--rw-r--r--   0        0        0       36 2023-04-11 09:07:40.592934 onestep-0.1.75/src/onestep/store/__init__.py
--rw-r--r--   0        0        0     4170 2023-04-11 09:07:40.592934 onestep-0.1.75/src/onestep/store/rabbitmq.py
--rw-r--r--   0        0        0     3517 2023-04-11 09:07:40.592934 onestep-0.1.75/src/onestep/worker.py
--rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.75/PKG-INFO
+-rw-r--r--   0        0        0     1362 2023-04-21 01:22:59.195390 onestep-0.1.76/README.md
+-rw-r--r--   0        0        0      704 2023-04-21 01:22:59.195390 onestep-0.1.76/pyproject.toml
+-rw-r--r--   0        0        0     1374 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/__init__.py
+-rw-r--r--   0        0        0      221 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/__init__.py
+-rw-r--r--   0        0        0     4310 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/base.py
+-rw-r--r--   0        0        0      957 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/cron.py
+-rw-r--r--   0        0        0      151 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/memory.py
+-rw-r--r--   0        0        0     1997 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/rabbitmq.py
+-rw-r--r--   0        0        0     2144 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/broker/webhook.py
+-rw-r--r--   0        0        0      610 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/exception.py
+-rw-r--r--   0        0        0     4338 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/message.py
+-rw-r--r--   0        0        0      286 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/middleware/__init__.py
+-rw-r--r--   0        0        0      521 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/middleware/base.py
+-rw-r--r--   0        0        0     2438 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/middleware/config.py
+-rw-r--r--   0        0        0     6350 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/onestep.py
+-rw-r--r--   0        0        0     2699 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/retry.py
+-rw-r--r--   0        0        0      293 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/signal.py
+-rw-r--r--   0        0        0      618 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/state.py
+-rw-r--r--   0        0        0       36 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/store/__init__.py
+-rw-r--r--   0        0        0     4170 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/store/rabbitmq.py
+-rw-r--r--   0        0        0     3516 2023-04-21 01:22:59.199390 onestep-0.1.76/src/onestep/worker.py
+-rw-r--r--   0        0        0     1993 1970-01-01 00:00:00.000000 onestep-0.1.76/PKG-INFO
```

### Comparing `onestep-0.1.75/README.md` & `onestep-0.1.76/README.md`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/pyproject.toml` & `onestep-0.1.76/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "onestep"
-version = "0.1.75"
+version = "0.1.76"
 description = ""
 authors = ["miclon <jcnd@163.com>"]
 readme = "README.md"
 packages = [
     { include = 'onestep', from = 'src' }
 ]
```

### Comparing `onestep-0.1.75/src/onestep/__init__.py` & `onestep-0.1.76/src/onestep/__init__.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/broker/base.py` & `onestep-0.1.76/src/onestep/broker/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/broker/cron.py` & `onestep-0.1.76/src/onestep/broker/cron.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/broker/rabbitmq.py` & `onestep-0.1.76/src/onestep/broker/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/broker/webhook.py` & `onestep-0.1.76/src/onestep/broker/webhook.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/exception.py` & `onestep-0.1.76/src/onestep/exception.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/message.py` & `onestep-0.1.76/src/onestep/message.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,10 +1,12 @@
 import json
+import sys
 import time
 import uuid
+from traceback import format_exception, TracebackException
 from typing import Optional, Any, Union
 
 
 class Extra:
     def __init__(self, task_id=None, publish_time=None, failure_count=0):
         self.task_id = task_id or str(uuid.uuid4())
         self.publish_time = publish_time or round(time.time(), 3)
@@ -45,16 +47,17 @@
         if isinstance(extra, Extra):
             return extra
         elif isinstance(extra, dict):
             return Extra(**extra)
         else:
             return Extra()
     
-    def set_exception(self, exception):
-        self.exception = exception
+    def set_exception(self, exception: Optional[Union[TracebackException, Exception, Any]] = None):
+        """设置异常信息 一般不用自己传入exception，会自动获取"""
+        self.exception = exception if exception else TracebackException(*sys.exc_info())
         self.failure_count = self.failure_count + 1
     
     @property
     def exception(self):
         return self._exception
     
     @exception.setter
@@ -82,23 +85,28 @@
                 value = self._set_extra(value)
             setattr(self, key, value)
         return self
     
     def to_dict(self, include_exception=False) -> dict:
         data = {'body': self.body, 'extra': self.extra.to_dict()}
         if include_exception and self.exception:
-            # 保存 异常信息，包括 错误的类名 方法名 行号
-            data['exception'] = {
-                'type': self.exception.__class__.__name__,
-                'message': str(self.exception),
-            }
-            if hasattr(self.exception, '__traceback__'):
-                data['exception']['traceback'] = f"{self.exception.__traceback__.tb_frame.f_code.co_filename}:" \
-                                                 f"{self.exception.__traceback__.tb_frame.f_code.co_name}:" \
-                                                 f"{self.exception.__traceback__.tb_lineno}"
+            if isinstance(self.exception, TracebackException):
+                data['exception'] = "".join(self.exception.format(chain=True))  # noqa
+            elif isinstance(self.exception, Exception):
+                data['exception'] = "".join(
+                    format_exception(
+                        self.exception.__class__, self.exception,
+                        self.exception.__getattr__('__traceback__', None)
+                    )
+                )
+            else:
+                try:
+                    data['exception'] = json.dumps(self.exception)
+                except Exception:
+                    data['exception'] = str(self.exception)
         
         return data
     
     def to_json(self, include_exception=False) -> str:
         return json.dumps(self.to_dict(include_exception))
     
     def confirm(self):
```

### Comparing `onestep-0.1.75/src/onestep/middleware/base.py` & `onestep-0.1.76/src/onestep/middleware/base.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/middleware/config.py` & `onestep-0.1.76/src/onestep/middleware/config.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/onestep.py` & `onestep-0.1.76/src/onestep/onestep.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/retry.py` & `onestep-0.1.76/src/onestep/retry.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/state.py` & `onestep-0.1.76/src/onestep/state.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/store/rabbitmq.py` & `onestep-0.1.76/src/onestep/store/rabbitmq.py`

 * *Files identical despite different names*

### Comparing `onestep-0.1.75/src/onestep/worker.py` & `onestep-0.1.76/src/onestep/worker.py`

 * *Files 0% similar despite different names*

```diff
@@ -74,15 +74,15 @@
                 return message.reject()
             except Exception as e:
                 message_error.send(self, message=message, error=e)
                 if self.instance.state.debug:
                     logger.exception(f"{self.instance.fn.__name__} run error <{type(e).__name__}: {str(e)}>")
                 else:
                     logger.error(f"{self.instance.fn.__name__} run error <{type(e).__name__}: {str(e)}>")
-                message.set_exception(e)
+                message.set_exception()
 
                 retry_state = self.retry(message)
                 if retry_state:  # True=继续（执行重试）
                     continue
                 elif retry_state is False:  # False=结束（执行回调）
                     if self.error_callback:
                         self.error_callback(message)
```

### Comparing `onestep-0.1.75/PKG-INFO` & `onestep-0.1.76/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: onestep
-Version: 0.1.75
+Version: 0.1.76
 Summary: 
 Author: miclon
 Author-email: jcnd@163.com
 Requires-Python: >=3.8,<4.0
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
```

