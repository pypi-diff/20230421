# Comparing `tmp/PrSpiders-0.4.0.tar.gz` & `tmp/PrSpiders-0.4.1.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "PrSpiders-0.4.0.tar", last modified: Wed Apr 19 08:21:10 2023, max compression
+gzip compressed data, was "PrSpiders-0.4.1.tar", last modified: Thu Apr 20 09:13:59 2023, max compression
```

## Comparing `PrSpiders-0.4.0.tar` & `PrSpiders-0.4.1.tar`

### file list

```diff
@@ -1,31 +1,31 @@
-drwxrwxrwx   0        0        0        0 2023-04-19 08:21:09.976073 PrSpiders-0.4.0/
--rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.4.0/LICENSE.txt
--rw-rw-rw-   0        0        0     4583 2023-04-19 08:21:09.969067 PrSpiders-0.4.0/PKG-INFO
-drwxrwxrwx   0        0        0        0 2023-04-19 08:21:07.980079 PrSpiders-0.4.0/PrSpider/
--rw-rw-rw-   0        0        0    11541 2023-04-19 06:57:57.000000 PrSpiders-0.4.0/PrSpider/PrSpiders.py
--rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.4.0/PrSpider/__init__.py
--rw-rw-rw-   0        0        0    11191 2023-04-18 06:06:03.000000 PrSpiders-0.4.0/PrSpider/pxpath.py
--rw-rw-rw-   0        0        0     4296 2023-04-19 08:20:32.000000 PrSpiders-0.4.0/PrSpider/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.0/PrSpider/useragent.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:21:08.303066 PrSpiders-0.4.0/PrSpiders.egg-info/
--rw-rw-rw-   0        0        0     4583 2023-04-19 08:21:04.000000 PrSpiders-0.4.0/PrSpiders.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      563 2023-04-19 08:21:05.000000 PrSpiders-0.4.0/PrSpiders.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-19 08:21:04.000000 PrSpiders-0.4.0/PrSpiders.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       61 2023-04-19 08:21:04.000000 PrSpiders-0.4.0/PrSpiders.egg-info/entry_points.txt
--rw-rw-rw-   0        0        0       40 2023-04-19 08:21:05.000000 PrSpiders-0.4.0/PrSpiders.egg-info/requires.txt
--rw-rw-rw-   0        0        0       26 2023-04-19 08:21:05.000000 PrSpiders-0.4.0/PrSpiders.egg-info/top_level.txt
--rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.4.0/README.md
-drwxrwxrwx   0        0        0        0 2023-04-19 08:21:08.591069 PrSpiders-0.4.0/pkg/
--rw-rw-rw-   0        0        0       23 2023-04-19 08:20:56.000000 PrSpiders-0.4.0/pkg/__init__.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:21:09.436070 PrSpiders-0.4.0/pkg/prspider/
--rw-rw-rw-   0        0        0     1168 2023-04-18 06:21:44.000000 PrSpiders-0.4.0/pkg/prspider/PrSpider_CMD.py
--rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.4.0/pkg/prspider/PrSpider_run.py
--rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.4.0/pkg/prspider/__init__.py
--rw-rw-rw-   0        0        0      494 2023-04-18 01:45:59.000000 PrSpiders-0.4.0/pkg/prspider/start.py
-drwxrwxrwx   0        0        0        0 2023-04-19 08:21:09.800065 PrSpiders-0.4.0/requestXpath/
--rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.4.0/requestXpath/__init__.py
--rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.4.0/requestXpath/pxpath.py
--rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.4.0/requestXpath/requestXpath.py
--rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.0/requestXpath/useragent.py
--rw-rw-rw-   0        0        0       42 2023-04-19 08:21:10.002069 PrSpiders-0.4.0/setup.cfg
--rw-rw-rw-   0        0        0     1022 2023-04-19 08:21:00.000000 PrSpiders-0.4.0/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:13:59.430207 PrSpiders-0.4.1/
+-rw-rw-rw-   0        0        0     1091 2023-02-21 09:22:44.000000 PrSpiders-0.4.1/LICENSE.txt
+-rw-rw-rw-   0        0        0     4583 2023-04-20 09:13:59.415198 PrSpiders-0.4.1/PKG-INFO
+drwxrwxrwx   0        0        0        0 2023-04-20 09:13:57.629204 PrSpiders-0.4.1/PrSpider/
+-rw-rw-rw-   0        0        0    11875 2023-04-20 09:05:41.000000 PrSpiders-0.4.1/PrSpider/PrSpiders.py
+-rw-rw-rw-   0        0        0       44 2023-03-28 05:34:05.000000 PrSpiders-0.4.1/PrSpider/__init__.py
+-rw-rw-rw-   0        0        0    11191 2023-04-18 06:06:03.000000 PrSpiders-0.4.1/PrSpider/pxpath.py
+-rw-rw-rw-   0        0        0     4423 2023-04-20 09:05:42.000000 PrSpiders-0.4.1/PrSpider/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.1/PrSpider/useragent.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:13:58.292204 PrSpiders-0.4.1/PrSpiders.egg-info/
+-rw-rw-rw-   0        0        0     4583 2023-04-20 09:13:56.000000 PrSpiders-0.4.1/PrSpiders.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      563 2023-04-20 09:13:57.000000 PrSpiders-0.4.1/PrSpiders.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-20 09:13:56.000000 PrSpiders-0.4.1/PrSpiders.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       61 2023-04-20 09:13:56.000000 PrSpiders-0.4.1/PrSpiders.egg-info/entry_points.txt
+-rw-rw-rw-   0        0        0       40 2023-04-20 09:13:56.000000 PrSpiders-0.4.1/PrSpiders.egg-info/requires.txt
+-rw-rw-rw-   0        0        0       26 2023-04-20 09:13:56.000000 PrSpiders-0.4.1/PrSpiders.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0     4071 2023-04-18 02:48:25.000000 PrSpiders-0.4.1/README.md
+drwxrwxrwx   0        0        0        0 2023-04-20 09:13:58.632202 PrSpiders-0.4.1/pkg/
+-rw-rw-rw-   0        0        0       23 2023-04-20 09:05:54.000000 PrSpiders-0.4.1/pkg/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:13:59.087200 PrSpiders-0.4.1/pkg/prspider/
+-rw-rw-rw-   0        0        0     1212 2023-04-20 09:13:43.000000 PrSpiders-0.4.1/pkg/prspider/PrSpider_CMD.py
+-rw-rw-rw-   0        0        0      257 2023-04-17 12:23:25.000000 PrSpiders-0.4.1/pkg/prspider/PrSpider_run.py
+-rw-rw-rw-   0        0        0       73 2023-03-31 05:29:27.000000 PrSpiders-0.4.1/pkg/prspider/__init__.py
+-rw-rw-rw-   0        0        0      835 2023-04-20 09:10:51.000000 PrSpiders-0.4.1/pkg/prspider/start.py
+drwxrwxrwx   0        0        0        0 2023-04-20 09:13:59.319201 PrSpiders-0.4.1/requestXpath/
+-rw-rw-rw-   0        0        0      933 2023-03-23 08:11:59.000000 PrSpiders-0.4.1/requestXpath/__init__.py
+-rw-rw-rw-   0        0        0     8642 2023-04-18 08:44:05.000000 PrSpiders-0.4.1/requestXpath/pxpath.py
+-rw-rw-rw-   0        0        0     4210 2023-03-23 08:11:59.000000 PrSpiders-0.4.1/requestXpath/requestXpath.py
+-rw-rw-rw-   0        0        0    11789 2023-02-22 08:11:29.000000 PrSpiders-0.4.1/requestXpath/useragent.py
+-rw-rw-rw-   0        0        0       42 2023-04-20 09:13:59.549204 PrSpiders-0.4.1/setup.cfg
+-rw-rw-rw-   0        0        0     1022 2023-04-20 09:05:46.000000 PrSpiders-0.4.1/setup.py
```

### Comparing `PrSpiders-0.4.0/LICENSE.txt` & `PrSpiders-0.4.1/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.0/PKG-INFO` & `PrSpiders-0.4.1/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.0
+Version: 0.4.1
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.0/PrSpider/PrSpiders.py` & `PrSpiders-0.4.1/PrSpider/PrSpiders.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,12 +1,13 @@
 import os
 import re
+import sys
 import logging
 import time
-import datetime
+import datetime, random
 from typing import Optional
 from .requestXpath import prequest
 from concurrent.futures import ThreadPoolExecutor, as_completed
 
 
 class settions(object):
     workers: Optional[int] = 1
@@ -15,15 +16,15 @@
     false_num: Optional[int] = 0
     setting: Optional[dict] = None
     start_urls: Optional[list] = None
     executor: Optional[object] = None
     retry: Optional[bool] = True
     pid: Optional[int] = os.getppid()
     start_time: Optional[int] = time.time()
-    download_delay: Optional[int] = 1
+    download_delay: Optional[int] = 0
     download_num: Optional[int] = 5
     log: Optional[object] = False
     logger: Optional[bool or str] = False
     log_level: Optional[str] = "info"
 
 
 class PrSpiders(settions):
@@ -87,16 +88,17 @@
             )
         else:
             url_dim_list = [
                 request[i : i + cls.download_num]
                 for i in range(0, len(request), cls.download_num)
             ]
             for u in url_dim_list:
-                time.sleep(cls.download_delay)
+                time.sleep(cls.download_delay + random.uniform(0.0000001, 0.0000005))
                 for _u in u:
+                    time.sleep(random.uniform(0.00000001, 0.00000005))
                     url = _u.get("url")
                     data = _u.get("data", None)
                     params = _u.get("params", None)
                     meta = _u.get("meta", None)
                     kwargs.update({"data": data})
                     kwargs.update({"params": params})
                     futures.append(
@@ -111,23 +113,22 @@
                             meta=meta,
                             encoding=encoding,
                             retry_interval=retry_interval,
                             **kwargs,
                         )
                     )
 
-                for future in as_completed(futures):
-                    worker_exception = future.exception()
-                    if worker_exception:
-                        current_time = datetime.datetime.now().strftime(
-                            "%Y-%m-%d %H:%M:%S"
-                        )
-                        cls.log.exception(
-                            f"{current_time} [PrSpider Exception] %s" % worker_exception
-                        )
+            for future in as_completed(futures):
+                futures.remove(future)
+                worker_exception = future.exception()
+                if worker_exception:
+                    current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
+                    cls.log.exception(
+                        f"{current_time} [PrSpider Exception] %s" % worker_exception
+                    )
 
     @classmethod
     def Requests(
         cls,
         url=None,
         callback=None,
         headers=None,
@@ -142,16 +143,17 @@
         futures = []
         if isinstance(url, str):
             url = [url]
         url_dim_list = [
             url[i : i + cls.download_num] for i in range(0, len(url), cls.download_num)
         ]
         for u in url_dim_list:
-            time.sleep(cls.download_delay)
+            time.sleep(cls.download_delay + random.uniform(0.0000001, 0.0000005))
             for _u in u:
+                time.sleep(random.uniform(0.00000001, 0.00000005))
                 futures.append(
                     ThreadPoolExecutor(cls.workers).submit(
                         cls.fetch,
                         url=_u,
                         callback=callback,
                         headers=headers,
                         timeout=timeout,
@@ -161,14 +163,15 @@
                         encoding=encoding,
                         retry_interval=retry_interval,
                         **kwargs,
                     )
                 )
 
         for future in as_completed(futures):
+            futures.remove(future)
             worker_exception = future.exception()
             if worker_exception:
                 current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
                 cls.log.exception(
                     f"{current_time} [PrSpider Exception] %s" % worker_exception
                 )
 
@@ -184,15 +187,14 @@
         encoding="utf-8",
         retry_interval=1,
         timeout=3,
         **kwargs,
     ):
         settions.request_num += 1
         current_time = datetime.datetime.now().strftime("%Y-%m-%d %H:%M:%S")
-        time.sleep(self.download_delay)
         response = prequest(self.log).get(
             url,
             headers=headers,
             retry_time=retry_time,
             method=method,
             meta=meta,
             encoding=encoding,
@@ -201,39 +203,39 @@
             settion=settions,
             **kwargs,
         )
         if response:
             if response.ok:
                 settions.success_num += 1
                 self.log.info(
-                    f"{current_time} [PrSpider] True [Method] {method} [Status] {response.code} [Url] {url}"
+                    f"{current_time} [Method] {method} [Status] {response.code} [Url] {url}"
                 )
                 callback(response)
                 return self
             else:
                 settions.false_num += 1
                 if response:
                     self.log.error(
-                        f"{current_time} [PrSpider] False [Method] {method} [Status] {response.code} [Url] {url}"
+                        f"{current_time} [Method] {method} [Status] {response.code} [Url] {url}"
                     )
                 else:
                     self.log.error(
-                        f"{current_time} [PrSpider] Error [Method] {method} [Status] Timeout [Url] {url}"
+                        f"{current_time} [Method] {method} [Status] Timeout [Url] {url}"
                     )
                 callback(response)
                 return self
         else:
             settions.false_num += 1
             if response:
                 self.log.error(
-                    f"{current_time} [PrSpider] False [Method] {method} [Status] {response.code} [Url] {url}"
+                    f"{current_time} [Method] {method} [Status] {response.code} [Url] {url}"
                 )
             else:
                 self.log.error(
-                    f"{current_time} [PrSpider] Error [Method] {method} [Status] Timeout [Url] {url}"
+                    f"{current_time} [Method] {method} [Status] Error [Url] {url}"
                 )
             callback(response)
             return self
 
     @classmethod
     def parse(self, response):
         raise NotImplementedError(
@@ -256,19 +258,18 @@
             "info": logging.INFO,
             "debug": logging.DEBUG,
             "error": logging.ERROR,
             "critical": logging.CRITICAL,
         }
         level = level_dict.get(level.lower())
         logger = logging.getLogger()
-        logger.setLevel(logging.DEBUG)
+        logger.setLevel(level)
+        sys.stdout = FileLike(logger)
 
-        formatter = logging.basicConfig(
-            format="[%(levelname)s] %(message)s", level=level
-        )
+        formatter = logging.basicConfig(format="%(message)s", level=level)
         # 创建一个handler，用于写入日志文件，并设置日志级别，mode:a是追加写模式，w是覆盖写模式
         if file_log:
             file_log = os.path.basename(__file__) if file_log is True else file_log
             file_log = (
                 re.sub("\..*", ".log", file_log)
                 if "." in file_log
                 else file_log + ".log"
@@ -314,7 +315,19 @@
             self.false_num,
             self.process_timestamp(self.start_time),
             self.process_timestamp(end_time),
             spend_time,
             average_time,
         )
         self.log.info(m)
+
+
+class FileLike:
+    def __init__(self, logger):
+        self.logger = logger
+
+    def write(self, message):
+        if message != "\n":
+            self.logger.log(logging.CRITICAL, message)
+
+    def flush(self):
+        pass
```

### Comparing `PrSpiders-0.4.0/PrSpider/pxpath.py` & `PrSpiders-0.4.1/PrSpider/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.0/PrSpider/requestXpath.py` & `PrSpiders-0.4.1/PrSpider/requestXpath.py`

 * *Files 2% similar despite different names*

```diff
@@ -85,19 +85,26 @@
                     *args,
                     **kwargs,
                 )
                 self.response.encoding = encoding
                 if self.response.ok:
                     return self
                 else:
-                    raise Exception(f"Respider {self.retry_interval}s")
+                    raise Exception(f"Response.ok is False")
+
             except Exception as e:
-                self.log.error("%s [ERRORS] %s [Msg] %s" % (self.current_time, url, e))
                 if settion.retry:
-                    self.log.info("[Retry] %s [Interval] %ss" % (url, retry_interval))
+                    self.log.info(
+                        "[Retry] %s [Msg] %s [Interval] %ss" % (url, e, retry_interval)
+                    )
+                else:
+                    self.log.info(
+                        "%s [ERRORS] %s [Msg] %s" % (self.current_time, url, e)
+                    )
+
                 retry_time -= 1
                 if retry_time <= 0 or settion.retry is False:
                     self.response.status_code = (
                         410
                         if not self.response.status_code
                         else self.response.status_code
                     )
```

### Comparing `PrSpiders-0.4.0/PrSpider/useragent.py` & `PrSpiders-0.4.1/PrSpider/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.0/PrSpiders.egg-info/PKG-INFO` & `PrSpiders-0.4.1/PrSpiders.egg-info/PKG-INFO`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: PrSpiders
-Version: 0.4.0
+Version: 0.4.1
 Summary: Inherit the requests module, add xpath functionality to expand the API, and handle request failures and retries
 Home-page: https://github.com/peng0928/prequests
 Author: penr
 Author-email: 1944542244@qq.com
 License: MIT
 Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
```

### Comparing `PrSpiders-0.4.0/PrSpiders.egg-info/SOURCES.txt` & `PrSpiders-0.4.1/PrSpiders.egg-info/SOURCES.txt`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.0/README.md` & `PrSpiders-0.4.1/README.md`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.0/pkg/prspider/PrSpider_CMD.py` & `PrSpiders-0.4.1/pkg/prspider/PrSpider_CMD.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 # encoding:utf-8
 
 from pkg import __version__
 import argparse
 
-from .start import start_code
+from .start import start_code, spider
 
 
 def get_version():
     return __version__
 
 
 def main():
@@ -34,10 +34,13 @@
     start = args.start
     keys = args.keys
     url = args.url
     if start:
         start_code(start)
         print("完成", start)
 
+    if url:
+        spider(url)
+
 
 if __name__ == "__main__":
     main()
```

### Comparing `PrSpiders-0.4.0/requestXpath/__init__.py` & `PrSpiders-0.4.1/requestXpath/__init__.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.0/requestXpath/pxpath.py` & `PrSpiders-0.4.1/requestXpath/pxpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.0/requestXpath/requestXpath.py` & `PrSpiders-0.4.1/requestXpath/requestXpath.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.0/requestXpath/useragent.py` & `PrSpiders-0.4.1/requestXpath/useragent.py`

 * *Files identical despite different names*

### Comparing `PrSpiders-0.4.0/setup.py` & `PrSpiders-0.4.1/setup.py`

 * *Files 1% similar despite different names*

```diff
@@ -1,13 +1,13 @@
 #!python
 # -*- coding:utf-8 -*-
 from __future__ import print_function
 from setuptools import setup, find_packages
 
-__version__ = "0.4.0"
+__version__ = "0.4.1"
 
 with open("README.md", "r", encoding="utf-8") as fh:
     long_description = fh.read()
 
 setup(
     name="PrSpiders",
     version=__version__,
```

