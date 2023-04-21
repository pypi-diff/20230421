# Comparing `tmp/cfgs-0.9.7.tar.gz` & `tmp/cfgs-0.9.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/cfgs-0.9.7.tar", last modified: Sat Feb 16 11:19:54 2019, max compression
+gzip compressed data, was "dist/cfgs-0.9.9.tar", last modified: Mon Apr  1 10:40:32 2019, max compression
```

## Comparing `cfgs-0.9.7.tar` & `cfgs-0.9.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2019-02-16 11:19:54.000000 cfgs-0.9.7/
-drwxr-xr-x   0 tom        (501) staff       (20)        0 2019-02-16 11:19:54.000000 cfgs-0.9.7/cfgs.egg-info/
--rw-r--r--   0 tom        (501) staff       (20)        1 2019-02-16 11:19:54.000000 cfgs-0.9.7/cfgs.egg-info/dependency_links.txt
--rw-r--r--   0 tom        (501) staff       (20)     5128 2019-02-16 11:19:54.000000 cfgs-0.9.7/cfgs.egg-info/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)      191 2019-02-16 11:19:54.000000 cfgs-0.9.7/cfgs.egg-info/SOURCES.txt
--rw-r--r--   0 tom        (501) staff       (20)        5 2019-02-16 11:19:54.000000 cfgs-0.9.7/cfgs.egg-info/top_level.txt
--rw-r--r--   0 tom        (501) staff       (20)    12144 2019-02-16 10:24:35.000000 cfgs-0.9.7/cfgs.py
--rw-r--r--   0 tom        (501) staff       (20)      209 2019-02-16 11:09:09.000000 cfgs-0.9.7/MANIFEST.in
--rw-r--r--   0 tom        (501) staff       (20)     5128 2019-02-16 11:19:54.000000 cfgs-0.9.7/PKG-INFO
--rw-r--r--   0 tom        (501) staff       (20)     3294 2019-02-16 10:18:54.000000 cfgs-0.9.7/README.rst
--rw-r--r--   0 tom        (501) staff       (20)      114 2019-02-16 11:19:54.000000 cfgs-0.9.7/setup.cfg
--rwxr-xr-x   0 tom        (501) staff       (20)     2506 2019-02-16 11:15:36.000000 cfgs-0.9.7/setup.py
--rw-r--r--   0 tom        (501) staff       (20)       39 2019-02-07 18:47:57.000000 cfgs-0.9.7/test_requirements.txt
--rw-r--r--   0 tom        (501) staff       (20)        6 2019-02-16 11:18:53.000000 cfgs-0.9.7/VERSION
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2019-04-01 10:40:32.000000 cfgs-0.9.9/
+drwxr-xr-x   0 tom        (501) staff       (20)        0 2019-04-01 10:40:32.000000 cfgs-0.9.9/cfgs.egg-info/
+-rw-r--r--   0 tom        (501) staff       (20)        1 2019-04-01 10:40:31.000000 cfgs-0.9.9/cfgs.egg-info/dependency_links.txt
+-rw-r--r--   0 tom        (501) staff       (20)     5153 2019-04-01 10:40:31.000000 cfgs-0.9.9/cfgs.egg-info/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)      191 2019-04-01 10:40:31.000000 cfgs-0.9.9/cfgs.egg-info/SOURCES.txt
+-rw-r--r--   0 tom        (501) staff       (20)        5 2019-04-01 10:40:31.000000 cfgs-0.9.9/cfgs.egg-info/top_level.txt
+-rw-r--r--   0 tom        (501) staff       (20)    12219 2019-04-01 10:33:41.000000 cfgs-0.9.9/cfgs.py
+-rw-r--r--   0 tom        (501) staff       (20)      209 2019-02-16 11:09:09.000000 cfgs-0.9.9/MANIFEST.in
+-rw-r--r--   0 tom        (501) staff       (20)     5153 2019-04-01 10:40:32.000000 cfgs-0.9.9/PKG-INFO
+-rw-r--r--   0 tom        (501) staff       (20)     3337 2019-02-17 11:45:14.000000 cfgs-0.9.9/README.rst
+-rw-r--r--   0 tom        (501) staff       (20)      114 2019-04-01 10:40:32.000000 cfgs-0.9.9/setup.cfg
+-rwxr-xr-x   0 tom        (501) staff       (20)     2480 2019-04-01 10:38:44.000000 cfgs-0.9.9/setup.py
+-rw-r--r--   0 tom        (501) staff       (20)       39 2019-02-07 18:47:57.000000 cfgs-0.9.9/test_requirements.txt
+-rw-r--r--   0 tom        (501) staff       (20)        6 2019-04-01 10:39:21.000000 cfgs-0.9.9/VERSION
```

### Comparing `cfgs-0.9.7/cfgs.egg-info/PKG-INFO` & `cfgs-0.9.9/cfgs.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: cfgs
-Version: 0.9.7
+Version: 0.9.9
 Summary: cfgs is a pure Python library for data and config files which implements the XDG standard for persistent files
-Home-page: http://github.com/timedata-org/cfgs
+Home-page: http://github.com/rec/cfgs
 Author: Tom Ritchford
 Author-email: tom@swirly.com
 License: MIT
-Download-URL: http://github.com/timedata-org/cfgs/archive/0.9.7.tar.gz
+Download-URL: http://github.com/rec/cfgs/archive/0.9.9.tar.gz
 Description: `cfgs`
         -------------
         
         Simple, correct handling of config, data and cache files
         ==================================================================
         
         Like everyone else, I wrote a lot of programs which saved config files
@@ -30,15 +30,15 @@
         It works on all versions of Python from 2.7 to 3.7, has complete test coverage,
         and all the functionality is reachable from a single class, ``cfgs.App``
         
         How it works in one sentence
         ===========================================
         
         Create a ``cfgs.App`` for your application, project, or script which
-        handles finding, reading and writing your data and config files and
+        handles finding, reading and writing your data and config files, and
         managing your cache directories.
         
         How to install
         =====================
         
         You can either use pip:
         
@@ -85,15 +85,15 @@
         
         .. code-block:: python
         
             import cfgs
             cache_size = 0x10000000
             app = cfgs.App('my-project')
             directory = app.cache.directory(cache_size=cache_size)
-        
+            # TODO: rewrite cache or add features.
         
         
         Using ``cfgs`` In legacy code
         =============================
         
         If you already have code to handle your config, data and cache files, then you
         can just use ``cgfs`` to get the
```

### Comparing `cfgs-0.9.7/cfgs.py` & `cfgs-0.9.9/cfgs.py`

 * *Files 0% similar despite different names*

```diff
@@ -142,14 +142,16 @@
              first try to guess the filename from the filename, then use
              `self.format`
         """
         if not filename:
             basename = os.path.basename(self.home)
             suffix = FORMAT_TO_SUFFIX[self.format.name]
             filename = '%s%s' % (basename, suffix)
+        elif filename.startswith('/'):
+            filename = filename[1:]
 
         return File(self.full_name(filename), self.format)
 
     def all_files(self, filename):
         """
         Yield all filenames matching the argument in either the home
         directory or any of the search directories
```

### Comparing `cfgs-0.9.7/PKG-INFO` & `cfgs-0.9.9/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,16 +1,16 @@
 Metadata-Version: 1.1
 Name: cfgs
-Version: 0.9.7
+Version: 0.9.9
 Summary: cfgs is a pure Python library for data and config files which implements the XDG standard for persistent files
-Home-page: http://github.com/timedata-org/cfgs
+Home-page: http://github.com/rec/cfgs
 Author: Tom Ritchford
 Author-email: tom@swirly.com
 License: MIT
-Download-URL: http://github.com/timedata-org/cfgs/archive/0.9.7.tar.gz
+Download-URL: http://github.com/rec/cfgs/archive/0.9.9.tar.gz
 Description: `cfgs`
         -------------
         
         Simple, correct handling of config, data and cache files
         ==================================================================
         
         Like everyone else, I wrote a lot of programs which saved config files
@@ -30,15 +30,15 @@
         It works on all versions of Python from 2.7 to 3.7, has complete test coverage,
         and all the functionality is reachable from a single class, ``cfgs.App``
         
         How it works in one sentence
         ===========================================
         
         Create a ``cfgs.App`` for your application, project, or script which
-        handles finding, reading and writing your data and config files and
+        handles finding, reading and writing your data and config files, and
         managing your cache directories.
         
         How to install
         =====================
         
         You can either use pip:
         
@@ -85,15 +85,15 @@
         
         .. code-block:: python
         
             import cfgs
             cache_size = 0x10000000
             app = cfgs.App('my-project')
             directory = app.cache.directory(cache_size=cache_size)
-        
+            # TODO: rewrite cache or add features.
         
         
         Using ``cfgs`` In legacy code
         =============================
         
         If you already have code to handle your config, data and cache files, then you
         can just use ``cgfs`` to get the
```

### Comparing `cfgs-0.9.7/README.rst` & `cfgs-0.9.9/README.rst`

 * *Files 2% similar despite different names*

```diff
@@ -21,15 +21,15 @@
 It works on all versions of Python from 2.7 to 3.7, has complete test coverage,
 and all the functionality is reachable from a single class, ``cfgs.App``
 
 How it works in one sentence
 ===========================================
 
 Create a ``cfgs.App`` for your application, project, or script which
-handles finding, reading and writing your data and config files and
+handles finding, reading and writing your data and config files, and
 managing your cache directories.
 
 How to install
 =====================
 
 You can either use pip:
 
@@ -76,15 +76,15 @@
 
 .. code-block:: python
 
     import cfgs
     cache_size = 0x10000000
     app = cfgs.App('my-project')
     directory = app.cache.directory(cache_size=cache_size)
-
+    # TODO: rewrite cache or add features.
 
 
 Using ``cfgs`` In legacy code
 =============================
 
 If you already have code to handle your config, data and cache files, then you
 can just use ``cgfs`` to get the
```

### Comparing `cfgs-0.9.7/setup.py` & `cfgs-0.9.9/setup.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-from setuptools import setup, find_packages
+from setuptools import setup
 from setuptools.command.test import test as TestCommand
 import os, sys
 
 
 # From here: http://pytest.org/2.2.4/goodpractises.html
 class RunTests(TestCommand):
     DIRECTORY = 'test'
@@ -35,27 +35,27 @@
         if coverage < fail_under:
             print('ERROR: coverage %.2f%% was less than fail_under=%s%%' % (
                   coverage, fail_under))
             raise SystemExit(1)
 
 
 NAME = 'cfgs'
-OWNER = 'timedata-org'
+OWNER = 'rec'
 FILENAME = os.path.join(os.path.dirname(__file__), 'VERSION')
 VERSION = open(FILENAME).read().strip()
 
 URL = 'http://github.com/{OWNER}/{NAME}'.format(**locals())
 DOWNLOAD_URL = '{URL}/archive/{VERSION}.tar.gz'.format(**locals())
 
 with open('test_requirements.txt') as f:
     TESTS_REQUIRE = f.read().splitlines()
 
 
 setup(
-    name='cfgs',
+    name=NAME,
     version=open('VERSION').read().strip(),
     description=(
         'cfgs is a pure Python library for data and config files which '
         'implements the XDG standard for persistent files'),
     long_description=open('README.rst').read(),
     author='Tom Ritchford',
     author_email='tom@swirly.com',
```

