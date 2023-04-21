# Comparing `tmp/gris-0.6.1.tar.gz` & `tmp/gris-0.7.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/gris-0.6.1.tar", last modified: Sat Oct  5 23:16:14 2019, max compression
+gzip compressed data, was "gris-0.7.0.tar", last modified: Fri Apr 21 01:13:54 2023, max compression
```

## Comparing `gris-0.6.1.tar` & `gris-0.7.0.tar`

### file list

```diff
@@ -1,15 +1,13 @@
-drwxr-xr-x   0 bootes     (501) staff       (20)        0 2019-10-05 23:16:14.000000 gris-0.6.1/
--rw-r--r--   0 bootes     (501) staff       (20)    18092 2017-09-19 03:16:44.000000 gris-0.6.1/LICENSE.txt
--rw-r--r--   0 bootes     (501) staff       (20)       27 2019-10-05 17:51:42.000000 gris-0.6.1/MANIFEST.in
--rw-r--r--   0 bootes     (501) staff       (20)     1191 2019-10-05 23:16:14.000000 gris-0.6.1/PKG-INFO
--rw-r--r--   0 bootes     (501) staff       (20)      450 2019-10-05 17:25:37.000000 gris-0.6.1/README.md
-drwxr-xr-x   0 bootes     (501) staff       (20)        0 2019-10-05 23:16:14.000000 gris-0.6.1/gris/
--rw-r--r--   0 bootes     (501) staff       (20)       20 2019-10-05 23:12:28.000000 gris-0.6.1/gris/__init__.py
--rw-r--r--   0 bootes     (501) staff       (20)    10150 2019-10-05 22:52:02.000000 gris-0.6.1/gris/gris.py
-drwxr-xr-x   0 bootes     (501) staff       (20)        0 2019-10-05 23:16:14.000000 gris-0.6.1/gris.egg-info/
--rw-r--r--   0 bootes     (501) staff       (20)     1191 2019-10-05 23:16:14.000000 gris-0.6.1/gris.egg-info/PKG-INFO
--rw-r--r--   0 bootes     (501) staff       (20)      184 2019-10-05 23:16:14.000000 gris-0.6.1/gris.egg-info/SOURCES.txt
--rw-r--r--   0 bootes     (501) staff       (20)        1 2019-10-05 23:16:14.000000 gris-0.6.1/gris.egg-info/dependency_links.txt
--rw-r--r--   0 bootes     (501) staff       (20)        5 2019-10-05 23:16:14.000000 gris-0.6.1/gris.egg-info/top_level.txt
--rw-r--r--   0 bootes     (501) staff       (20)       38 2019-10-05 23:16:14.000000 gris-0.6.1/setup.cfg
--rw-r--r--   0 bootes     (501) staff       (20)     1075 2019-10-05 22:52:07.000000 gris-0.6.1/setup.py
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 01:13:54.528541 gris-0.7.0/
+-rw-r--r--   0 anglyan    (502) staff       (20)    18092 2023-04-21 00:57:42.000000 gris-0.7.0/LICENSE.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)       27 2023-04-21 00:57:42.000000 gris-0.7.0/MANIFEST.in
+-rw-r--r--   0 anglyan    (502) staff       (20)     1382 2023-04-21 01:13:54.528408 gris-0.7.0/PKG-INFO
+-rw-r--r--   0 anglyan    (502) staff       (20)      648 2023-04-21 01:09:14.000000 gris-0.7.0/README.md
+drwxr-xr-x   0 anglyan    (502) staff       (20)        0 2023-04-21 01:13:54.528251 gris-0.7.0/gris.egg-info/
+-rw-r--r--   0 anglyan    (502) staff       (20)     1382 2023-04-21 01:13:54.000000 gris-0.7.0/gris.egg-info/PKG-INFO
+-rw-r--r--   0 anglyan    (502) staff       (20)      169 2023-04-21 01:13:54.000000 gris-0.7.0/gris.egg-info/SOURCES.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)        1 2023-04-21 01:13:54.000000 gris-0.7.0/gris.egg-info/dependency_links.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)        1 2023-04-21 01:13:54.000000 gris-0.7.0/gris.egg-info/top_level.txt
+-rw-r--r--   0 anglyan    (502) staff       (20)      689 2023-04-21 01:06:52.000000 gris-0.7.0/pyproject.toml
+-rw-r--r--   0 anglyan    (502) staff       (20)       38 2023-04-21 01:13:54.528576 gris-0.7.0/setup.cfg
+-rw-r--r--   0 anglyan    (502) staff       (20)     1075 2023-04-21 01:07:39.000000 gris-0.7.0/setup.py
```

### filetype from file(1)

```diff
@@ -1 +1 @@
-POSIX tar archive (GNU)
+POSIX tar archive
```

### Comparing `gris-0.6.1/LICENSE.txt` & `gris-0.7.0/LICENSE.txt`

 * *Files identical despite different names*

### Comparing `gris-0.6.1/PKG-INFO` & `gris-0.7.0/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 Metadata-Version: 2.1
 Name: gris
-Version: 0.6.1
-Summary: parser of RIS and WOK bibliography file format
+Version: 0.7.0
+Summary: Parser of RIS file format
 Home-page: https://github.com/anglyan/gris.git
 Author: Angel Yanguas-Gil
 Author-email: angel.yanguas@gmail.com
-License: UNKNOWN
-Description: README
-        ======
-        
-        About gris
-        ----------
-        
-        gris is a minimalistic tool to read, parse, and
-        write reference data in
-        [Refman RIS format](https://en.wikipedia.org/wiki/RIS_(file_format)).
-        
-        RIS format codifies bibliographic data using a series of tags. There
-        are two different standards: the RIS output by
-        Web of Knowledge and the original standard is used by other
-        providers. This module supports both.
-        
-        This module has been updated and tested in Python 3.7
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Project-URL: Homepage, https://github.com/anglyan/gris.git
+Keywords: RIS file format,RefMan RIS,bibliography,parser
 Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Topic :: Utilities
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+README
+======
+
+About gris
+----------
+
+gris is a minimalistic tool to read, parse, and
+write reference data in
+[Refman RIS format](https://en.wikipedia.org/wiki/RIS_(file_format)).
+
+RIS format codifies bibliographic data using a series of tags. There
+are two different standards: the RIS output by
+Web of Knowledge and the original standard is used by other
+providers. This module supports both.
+
+This module has been updated and tested in Python 3.7
+
+License
+-------
+Copyright (C) 2013 Angel Yanguas-Gil
+
+This program is free software, licensed under GPLv2 or later.
+A copy of the GPLv2 license is provided in the root directory of the source code.
```

### Comparing `gris-0.6.1/gris.egg-info/PKG-INFO` & `gris-0.7.0/gris.egg-info/PKG-INFO`

 * *Files 20% similar despite different names*

```diff
@@ -1,34 +1,43 @@
 Metadata-Version: 2.1
 Name: gris
-Version: 0.6.1
-Summary: parser of RIS and WOK bibliography file format
+Version: 0.7.0
+Summary: Parser of RIS file format
 Home-page: https://github.com/anglyan/gris.git
 Author: Angel Yanguas-Gil
 Author-email: angel.yanguas@gmail.com
-License: UNKNOWN
-Description: README
-        ======
-        
-        About gris
-        ----------
-        
-        gris is a minimalistic tool to read, parse, and
-        write reference data in
-        [Refman RIS format](https://en.wikipedia.org/wiki/RIS_(file_format)).
-        
-        RIS format codifies bibliographic data using a series of tags. There
-        are two different standards: the RIS output by
-        Web of Knowledge and the original standard is used by other
-        providers. This module supports both.
-        
-        This module has been updated and tested in Python 3.7
-        
-Platform: UNKNOWN
-Classifier: Development Status :: 4 - Beta
+Project-URL: Homepage, https://github.com/anglyan/gris.git
+Keywords: RIS file format,RefMan RIS,bibliography,parser
 Classifier: Programming Language :: Python :: 3
+Classifier: Development Status :: 4 - Beta
+Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
+Classifier: Operating System :: OS Independent
 Classifier: Environment :: Console
 Classifier: Topic :: Scientific/Engineering
-Classifier: License :: OSI Approved :: GNU General Public License v2 or later (GPLv2+)
 Classifier: Topic :: Utilities
 Requires-Python: >=3
 Description-Content-Type: text/markdown
+License-File: LICENSE.txt
+
+README
+======
+
+About gris
+----------
+
+gris is a minimalistic tool to read, parse, and
+write reference data in
+[Refman RIS format](https://en.wikipedia.org/wiki/RIS_(file_format)).
+
+RIS format codifies bibliographic data using a series of tags. There
+are two different standards: the RIS output by
+Web of Knowledge and the original standard is used by other
+providers. This module supports both.
+
+This module has been updated and tested in Python 3.7
+
+License
+-------
+Copyright (C) 2013 Angel Yanguas-Gil
+
+This program is free software, licensed under GPLv2 or later.
+A copy of the GPLv2 license is provided in the root directory of the source code.
```

### Comparing `gris-0.6.1/setup.py` & `gris-0.7.0/setup.py`

 * *Files 8% similar despite different names*

```diff
@@ -8,15 +8,15 @@
 
 here = path.abspath(path.dirname(__file__))
 with open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(name = 'gris',
     description = "parser of RIS and WOK bibliography file format",
-    version = '0.6.1',
+    version = '0.7.0',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author = "Angel Yanguas-Gil",
     author_email = "angel.yanguas@gmail.com",
     url = "https://github.com/anglyan/gris.git",
     packages=find_packages(),
     python_requires=">=3",
```

