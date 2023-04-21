# Comparing `tmp/unitranscode-0.1.0.tar.gz` & `tmp/unitranscode-0.2.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "unitranscode-0.1.0.tar", last modified: Sun Jan  1 03:23:01 2023, max compression
+gzip compressed data, was "unitranscode-0.2.0.tar", last modified: Fri Apr 21 07:42:30 2023, max compression
```

## Comparing `unitranscode-0.1.0.tar` & `unitranscode-0.2.0.tar`

### file list

```diff
@@ -1,17 +1,19 @@
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-01-01 03:23:01.979788 unitranscode-0.1.0/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.1.0/LICENSE
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-01-01 03:23:01.979788 unitranscode-0.1.0/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.1.0/README.md
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-01-01 03:23:01.979788 unitranscode-0.1.0/setup.cfg
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      691 2023-01-01 03:22:29.000000 unitranscode-0.1.0/setup.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-01-01 03:23:01.979788 unitranscode-0.1.0/unitranscode/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.1.0/unitranscode/__init__.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)     3187 2022-12-31 23:03:38.000000 unitranscode-0.1.0/unitranscode/custom_types.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)    21410 2023-01-01 03:10:23.000000 unitranscode-0.1.0/unitranscode/transcoder.py
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-01-01 01:28:30.000000 unitranscode-0.1.0/unitranscode/utils.py
-drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-01-01 03:23:01.979788 unitranscode-0.1.0/unitranscode.egg-info/
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      603 2023-01-01 03:23:01.000000 unitranscode-0.1.0/unitranscode.egg-info/PKG-INFO
--rw-rw-r--   0 matthew   (1000) matthew   (1000)      308 2023-01-01 03:23:01.000000 unitranscode-0.1.0/unitranscode.egg-info/SOURCES.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-01-01 03:23:01.000000 unitranscode-0.1.0/unitranscode.egg-info/dependency_links.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-01-01 03:23:01.000000 unitranscode-0.1.0/unitranscode.egg-info/requires.txt
--rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-01-01 03:23:01.000000 unitranscode-0.1.0/unitranscode.egg-info/top_level.txt
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 07:42:30.237139 unitranscode-0.2.0/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1062 2023-01-01 01:11:48.000000 unitranscode-0.2.0/LICENSE
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-04-21 07:42:30.237139 unitranscode-0.2.0/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     1399 2023-01-01 03:15:58.000000 unitranscode-0.2.0/README.md
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       38 2023-04-21 07:42:30.237139 unitranscode-0.2.0/setup.cfg
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      716 2023-04-21 07:41:27.000000 unitranscode-0.2.0/setup.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 07:42:30.237139 unitranscode-0.2.0/tests/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      672 2023-04-21 07:38:21.000000 unitranscode-0.2.0/tests/test_transcoder.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 07:42:30.237139 unitranscode-0.2.0/unitranscode/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      411 2023-01-01 01:28:59.000000 unitranscode-0.2.0/unitranscode/__init__.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)     3187 2022-12-31 23:03:38.000000 unitranscode-0.2.0/unitranscode/custom_types.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)    22131 2023-04-21 07:36:48.000000 unitranscode-0.2.0/unitranscode/transcoder.py
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      137 2023-01-01 01:28:30.000000 unitranscode-0.2.0/unitranscode/utils.py
+drwxrwxr-x   0 matthew   (1000) matthew   (1000)        0 2023-04-21 07:42:30.237139 unitranscode-0.2.0/unitranscode.egg-info/
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      558 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/PKG-INFO
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)      333 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/SOURCES.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        1 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/dependency_links.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)        7 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/requires.txt
+-rw-rw-r--   0 matthew   (1000) matthew   (1000)       13 2023-04-21 07:42:30.000000 unitranscode-0.2.0/unitranscode.egg-info/top_level.txt
```

### Comparing `unitranscode-0.1.0/LICENSE` & `unitranscode-0.2.0/LICENSE`

 * *Files identical despite different names*

### Comparing `unitranscode-0.1.0/PKG-INFO` & `unitranscode-0.2.0/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.1.0
+Version: 0.2.0
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
-License: UNKNOWN
 Keywords: unitranscode
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
-
-UNKNOWN
-
```

### Comparing `unitranscode-0.1.0/README.md` & `unitranscode-0.2.0/README.md`

 * *Files identical despite different names*

### Comparing `unitranscode-0.1.0/setup.py` & `unitranscode-0.2.0/setup.py`

 * *Files 16% similar despite different names*

```diff
@@ -1,24 +1,22 @@
 from setuptools import setup
 
 setup(
     name='unitranscode',
-    version='0.1.0',
+    version='0.2.0',
     description='Universal transcoding library',
     url='https://github.com/MatthewScholefield/unitranscode',
     author='Matthew D. Scholefield',
     author_email='matthew331199@gmail.com',
     classifiers=[
         'Development Status :: 3 - Alpha',
-
         'Intended Audience :: Developers',
         'Programming Language :: Python :: 3',
         'Programming Language :: Python :: 3.8',
         'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
     ],
     keywords='unitranscode',
     packages=['unitranscode'],
-    install_requires=[
-        'loguru'
-    ],
+    install_requires=['loguru'],
+    extra_requires={'dev': ['pytest']},
 )
```

### Comparing `unitranscode-0.1.0/unitranscode/custom_types.py` & `unitranscode-0.2.0/unitranscode/custom_types.py`

 * *Files identical despite different names*

### Comparing `unitranscode-0.1.0/unitranscode/transcoder.py` & `unitranscode-0.2.0/unitranscode/transcoder.py`

 * *Files 2% similar despite different names*

```diff
@@ -10,15 +10,15 @@
 from functools import cached_property, lru_cache
 from os.path import abspath, isfile, splitext
 from signal import SIGCONT, SIGTSTP
 from subprocess import PIPE, Popen
 from tempfile import NamedTemporaryFile
 from threading import Lock
 from time import sleep
-from typing import List, Optional, Union
+from typing import List, Optional, Tuple, Union
 
 from loguru import logger
 
 from .custom_types import (
     AudiogramOp,
     EncodingInfo,
     ProgressHandler,
@@ -173,24 +173,21 @@
         on_progress: ProgressHandler = None,
         op: FfmpegOperation = None,
         force_no_transcode: bool = True,
     ) -> str:
         op = op or self.op()
         assert force_no_transcode, 'Transcoding not supported yet for chop'
         assert (
-            pos_start_s is None
-        ), 'Custom start position not supported yet for chop'
-        assert (
-            pos_end_s is not None
-        ), 'Undefined end position not supported yet for chop'
+            pos_start_s is None or pos_end_s is not None
+        ), 'Must specify either start or end position to chop to'
         self.ffmpeg(
             *['-i', in_file],
             *['-c', 'copy'],
-            *['-ss', '0'],
-            *['-t', str(pos_end_s)],
+            *['-ss', str(pos_start_s)] * (pos_start_s is not None),
+            *['-to', str(pos_end_s)] * (pos_end_s is not None),
             out_file,
             duration_s=self.info(in_file).duration_s if on_progress else None,
             on_progress=on_progress,
             op=op,
         )
         return out_file
 
@@ -545,14 +542,38 @@
                 out_file,
                 duration_s=duration_s,
                 on_progress=on_progress,
                 op=op,
             )
         return out_file
 
+    def edit(
+        self,
+        in_file: str,
+        cuts: List[Tuple[float, float]],
+        output_file: str,
+        on_progress: ProgressHandler = None,
+        op: FfmpegOperation = None,
+    ) -> str:
+        op = op or self.op()
+        filter_str = '+'.join(
+            f'between(t,{start},{end})' for start, end in cuts
+        )
+
+        self.ffmpeg(
+            *('-i', in_file),
+            *('-vf', f"select='{filter_str}',setpts=N/FRAME_RATE/TB"),
+            *('-af', f"aselect='{filter_str}',asetpts=N/SR/TB"),
+            output_file,
+            duration_s=self.info(in_file).duration_s if on_progress else None,
+            on_progress=on_progress,
+            op=op,
+        )
+        return output_file
+
     def split(
         self,
         in_file: str,
         split_timestamps: Optional[List[float]],
         out_file_fmt='{in_base}-%d.{in_ext}',
         on_progress: ProgressHandler = None,
         op: FfmpegOperation = None,
```

### Comparing `unitranscode-0.1.0/unitranscode.egg-info/PKG-INFO` & `unitranscode-0.2.0/unitranscode.egg-info/PKG-INFO`

 * *Files 12% similar despite different names*

```diff
@@ -1,20 +1,15 @@
 Metadata-Version: 2.1
 Name: unitranscode
-Version: 0.1.0
+Version: 0.2.0
 Summary: Universal transcoding library
 Home-page: https://github.com/MatthewScholefield/unitranscode
 Author: Matthew D. Scholefield
 Author-email: matthew331199@gmail.com
-License: UNKNOWN
 Keywords: unitranscode
-Platform: UNKNOWN
 Classifier: Development Status :: 3 - Alpha
 Classifier: Intended Audience :: Developers
 Classifier: Programming Language :: Python :: 3
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 License-File: LICENSE
-
-UNKNOWN
-
```

