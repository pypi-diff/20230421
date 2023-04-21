# Comparing `tmp/shellfish-0.3.1.tar.gz` & `tmp/shellfish-0.3.2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "shellfish-0.3.1.tar", max compression
+gzip compressed data, was "shellfish-0.3.2.tar", max compression
```

## Comparing `shellfish-0.3.1.tar` & `shellfish-0.3.2.tar`

### file list

```diff
@@ -1,36 +1,36 @@
--rw-r--r--   0        0        0     2275 2023-04-20 23:19:53.924845 shellfish-0.3.1/pyproject.toml
--rw-r--r--   0        0        0     1003 2022-09-19 18:35:16.987296 shellfish-0.3.1/README.md
--rw-r--r--   0        0        0      295 2023-04-20 23:19:54.396173 shellfish-0.3.1/shellfish/__about__.py
--rw-r--r--   0        0        0     1148 2023-04-20 20:51:48.622821 shellfish-0.3.1/shellfish/__init__.py
--rw-r--r--   0        0        0      483 2023-04-20 20:51:48.622563 shellfish-0.3.1/shellfish/__main__.py
--rw-r--r--   0        0        0      358 2023-04-20 20:38:23.592387 shellfish-0.3.1/shellfish/_meta.py
--rw-r--r--   0        0        0      866 2023-04-19 19:17:33.733686 shellfish-0.3.1/shellfish/_types.py
--rw-r--r--   0        0        0     3278 2023-04-19 19:17:33.734686 shellfish-0.3.1/shellfish/aios/__init__.py
--rw-r--r--   0        0        0      640 2023-04-19 19:16:52.950595 shellfish-0.3.1/shellfish/aios/_path.py
--rw-r--r--   0        0        0     7251 2023-04-19 19:17:33.734686 shellfish-0.3.1/shellfish/batman.py
--rw-r--r--   0        0        0      295 2022-02-17 22:17:07.429546 shellfish-0.3.1/shellfish/const.py
--rw-r--r--   0        0        0       49 2022-02-04 21:32:32.211842 shellfish-0.3.1/shellfish/dev/__init__.py
--rw-r--r--   0        0        0     1439 2023-04-19 19:17:33.735685 shellfish-0.3.1/shellfish/dev/do.py
--rw-r--r--   0        0        0     3456 2023-04-19 19:17:33.735685 shellfish-0.3.1/shellfish/dev/popen_gen.py
--rw-r--r--   0        0        0     7941 2023-04-19 19:17:33.736685 shellfish-0.3.1/shellfish/dev/run_async.py
--rw-r--r--   0        0        0     4265 2023-04-11 22:29:27.086800 shellfish-0.3.1/shellfish/dotenv.py
--rw-r--r--   0        0        0      664 2023-03-31 17:46:06.868732 shellfish-0.3.1/shellfish/echo.py
--rw-r--r--   0        0        0     7924 2023-04-19 19:17:33.736685 shellfish-0.3.1/shellfish/exe.py
--rw-r--r--   0        0        0    54264 2023-04-20 20:51:48.652243 shellfish-0.3.1/shellfish/fs/__init__.py
--rw-r--r--   0        0        0    15169 2023-04-19 19:17:33.738722 shellfish-0.3.1/shellfish/fs/_async.py
--rw-r--r--   0        0        0     1534 2023-02-24 22:45:12.450622 shellfish-0.3.1/shellfish/fs/promises.py
--rw-r--r--   0        0        0     1917 2023-04-19 19:17:33.738722 shellfish-0.3.1/shellfish/libhash.py
--rw-r--r--   0        0        0       50 2023-02-09 22:42:06.315587 shellfish-0.3.1/shellfish/libsh/__init__.py
--rw-r--r--   0        0        0     3655 2023-04-19 19:17:33.739722 shellfish-0.3.1/shellfish/libsh/_dirtree.py
--rw-r--r--   0        0        0     1872 2023-04-19 19:17:33.739722 shellfish-0.3.1/shellfish/libsh/args.py
--rw-r--r--   0        0        0    10653 2023-04-19 19:17:33.739722 shellfish-0.3.1/shellfish/osfs.py
--rw-r--r--   0        0        0     7266 2023-04-19 19:17:33.740721 shellfish-0.3.1/shellfish/process.py
--rw-r--r--   0        0        0      308 2023-03-24 22:14:11.926875 shellfish-0.3.1/shellfish/psu.py
--rw-r--r--   0        0        0        0 2022-02-01 22:06:04.844951 shellfish-0.3.1/shellfish/py.typed
--rw-r--r--   0        0        0    63208 2023-04-20 20:51:48.644235 shellfish-0.3.1/shellfish/sh.py
--rw-r--r--   0        0        0     8275 2023-04-19 19:17:33.741721 shellfish-0.3.1/shellfish/sp.py
--rw-r--r--   0        0        0      228 2023-04-19 19:17:33.741721 shellfish-0.3.1/shellfish/stdio.py
--rw-r--r--   0        0        0     2617 2023-04-11 22:29:27.086800 shellfish-0.3.1/shellfish/testing.py
--rw-r--r--   0        0        0       27 2023-04-19 19:17:33.742721 shellfish-0.3.1/shellfish/tests/__init__.py
--rw-r--r--   0        0        0     2814 2023-04-19 19:17:33.742721 shellfish-0.3.1/shellfish/tests/test_fs.py
--rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 shellfish-0.3.1/PKG-INFO
+-rw-r--r--   0        0        0     2275 2023-04-21 00:18:13.195085 shellfish-0.3.2/pyproject.toml
+-rw-r--r--   0        0        0     1003 2022-09-19 18:35:16.987296 shellfish-0.3.2/README.md
+-rw-r--r--   0        0        0      295 2023-04-21 00:18:13.195085 shellfish-0.3.2/shellfish/__about__.py
+-rw-r--r--   0        0        0     1148 2023-04-21 00:04:53.526032 shellfish-0.3.2/shellfish/__init__.py
+-rw-r--r--   0        0        0      483 2023-04-21 00:04:53.526032 shellfish-0.3.2/shellfish/__main__.py
+-rw-r--r--   0        0        0      358 2023-04-21 00:04:53.526032 shellfish-0.3.2/shellfish/_meta.py
+-rw-r--r--   0        0        0      866 2023-04-19 19:17:33.733686 shellfish-0.3.2/shellfish/_types.py
+-rw-r--r--   0        0        0     3278 2023-04-19 19:17:33.734686 shellfish-0.3.2/shellfish/aios/__init__.py
+-rw-r--r--   0        0        0      640 2023-04-19 19:16:52.950595 shellfish-0.3.2/shellfish/aios/_path.py
+-rw-r--r--   0        0        0     7251 2023-04-19 19:17:33.734686 shellfish-0.3.2/shellfish/batman.py
+-rw-r--r--   0        0        0      295 2022-02-17 22:17:07.429546 shellfish-0.3.2/shellfish/const.py
+-rw-r--r--   0        0        0       49 2022-02-04 21:32:32.211842 shellfish-0.3.2/shellfish/dev/__init__.py
+-rw-r--r--   0        0        0     1439 2023-04-19 19:17:33.735685 shellfish-0.3.2/shellfish/dev/do.py
+-rw-r--r--   0        0        0     3456 2023-04-19 19:17:33.735685 shellfish-0.3.2/shellfish/dev/popen_gen.py
+-rw-r--r--   0        0        0     7941 2023-04-19 19:17:33.736685 shellfish-0.3.2/shellfish/dev/run_async.py
+-rw-r--r--   0        0        0     4265 2023-04-11 22:29:27.086800 shellfish-0.3.2/shellfish/dotenv.py
+-rw-r--r--   0        0        0      664 2023-03-31 17:46:06.868732 shellfish-0.3.2/shellfish/echo.py
+-rw-r--r--   0        0        0     7924 2023-04-19 19:17:33.736685 shellfish-0.3.2/shellfish/exe.py
+-rw-r--r--   0        0        0    54196 2023-04-21 00:18:13.196068 shellfish-0.3.2/shellfish/fs/__init__.py
+-rw-r--r--   0        0        0    15169 2023-04-19 19:17:33.738722 shellfish-0.3.2/shellfish/fs/_async.py
+-rw-r--r--   0        0        0     1534 2023-02-24 22:45:12.450622 shellfish-0.3.2/shellfish/fs/promises.py
+-rw-r--r--   0        0        0     1917 2023-04-19 19:17:33.738722 shellfish-0.3.2/shellfish/libhash.py
+-rw-r--r--   0        0        0       50 2023-02-09 22:42:06.315587 shellfish-0.3.2/shellfish/libsh/__init__.py
+-rw-r--r--   0        0        0     3655 2023-04-19 19:17:33.739722 shellfish-0.3.2/shellfish/libsh/_dirtree.py
+-rw-r--r--   0        0        0     1872 2023-04-19 19:17:33.739722 shellfish-0.3.2/shellfish/libsh/args.py
+-rw-r--r--   0        0        0    10653 2023-04-19 19:17:33.739722 shellfish-0.3.2/shellfish/osfs.py
+-rw-r--r--   0        0        0     7266 2023-04-19 19:17:33.740721 shellfish-0.3.2/shellfish/process.py
+-rw-r--r--   0        0        0      308 2023-03-24 22:14:11.926875 shellfish-0.3.2/shellfish/psu.py
+-rw-r--r--   0        0        0        0 2022-02-01 22:06:04.844951 shellfish-0.3.2/shellfish/py.typed
+-rw-r--r--   0        0        0    63208 2023-04-21 00:04:53.526032 shellfish-0.3.2/shellfish/sh.py
+-rw-r--r--   0        0        0     8275 2023-04-19 19:17:33.741721 shellfish-0.3.2/shellfish/sp.py
+-rw-r--r--   0        0        0      228 2023-04-19 19:17:33.741721 shellfish-0.3.2/shellfish/stdio.py
+-rw-r--r--   0        0        0     2617 2023-04-11 22:29:27.086800 shellfish-0.3.2/shellfish/testing.py
+-rw-r--r--   0        0        0       27 2023-04-19 19:17:33.742721 shellfish-0.3.2/shellfish/tests/__init__.py
+-rw-r--r--   0        0        0     2814 2023-04-19 19:17:33.742721 shellfish-0.3.2/shellfish/tests/test_fs.py
+-rw-r--r--   0        0        0     2404 1970-01-01 00:00:00.000000 shellfish-0.3.2/PKG-INFO
```

### Comparing `shellfish-0.3.1/pyproject.toml` & `shellfish-0.3.2/pyproject.toml`

 * *Files 0% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "shellfish"
-version = "0.3.1"
+version = "0.3.2"
 description = "shellfish ~ shell & file-system utils"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish"
 readme = 'README.md'
 packages = [
```

### Comparing `shellfish-0.3.1/README.md` & `shellfish-0.3.2/README.md`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/__init__.py` & `shellfish-0.3.2/shellfish/__init__.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/_types.py` & `shellfish-0.3.2/shellfish/_types.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/aios/__init__.py` & `shellfish-0.3.2/shellfish/aios/__init__.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/aios/_path.py` & `shellfish-0.3.2/shellfish/aios/_path.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/batman.py` & `shellfish-0.3.2/shellfish/batman.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/dev/do.py` & `shellfish-0.3.2/shellfish/dev/do.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/dev/popen_gen.py` & `shellfish-0.3.2/shellfish/dev/popen_gen.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/dev/run_async.py` & `shellfish-0.3.2/shellfish/dev/run_async.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/dotenv.py` & `shellfish-0.3.2/shellfish/dotenv.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/echo.py` & `shellfish-0.3.2/shellfish/echo.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/exe.py` & `shellfish-0.3.2/shellfish/exe.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/fs/__init__.py` & `shellfish-0.3.2/shellfish/fs/__init__.py`

 * *Files 0% similar despite different names*

```diff
@@ -562,15 +562,15 @@
         >>> expected_dirs = [el.replace('\\', '/') for el in expected_dirs]
         >>> pprint(expected_dirs)
         ['dirs_gen.doctest/dir',
          'dirs_gen.doctest/dir/dir2',
          'dirs_gen.doctest/dir/dir2a']
         >>> _files = list(files_gen(tmpdir))
         >>> _dirs = list(dirs_gen(tmpdir))
-        >>> files_n_dirs_list = list(sorted(set(_files + _dirs)))
+        >>> files_n_dirs_list = list(sorted(_files + _dirs))
         >>> files_n_dirs_list = [el.replace('\\', '/') for el in files_n_dirs_list]
         >>> pprint(files_n_dirs_list)
         ['dirs_gen.doctest',
          'dirs_gen.doctest/dir',
          'dirs_gen.doctest/dir/dir2',
          'dirs_gen.doctest/dir/dir2/file1.txt',
          'dirs_gen.doctest/dir/dir2/file2.txt',
@@ -803,15 +803,15 @@
          'walk_gen.doctest/dir/dir2a/file1.txt',
          'walk_gen.doctest/dir/dir2a/file2.txt',
          'walk_gen.doctest/dir/dir2a/file3.txt']
         >>> pprint(expected_dirs)
         ['walk_gen.doctest/dir',
          'walk_gen.doctest/dir/dir2',
          'walk_gen.doctest/dir/dir2a']
-        >>> walk_gen_list = list(sorted(set(walk_gen(tmpdir))))
+        >>> walk_gen_list = list(sorted(walk_gen(tmpdir)))
         >>> walk_gen_list = [el.replace('\\', '/') for el in walk_gen_list]
         >>> pprint(walk_gen_list)
         ['walk_gen.doctest',
          'walk_gen.doctest/dir',
          'walk_gen.doctest/dir/dir2',
          'walk_gen.doctest/dir/dir2/file1.txt',
          'walk_gen.doctest/dir/dir2/file2.txt',
@@ -850,15 +850,14 @@
     return (
         str(path_string)
         if abspath
         else str(path_string).replace(dirpath, "").strip(sep)
         for path_string in chain.from_iterable(
             (
                 pwd,
-                *(path.join(pwd, _dir) for _dir in dirs),
                 *(path.join(pwd, _file) for _file in files),
             )
             for pwd, dirs, files in walk(
                 dirpath,
                 topdown=topdown,
                 followlinks=followlinks,
                 onerror=onerror,
```

### Comparing `shellfish-0.3.1/shellfish/fs/_async.py` & `shellfish-0.3.2/shellfish/fs/_async.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/fs/promises.py` & `shellfish-0.3.2/shellfish/fs/promises.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/libhash.py` & `shellfish-0.3.2/shellfish/libhash.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/libsh/_dirtree.py` & `shellfish-0.3.2/shellfish/libsh/_dirtree.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/libsh/args.py` & `shellfish-0.3.2/shellfish/libsh/args.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/osfs.py` & `shellfish-0.3.2/shellfish/osfs.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/process.py` & `shellfish-0.3.2/shellfish/process.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/sh.py` & `shellfish-0.3.2/shellfish/sh.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/sp.py` & `shellfish-0.3.2/shellfish/sp.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/testing.py` & `shellfish-0.3.2/shellfish/testing.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/shellfish/tests/test_fs.py` & `shellfish-0.3.2/shellfish/tests/test_fs.py`

 * *Files identical despite different names*

### Comparing `shellfish-0.3.1/PKG-INFO` & `shellfish-0.3.2/PKG-INFO`

 * *Files 1% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: shellfish
-Version: 0.3.1
+Version: 0.3.2
 Summary: shellfish ~ shell & file-system utils
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/shellfish
 License: MIT
 Keywords: dgpy,shell,fs,filesystem,typed
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0
```

#### html2text {}

```diff
@@ -1,8 +1,8 @@
-Metadata-Version: 2.1 Name: shellfish Version: 0.3.1 Summary: shellfish ~ shell
+Metadata-Version: 2.1 Name: shellfish Version: 0.3.2 Summary: shellfish ~ shell
 & file-system utils Home-page: https://github.com/dynamic-graphics-inc/dgpy-
 libs/tree/main/libs/shellfish License: MIT Keywords:
 dgpy,shell,fs,filesystem,typed Author: jesse Author-email: jesse@dgi.com
 Requires-Python: >=3.7,<4.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
```

