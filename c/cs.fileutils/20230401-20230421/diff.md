# Comparing `tmp/cs.fileutils-20230401.tar.gz` & `tmp/cs.fileutils-20230421.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "cs.fileutils-20230401.tar", last modified: Sat Apr  1 05:09:57 2023, max compression
+gzip compressed data, was "cs.fileutils-20230421.tar", last modified: Fri Apr 21 03:55:44 2023, max compression
```

## Comparing `cs.fileutils-20230401.tar` & `cs.fileutils-20230421.tar`

### file list

```diff
@@ -1,17 +1,17 @@
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:09:57.355757 cs.fileutils-20230401/
--rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-04-01 05:09:20.000000 cs.fileutils-20230401/MANIFEST.in
--rw-rw-r--   0 cameron    (501) cameron    (502)    26112 2023-04-01 05:09:57.355931 cs.fileutils-20230401/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)    29151 2023-04-01 05:09:27.000000 cs.fileutils-20230401/README.md
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:09:57.351242 cs.fileutils-20230401/lib/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:09:57.351571 cs.fileutils-20230401/lib/python/
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:09:57.353605 cs.fileutils-20230401/lib/python/cs/
--rw-r--r--   0 cameron    (501) cameron    (502)    58169 2023-04-01 05:09:10.000000 cs.fileutils-20230401/lib/python/cs/fileutils.py
-drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-01 05:09:57.355466 cs.fileutils-20230401/lib/python/cs.fileutils.egg-info/
--rw-rw-r--   0 cameron    (501) cameron    (502)    26112 2023-04-01 05:09:57.000000 cs.fileutils-20230401/lib/python/cs.fileutils.egg-info/PKG-INFO
--rw-rw-r--   0 cameron    (501) cameron    (502)      316 2023-04-01 05:09:57.000000 cs.fileutils-20230401/lib/python/cs.fileutils.egg-info/SOURCES.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-04-01 05:09:57.000000 cs.fileutils-20230401/lib/python/cs.fileutils.egg-info/dependency_links.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)      263 2023-04-01 05:09:57.000000 cs.fileutils-20230401/lib/python/cs.fileutils.egg-info/requires.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-04-01 05:09:57.000000 cs.fileutils-20230401/lib/python/cs.fileutils.egg-info/top_level.txt
--rw-rw-r--   0 cameron    (501) cameron    (502)    26625 2023-04-01 05:09:49.000000 cs.fileutils-20230401/pyproject.toml
--rw-rw-r--   0 cameron    (501) cameron    (502)     1153 2023-04-01 05:09:57.356577 cs.fileutils-20230401/setup.cfg
--rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-04-01 05:09:27.000000 cs.fileutils-20230401/setup.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-21 03:55:44.172735 cs.fileutils-20230421/
+-rw-rw-r--   0 cameron    (501) cameron    (502)       18 2023-04-21 03:54:54.000000 cs.fileutils-20230421/MANIFEST.in
+-rw-rw-r--   0 cameron    (501) cameron    (502)    26284 2023-04-21 03:55:44.172907 cs.fileutils-20230421/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)    29309 2023-04-21 03:55:03.000000 cs.fileutils-20230421/README.md
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-21 03:55:44.167464 cs.fileutils-20230421/lib/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-21 03:55:44.167808 cs.fileutils-20230421/lib/python/
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-21 03:55:44.169879 cs.fileutils-20230421/lib/python/cs/
+-rw-r--r--   0 cameron    (501) cameron    (502)    58176 2023-04-21 03:54:27.000000 cs.fileutils-20230421/lib/python/cs/fileutils.py
+drwxrwxr-x   0 cameron    (501) cameron    (502)        0 2023-04-21 03:55:44.172435 cs.fileutils-20230421/lib/python/cs.fileutils.egg-info/
+-rw-rw-r--   0 cameron    (501) cameron    (502)    26284 2023-04-21 03:55:44.000000 cs.fileutils-20230421/lib/python/cs.fileutils.egg-info/PKG-INFO
+-rw-rw-r--   0 cameron    (501) cameron    (502)      316 2023-04-21 03:55:44.000000 cs.fileutils-20230421/lib/python/cs.fileutils.egg-info/SOURCES.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        1 2023-04-21 03:55:44.000000 cs.fileutils-20230421/lib/python/cs.fileutils.egg-info/dependency_links.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)      263 2023-04-21 03:55:44.000000 cs.fileutils-20230421/lib/python/cs.fileutils.egg-info/requires.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)        3 2023-04-21 03:55:44.000000 cs.fileutils-20230421/lib/python/cs.fileutils.egg-info/top_level.txt
+-rw-rw-r--   0 cameron    (501) cameron    (502)    26797 2023-04-21 03:55:30.000000 cs.fileutils-20230421/pyproject.toml
+-rw-rw-r--   0 cameron    (501) cameron    (502)     1153 2023-04-21 03:55:44.173643 cs.fileutils-20230421/setup.cfg
+-rw-rw-r--   0 cameron    (501) cameron    (502)       59 2023-04-21 03:55:03.000000 cs.fileutils-20230421/setup.py
```

### Comparing `cs.fileutils-20230401/PKG-INFO` & `cs.fileutils-20230421/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fileutils
-Version: 20230401
+Version: 20230421
 Summary: My grab bag of convenience functions for files and filenames/pathnames.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -16,16 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 My grab bag of convenience functions for files and filenames/pathnames.
 
-*Latest release 20230401*:
-Replaced a lot of runstate plumbing with @uses_runstate.
+*Latest release 20230421*:
+atomic_filename: raise FileExistsError instead of ValueError if not exists_ok and existspath(filename).
 
 ## Function `abspath_from_file(path, from_file)`
 
 Return the absolute path of `path` with respect to `from_file`,
 as one might do for an include file.
 
 ## Function `atomic_filename(filename, exists_ok=False, placeholder=False, dir=None, prefix=None, suffix=None, **kw)`
@@ -600,14 +600,17 @@
 A `saferename()` that returns `True` on success,
 `False` on failure.
 
 # Release Log
 
 
 
+*Release 20230421*:
+atomic_filename: raise FileExistsError instead of ValueError if not exists_ok and existspath(filename).
+
 *Release 20230401*:
 Replaced a lot of runstate plumbing with @uses_runstate.
 
 *Release 20221118*:
 atomic_filename: use shutil.copystat instead of shutil.copymode, bugfix the associated logic.
 
 *Release 20220429*:
```

### Comparing `cs.fileutils-20230401/README.md` & `cs.fileutils-20230421/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,11 @@
 My grab bag of convenience functions for files and filenames/pathnames.
 
-*Latest release 20230401*:
-Replaced a lot of runstate plumbing with @uses_runstate.
+*Latest release 20230421*:
+atomic_filename: raise FileExistsError instead of ValueError if not exists_ok and existspath(filename).
 
 ## Function `abspath_from_file(path, from_file)`
 
 Return the absolute path of `path` with respect to `from_file`,
 as one might do for an include file.
 
 ## Function `atomic_filename(filename, exists_ok=False, placeholder=False, dir=None, prefix=None, suffix=None, **kw)`
@@ -494,15 +494,15 @@
 
 *Property `Pathname.isabs`*:
 Whether this Pathname is an absolute Pathname.
 
 *Property `Pathname.short`*:
 The shortened form of this Pathname.
 
-*Method `Pathname.shorten(self, environ=None, prefixes=None)`*:
+*Method `Pathname.shorten(self, prefixes=None)`*:
 Shorten a Pathname using ~ and ~user.
 
 ## Function `poll_file(path, old_state, reload_file, missing_ok=False)`
 
 Watch a file for modification by polling its state as obtained
 by `FileState()`.
 Call `reload_file(path)` if the state changes.
@@ -703,14 +703,17 @@
 A `saferename()` that returns `True` on success,
 `False` on failure.
 
 # Release Log
 
 
 
+*Release 20230421*:
+atomic_filename: raise FileExistsError instead of ValueError if not exists_ok and existspath(filename).
+
 *Release 20230401*:
 Replaced a lot of runstate plumbing with @uses_runstate.
 
 *Release 20221118*:
 atomic_filename: use shutil.copystat instead of shutil.copymode, bugfix the associated logic.
 
 *Release 20220429*:
```

### Comparing `cs.fileutils-20230401/lib/python/cs/fileutils.py` & `cs.fileutils-20230421/lib/python/cs/fileutils.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,27 +35,27 @@
 from tempfile import TemporaryFile, NamedTemporaryFile, mkstemp
 from threading import Lock, RLock
 import time
 from cs.buffer import CornuCopyBuffer
 from cs.deco import cachedmethod, decorator, fmtdoc, strable
 from cs.filestate import FileState
 from cs.fs import shortpath
-from cs.gimmicks import TimeoutError
+from cs.gimmicks import TimeoutError  # pylint: disable=redefined-builtin
 from cs.lex import as_lines, cutsuffix, common_prefix
 from cs.logutils import error, warning, debug
 from cs.pfx import Pfx, pfx, pfx_call
 from cs.progress import Progress, progressbar
 from cs.py3 import ustr, bytes, pread  # pylint: disable=redefined-builtin
 from cs.range import Range
 from cs.resources import uses_runstate
 from cs.result import CancellationError
 from cs.threads import locked
 from cs.units import BINARY_BYTES_SCALE
 
-__version__ = '20230401'
+__version__ = '20230421'
 
 DISTINFO = {
     'keywords': ["python2", "python3"],
     'classifiers': [
         "Programming Language :: Python",
         "Programming Language :: Python :: 2",
         "Programming Language :: Python :: 3",
@@ -790,29 +790,29 @@
     if path.endswith(os.sep):
       if sep:
         raise ValueError(
             "mkdirn(path=%r, sep=%r): using non-empty sep"
             " with a trailing %r seems nonsensical" % (path, sep, os.sep)
         )
       dirpath = path[:-len(os.sep)]
-      pfx = ''
+      prefix = ''
     else:
       dirpath = dirname(path)
       if not dirpath:
         dirpath = '.'
-      pfx = basename(path) + sep
+      prefix = basename(path) + sep
 
     if not isdir(dirpath):
       error("parent not a directory: %r", dirpath)
       return None
 
     # do a quick scan of the directory to find
     # if any names of the desired form already exist
     # in order to start after them
-    maxn = max_suffix(dirpath, pfx)
+    maxn = max_suffix(dirpath, prefix)
     if maxn is None:
       newn = 0
     else:
       newn = maxn
 
     while True:
       newn += 1
@@ -996,18 +996,18 @@
 
   @property
   def short(self):
     ''' The shortened form of this Pathname.
     '''
     return self.shorten()
 
-  def shorten(self, environ=None, prefixes=None):
+  def shorten(self, prefixes=None):
     ''' Shorten a Pathname using ~ and ~user.
     '''
-    return shortpath(self, environ=environ, prefixes=prefixes)
+    return shortpath(self, prefixes=prefixes)
 
 def iter_fd(fd, **kw):
   ''' Iterate over data from the file descriptor `fd`.
   '''
   for bs in CornuCopyBuffer.from_fd(fd, **kw):
     yield bs
 
@@ -1197,17 +1197,15 @@
     bfr = getattr(self, '_reading_bfr', None)
     if offset is None:
       if bfr is None:
         offset = self.tell()
       else:
         offset = bfr.offset
     if size == -1:
-      size = len(self) - offset
-      if size < 0:
-        size = 0
+      size = max(len(self) - offset, 0)
     if size == 0:
       return b''
     if longread:
       bss = []
     while size > 0:
       with self._lock:
         # We need to retest on each iteration because other reads
@@ -1686,16 +1684,16 @@
   if dir is None:
     dir = dirname(filename)
   fprefix, fsuffix = splitext(basename(filename))
   if prefix is None:
     prefix = '.' + fprefix
   if suffix is None:
     suffix = fsuffix
-  if existspath(filename) and not exists_ok:
-    raise ValueError("already exists: %r" % (filename,))
+  if not exists_ok and existspath(filename):
+    raise FileExistsError(errno.EEXIST, os.strerror(errno.EEXIST), filename)
   with NamedTemporaryFile(dir=dir, prefix=prefix, suffix=suffix, delete=False,
                           **kw) as T:
     if placeholder:
       # create a placeholder file
       with open(filename, 'ab' if exists_ok else 'xb'):
         pass
     yield T
```

### Comparing `cs.fileutils-20230401/lib/python/cs.fileutils.egg-info/PKG-INFO` & `cs.fileutils-20230421/lib/python/cs.fileutils.egg-info/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: cs.fileutils
-Version: 20230401
+Version: 20230421
 Summary: My grab bag of convenience functions for files and filenames/pathnames.
 Home-page: https://bitbucket.org/cameron_simpson/css/commits/all
 Author: Cameron Simpson
 Author-email: Cameron Simpson <cs@cskk.id.au>
 License: GNU General Public License v3 or later (GPLv3+)
 Project-URL: URL, https://bitbucket.org/cameron_simpson/css/commits/all
 Keywords: python2,python3
@@ -16,16 +16,16 @@
 Classifier: Operating System :: OS Independent
 Classifier: Topic :: Software Development :: Libraries :: Python Modules
 Classifier: License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)
 Description-Content-Type: text/markdown
 
 My grab bag of convenience functions for files and filenames/pathnames.
 
-*Latest release 20230401*:
-Replaced a lot of runstate plumbing with @uses_runstate.
+*Latest release 20230421*:
+atomic_filename: raise FileExistsError instead of ValueError if not exists_ok and existspath(filename).
 
 ## Function `abspath_from_file(path, from_file)`
 
 Return the absolute path of `path` with respect to `from_file`,
 as one might do for an include file.
 
 ## Function `atomic_filename(filename, exists_ok=False, placeholder=False, dir=None, prefix=None, suffix=None, **kw)`
@@ -600,14 +600,17 @@
 A `saferename()` that returns `True` on success,
 `False` on failure.
 
 # Release Log
 
 
 
+*Release 20230421*:
+atomic_filename: raise FileExistsError instead of ValueError if not exists_ok and existspath(filename).
+
 *Release 20230401*:
 Replaced a lot of runstate plumbing with @uses_runstate.
 
 *Release 20221118*:
 atomic_filename: use shutil.copystat instead of shutil.copymode, bugfix the associated logic.
 
 *Release 20220429*:
```

### Comparing `cs.fileutils-20230401/pyproject.toml` & `cs.fileutils-20230421/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -30,28 +30,28 @@
     "Programming Language :: Python :: 3",
     "Development Status :: 4 - Beta",
     "Intended Audience :: Developers",
     "Operating System :: OS Independent",
     "Topic :: Software Development :: Libraries :: Python Modules",
     "License :: OSI Approved :: GNU General Public License v3 or later (GPLv3+)",
 ]
-version = "20230401"
+version = "20230421"
 
 [project.license]
 text = "GNU General Public License v3 or later (GPLv3+)"
 
 [project.urls]
 URL = "https://bitbucket.org/cameron_simpson/css/commits/all"
 
 [project.readme]
 text = """
 My grab bag of convenience functions for files and filenames/pathnames.
 
-*Latest release 20230401*:
-Replaced a lot of runstate plumbing with @uses_runstate.
+*Latest release 20230421*:
+atomic_filename: raise FileExistsError instead of ValueError if not exists_ok and existspath(filename).
 
 ## Function `abspath_from_file(path, from_file)`
 
 Return the absolute path of `path` with respect to `from_file`,
 as one might do for an include file.
 
 ## Function `atomic_filename(filename, exists_ok=False, placeholder=False, dir=None, prefix=None, suffix=None, **kw)`
@@ -626,14 +626,17 @@
 A `saferename()` that returns `True` on success,
 `False` on failure.
 
 # Release Log
 
 
 
+*Release 20230421*:
+atomic_filename: raise FileExistsError instead of ValueError if not exists_ok and existspath(filename).
+
 *Release 20230401*:
 Replaced a lot of runstate plumbing with @uses_runstate.
 
 *Release 20221118*:
 atomic_filename: use shutil.copystat instead of shutil.copymode, bugfix the associated logic.
 
 *Release 20220429*:
```

### Comparing `cs.fileutils-20230401/setup.cfg` & `cs.fileutils-20230421/setup.cfg`

 * *Files 9% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [metadata]
 name = cs.fileutils
-version = 20230401
+version = 20230421
 author = Cameron Simpson
 author_email = cs@cskk.id.au
 license = GNU General Public License v3 or later (GPLv3+)
 description = My grab bag of convenience functions for files and filenames/pathnames.
 keywords = python2, python3
 url = https://bitbucket.org/cameron_simpson/css/commits/all
 classifiers =
```

