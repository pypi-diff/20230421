# Comparing `tmp/pyconn-0.2.2.tar.gz` & `tmp/pyconn-0.2.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "pyconn-0.2.2.tar", last modified: Wed Oct 26 06:51:05 2022, max compression
+gzip compressed data, was "pyconn-0.2.3.tar", last modified: Fri Apr 21 07:25:12 2023, max compression
```

## Comparing `pyconn-0.2.2.tar` & `pyconn-0.2.3.tar`

### file list

```diff
@@ -1,33 +1,33 @@
-drwxrwxrwx   0        0        0        0 2022-10-26 06:51:05.754784 pyconn-0.2.2/
--rw-rw-rw-   0        0        0     1288 2021-09-09 08:20:48.000000 pyconn-0.2.2/LICENSE
--rw-rw-rw-   0        0        0       36 2018-01-29 03:34:56.000000 pyconn-0.2.2/MANIFEST.in
--rw-rw-rw-   0        0        0     1794 2022-10-26 06:51:05.754260 pyconn-0.2.2/PKG-INFO
--rw-rw-rw-   0        0        0      202 2022-07-19 06:18:38.000000 pyconn-0.2.2/README.md
-drwxrwxrwx   0        0        0        0 2022-10-26 06:51:05.708819 pyconn-0.2.2/pyconn/
--rw-rw-rw-   0        0        0      756 2021-10-19 02:32:33.000000 pyconn-0.2.2/pyconn/__init__.py
-drwxrwxrwx   0        0        0        0 2022-10-26 06:51:05.726027 pyconn-0.2.2/pyconn/common/
--rw-rw-rw-   0        0        0        0 2021-10-19 02:36:29.000000 pyconn-0.2.2/pyconn/common/__init__.py
--rw-rw-rw-   0        0        0      157 2018-01-29 03:34:56.000000 pyconn-0.2.2/pyconn/common/util.py
-drwxrwxrwx   0        0        0        0 2022-10-26 06:51:05.737065 pyconn-0.2.2/pyconn/db/
--rw-rw-rw-   0        0        0        0 2021-10-19 02:36:29.000000 pyconn-0.2.2/pyconn/db/__init__.py
--rw-rw-rw-   0        0        0     1043 2022-07-19 06:18:38.000000 pyconn-0.2.2/pyconn/db/advancedqreader.py
--rw-rw-rw-   0        0        0     1997 2022-08-08 01:12:11.000000 pyconn-0.2.2/pyconn/db/kdb.py
--rw-rw-rw-   0        0        0     1562 2018-01-29 03:34:56.000000 pyconn-0.2.2/pyconn/db/oracle.py
--rw-rw-rw-   0        0        0     6068 2022-10-26 06:38:01.000000 pyconn-0.2.2/pyconn/db/qpool.py
-drwxrwxrwx   0        0        0        0 2022-10-26 06:51:05.741281 pyconn-0.2.2/pyconn/file/
--rw-rw-rw-   0        0        0        0 2021-10-19 02:36:29.000000 pyconn-0.2.2/pyconn/file/__init__.py
--rw-rw-rw-   0        0        0      187 2018-01-29 03:34:56.000000 pyconn-0.2.2/pyconn/file/csv.py
--rw-rw-rw-   0        0        0       20 2018-01-29 03:34:56.000000 pyconn-0.2.2/pyconn/file/excel.py
--rw-rw-rw-   0        0        0     1283 2018-02-05 08:00:48.000000 pyconn-0.2.2/pyconn/slack.py
-drwxrwxrwx   0        0        0        0 2022-10-26 06:51:05.752648 pyconn-0.2.2/pyconn/wx/
--rw-rw-rw-   0        0        0       20 2018-01-29 03:34:56.000000 pyconn-0.2.2/pyconn/wx/__init__.py
--rw-rw-rw-   0        0        0      258 2019-03-05 02:14:32.000000 pyconn-0.2.2/pyconn/wx/config.py
--rw-rw-rw-   0        0        0     2911 2019-03-05 02:08:29.000000 pyconn-0.2.2/pyconn/wx/wechat.py
-drwxrwxrwx   0        0        0        0 2022-10-26 06:51:05.723421 pyconn-0.2.2/pyconn.egg-info/
--rw-rw-rw-   0        0        0     1794 2022-10-26 06:51:05.000000 pyconn-0.2.2/pyconn.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      503 2022-10-26 06:51:05.000000 pyconn-0.2.2/pyconn.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2022-10-26 06:51:05.000000 pyconn-0.2.2/pyconn.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0       28 2022-10-26 06:51:05.000000 pyconn-0.2.2/pyconn.egg-info/requires.txt
--rw-rw-rw-   0        0        0        7 2022-10-26 06:51:05.000000 pyconn-0.2.2/pyconn.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2022-10-26 06:51:05.755340 pyconn-0.2.2/setup.cfg
--rw-rw-rw-   0        0        0      561 2022-10-26 05:59:37.000000 pyconn-0.2.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:25:12.491304 pyconn-0.2.3/
+-rw-rw-rw-   0        0        0     1288 2021-09-09 08:20:48.000000 pyconn-0.2.3/LICENSE
+-rw-rw-rw-   0        0        0       36 2018-01-29 03:34:56.000000 pyconn-0.2.3/MANIFEST.in
+-rw-rw-rw-   0        0        0     1817 2023-04-21 07:25:12.490792 pyconn-0.2.3/PKG-INFO
+-rw-rw-rw-   0        0        0      202 2022-07-19 06:18:38.000000 pyconn-0.2.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 07:25:12.456625 pyconn-0.2.3/pyconn/
+-rw-rw-rw-   0        0        0      756 2021-10-19 02:32:33.000000 pyconn-0.2.3/pyconn/__init__.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:25:12.478865 pyconn-0.2.3/pyconn/common/
+-rw-rw-rw-   0        0        0        0 2021-10-19 02:36:29.000000 pyconn-0.2.3/pyconn/common/__init__.py
+-rw-rw-rw-   0        0        0      157 2018-01-29 03:34:56.000000 pyconn-0.2.3/pyconn/common/util.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:25:12.483052 pyconn-0.2.3/pyconn/db/
+-rw-rw-rw-   0        0        0        0 2021-10-19 02:36:29.000000 pyconn-0.2.3/pyconn/db/__init__.py
+-rw-rw-rw-   0        0        0     1043 2022-12-13 07:40:49.000000 pyconn-0.2.3/pyconn/db/advancedqreader.py
+-rw-rw-rw-   0        0        0     1997 2022-08-08 01:12:11.000000 pyconn-0.2.3/pyconn/db/kdb.py
+-rw-rw-rw-   0        0        0     1562 2018-01-29 03:34:56.000000 pyconn-0.2.3/pyconn/db/oracle.py
+-rw-rw-rw-   0        0        0     6871 2023-03-21 06:09:25.000000 pyconn-0.2.3/pyconn/db/qpool.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:25:12.486155 pyconn-0.2.3/pyconn/file/
+-rw-rw-rw-   0        0        0        0 2021-10-19 02:36:29.000000 pyconn-0.2.3/pyconn/file/__init__.py
+-rw-rw-rw-   0        0        0      187 2018-01-29 03:34:56.000000 pyconn-0.2.3/pyconn/file/csv.py
+-rw-rw-rw-   0        0        0       20 2018-01-29 03:34:56.000000 pyconn-0.2.3/pyconn/file/excel.py
+-rw-rw-rw-   0        0        0     1283 2018-02-05 08:00:48.000000 pyconn-0.2.3/pyconn/slack.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:25:12.489769 pyconn-0.2.3/pyconn/wx/
+-rw-rw-rw-   0        0        0       20 2018-01-29 03:34:56.000000 pyconn-0.2.3/pyconn/wx/__init__.py
+-rw-rw-rw-   0        0        0      258 2019-03-05 02:14:32.000000 pyconn-0.2.3/pyconn/wx/config.py
+-rw-rw-rw-   0        0        0     2911 2019-03-05 02:08:29.000000 pyconn-0.2.3/pyconn/wx/wechat.py
+drwxrwxrwx   0        0        0        0 2023-04-21 07:25:12.477295 pyconn-0.2.3/pyconn.egg-info/
+-rw-rw-rw-   0        0        0     1817 2023-04-21 07:25:11.000000 pyconn-0.2.3/pyconn.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      503 2023-04-21 07:25:12.000000 pyconn-0.2.3/pyconn.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 07:25:11.000000 pyconn-0.2.3/pyconn.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0       29 2023-04-21 07:25:12.000000 pyconn-0.2.3/pyconn.egg-info/requires.txt
+-rw-rw-rw-   0        0        0        7 2023-04-21 07:25:12.000000 pyconn-0.2.3/pyconn.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 07:25:12.491304 pyconn-0.2.3/setup.cfg
+-rw-rw-rw-   0        0        0      562 2023-04-21 07:21:56.000000 pyconn-0.2.3/setup.py
```

### Comparing `pyconn-0.2.2/LICENSE` & `pyconn-0.2.3/LICENSE`

 * *Files identical despite different names*

### Comparing `pyconn-0.2.2/PKG-INFO` & `pyconn-0.2.3/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyconn
-Version: 0.2.2
+Version: 0.2.3
 Summary: python connection tools collection
 Home-page: 
 Author: luoanni
 Author-email: luoanni33@gmail.com
 License: Copyright (c) 2016, James Liu
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
         Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pyconn is a tool set which include:
 
 1. Connect and query kdb+, Oracle database
 
@@ -25,7 +26,9 @@
 
 ## Requirements
 - Python 3.6+
 - qpython 2.0+
 - numpy
 - pandas
 - cx_Oracle
+
+
```

### Comparing `pyconn-0.2.2/pyconn/__init__.py` & `pyconn-0.2.3/pyconn/__init__.py`

 * *Files identical despite different names*

### Comparing `pyconn-0.2.2/pyconn/db/advancedqreader.py` & `pyconn-0.2.3/pyconn/db/advancedqreader.py`

 * *Files identical despite different names*

### Comparing `pyconn-0.2.2/pyconn/db/kdb.py` & `pyconn-0.2.3/pyconn/db/kdb.py`

 * *Files identical despite different names*

### Comparing `pyconn-0.2.2/pyconn/db/oracle.py` & `pyconn-0.2.3/pyconn/db/oracle.py`

 * *Files identical despite different names*

### Comparing `pyconn-0.2.2/pyconn/db/qpool.py` & `pyconn-0.2.3/pyconn/db/qpool.py`

 * *Files 15% similar despite different names*

```diff
@@ -136,14 +136,29 @@
                 log_str = f'DB[{self.server.name}] error: {e.args}, query: {query}, params: {parameters}, options: {options}'
                 logger.error(log_str)
         else:
             log_str = f'Process[{os.getpid()}], Thread[{threading.get_ident()}], DB[{self.server.name}] error: Invalid handle, query: {query}, params: {parameters}, options: {options}'
             logger.error(log_str)
         return result
 
+    def query_async(self, query, *parameters, **options):
+        result = None
+        self.conn = self.pool.get_connection(self.server)
+        if self.conn is not None and self.conn.is_connected:
+            try:
+                with self.conn.lock:
+                    result = self.conn.sendaSync(query, *parameters, **options)
+            except Exception as e:
+                log_str = f'DB[{self.server.name}] error: {e.args}, query: {query}, params: {parameters}, options: {options}'
+                logger.error(log_str)
+        else:
+            log_str = f'Process[{os.getpid()}], Thread[{threading.get_ident()}], DB[{self.server.name}] error: Invalid handle, query: {query}, params: {parameters}, options: {options}'
+            logger.error(log_str)
+        return result
+
     @staticmethod
     def to_sym(s):
         return numpy.string_(s, encoding='utf-8')
 
     @staticmethod
     def to_sym_list(arr):
         """
```

### Comparing `pyconn-0.2.2/pyconn/slack.py` & `pyconn-0.2.3/pyconn/slack.py`

 * *Files identical despite different names*

### Comparing `pyconn-0.2.2/pyconn/wx/wechat.py` & `pyconn-0.2.3/pyconn/wx/wechat.py`

 * *Files identical despite different names*

### Comparing `pyconn-0.2.2/pyconn.egg-info/PKG-INFO` & `pyconn-0.2.3/pyconn.egg-info/PKG-INFO`

 * *Files 18% similar despite different names*

```diff
@@ -1,23 +1,24 @@
 Metadata-Version: 2.1
 Name: pyconn
-Version: 0.2.2
+Version: 0.2.3
 Summary: python connection tools collection
 Home-page: 
 Author: luoanni
 Author-email: luoanni33@gmail.com
 License: Copyright (c) 2016, James Liu
         
         All rights reserved.
         
         Redistribution and use in source and binary forms, with or without modification, are permitted provided that the following conditions are met:
         
         Redistributions of source code must retain the above copyright notice, this list of conditions and the following disclaimer.
         Redistributions in binary form must reproduce the above copyright notice, this list of conditions and the following disclaimer in the documentation and/or other materials provided with the distribution.
         THIS SOFTWARE IS PROVIDED BY THE COPYRIGHT HOLDERS AND CONTRIBUTORS "AS IS" AND ANY EXPRESS OR IMPLIED WARRANTIES, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE ARE DISCLAIMED. IN NO EVENT SHALL THE COPYRIGHT HOLDER OR CONTRIBUTORS BE LIABLE FOR ANY DIRECT, INDIRECT, INCIDENTAL, SPECIAL, EXEMPLARY, OR CONSEQUENTIAL DAMAGES (INCLUDING, BUT NOT LIMITED TO, PROCUREMENT OF SUBSTITUTE GOODS OR SERVICES; LOSS OF USE, DATA, OR PROFITS; OR BUSINESS INTERRUPTION) HOWEVER CAUSED AND ON ANY THEORY OF LIABILITY, WHETHER IN CONTRACT, STRICT LIABILITY, OR TORT (INCLUDING NEGLIGENCE OR OTHERWISE) ARISING IN ANY WAY OUT OF THE USE OF THIS SOFTWARE, EVEN IF ADVISED OF THE POSSIBILITY OF SUCH DAMAGE.
+Platform: UNKNOWN
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 pyconn is a tool set which include:
 
 1. Connect and query kdb+, Oracle database
 
@@ -25,7 +26,9 @@
 
 ## Requirements
 - Python 3.6+
 - qpython 2.0+
 - numpy
 - pandas
 - cx_Oracle
+
+
```

### Comparing `pyconn-0.2.2/setup.py` & `pyconn-0.2.3/setup.py`

 * *Files 20% similar despite different names*

```diff
@@ -4,18 +4,18 @@
     readme = f.read()
 
 with open('LICENSE') as f:
     license = f.read()
 
 setup(
     name='pyconn',
-    version='0.2.2',
+    version='0.2.3',
     description='python connection tools collection',
     long_description=readme,
     long_description_content_type='text/markdown',
     author='luoanni',
     author_email='luoanni33@gmail.com',
     url='',
     license=license,
     packages=find_packages(exclude=('tests', 'docs')),
-    install_requires=['qPython>=2.0.0', 'numpy', 'pandas']
+    install_requires=['qPython3>=1.0.0', 'numpy', 'pandas']
 )
```

