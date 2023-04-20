# Comparing `tmp/h5-0.8.8.tar.gz` & `tmp/h5-0.8.9.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "h5-0.8.8.tar", max compression
+gzip compressed data, was "h5-0.8.9.tar", max compression
```

## Comparing `h5-0.8.8.tar` & `h5-0.8.9.tar`

### file list

```diff
@@ -1,14 +1,14 @@
--rw-r--r--   0        0        0     2987 2023-04-10 16:39:46.706848 h5-0.8.8/h5/__init__.py
--rw-r--r--   0        0        0     1048 2023-04-10 16:39:46.707849 h5-0.8.8/h5/__main__.py
--rw-r--r--   0        0        0      184 2023-04-10 16:41:57.348070 h5-0.8.8/h5/_meta.py
--rw-r--r--   0        0        0    12195 2023-04-10 16:39:46.707849 h5-0.8.8/h5/cli.py
--rw-r--r--   0        0        0    15743 2023-04-10 16:39:46.708848 h5-0.8.8/h5/core.py
--rw-r--r--   0        0        0    14738 2023-04-10 16:39:46.708848 h5-0.8.8/h5/dev.py
--rw-r--r--   0        0        0     2935 2023-03-31 17:44:54.413796 h5-0.8.8/h5/legacy.py
--rw-r--r--   0        0        0        0 2022-02-01 20:37:20.150020 h5-0.8.8/h5/py.typed
--rw-r--r--   0        0        0     4457 2023-04-10 16:39:46.708848 h5-0.8.8/h5/testing.py
--rw-r--r--   0        0        0     1056 2022-02-11 23:27:58.156814 h5-0.8.8/LICENSE
--rw-r--r--   0        0        0     1891 2023-04-10 16:45:29.557162 h5-0.8.8/pyproject.toml
--rw-r--r--   0        0        0      739 2022-12-12 16:24:11.593604 h5-0.8.8/README.md
--rw-r--r--   0        0        0     1745 1970-01-01 00:00:00.000000 h5-0.8.8/setup.py
--rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 h5-0.8.8/PKG-INFO
+-rw-r--r--   0        0        0      261 2023-04-20 23:19:54.396173 h5-0.8.9/h5/__about__.py
+-rw-r--r--   0        0        0     2991 2023-04-20 20:51:48.646243 h5-0.8.9/h5/__init__.py
+-rw-r--r--   0        0        0     1052 2023-04-20 20:51:48.638448 h5-0.8.9/h5/__main__.py
+-rw-r--r--   0        0        0      337 2023-04-20 20:38:23.581137 h5-0.8.9/h5/_meta.py
+-rw-r--r--   0        0        0    12195 2023-04-10 18:06:42.523049 h5-0.8.9/h5/cli.py
+-rw-r--r--   0        0        0    15746 2023-04-19 19:17:33.717864 h5-0.8.9/h5/core.py
+-rw-r--r--   0        0        0    14738 2023-04-05 20:11:35.022106 h5-0.8.9/h5/dev.py
+-rw-r--r--   0        0        0     2935 2023-03-31 17:46:06.860725 h5-0.8.9/h5/legacy.py
+-rw-r--r--   0        0        0        0 2022-02-01 22:06:04.805953 h5-0.8.9/h5/py.typed
+-rw-r--r--   0        0        0     4457 2023-04-05 20:11:35.027132 h5-0.8.9/h5/testing.py
+-rw-r--r--   0        0        0     1056 2022-02-17 22:17:07.419494 h5-0.8.9/LICENSE
+-rw-r--r--   0        0        0     1899 2023-04-20 23:19:51.777329 h5-0.8.9/pyproject.toml
+-rw-r--r--   0        0        0      739 2022-09-19 18:35:16.982212 h5-0.8.9/README.md
+-rw-r--r--   0        0        0     2035 1970-01-01 00:00:00.000000 h5-0.8.9/PKG-INFO
```

### Comparing `h5-0.8.8/h5/__init__.py` & `h5-0.8.9/h5/__init__.py`

 * *Files 4% similar despite different names*

```diff
@@ -1,12 +1,12 @@
 # -*- coding: utf-8 -*-
 """HDF5 functions, and utils, and generators, OH MY!"""
 from h5py import AttributeManager, Dataset, File, Group, __version__ as __h5py_version__
 
-from h5._meta import __version__
+from h5.__about__ import __version__
 from h5.core import (
     as_h5py_obj as as_h5py_obj,
     attrs as attrs,
     attrs_dict as attrs_dict,
     attrs_gen as attrs_gen,
     attrs_gen_from_fspath as attrs_gen_from_fspath,
     datasets as datasets,
```

### Comparing `h5-0.8.8/h5/__main__.py` & `h5-0.8.9/h5/__main__.py`

 * *Files 7% similar despite different names*

```diff
@@ -1,15 +1,15 @@
 # -*- coding: utf-8 -*-
 """pkg entry ~ `python -m h5`"""
 import json
 import sys
 
 from typing import Optional
 
-from h5._meta import __pkgroot__, __title__, __version__
+from h5.__about__ import __pkgroot__, __title__, __version__
 
 __click_version__: Optional[str] = None
 try:
     from click import __version__ as __click_version__
 except ImportError:
     ...
```

### Comparing `h5-0.8.8/h5/cli.py` & `h5-0.8.9/h5/cli.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.8/h5/core.py` & `h5-0.8.9/h5/core.py`

 * *Files 1% similar despite different names*

```diff
@@ -143,15 +143,15 @@
         return File(obj, "r")
     return obj
 
 
 def h5py_obj_gen(
     h5py_obj: Union[File, Group], h5_path: str = "", root: bool = True
 ) -> Iterable[Tuple[str, Union[Dataset, Group, File]]]:
-    """Recursive h5 datset/group generator.
+    """Recursive h5 dataset/group generator.
 
 
     Args:
         h5py_obj: h5-h5py group object
         h5_path: path so far (Default value = "")
         root: if True, yield the root path (Default value = True)
 
@@ -172,15 +172,15 @@
         ),
     )
 
 
 def h5py_obj_keys_gen(
     h5py_obj: Union[File, Group], h5_path: str = "", root: bool = True
 ) -> Iterable[str]:
-    """Recursive h5 datset generator.
+    """Recursive h5 dataset generator.
 
     Args:
         h5py_obj: h5-h5py group object
         h5_path: path so far (Default value = "")
         root: if True, yield the root path (Default value = True)
 
     Returns:
@@ -308,15 +308,15 @@
     with File(str(fspath), mode="r") as f:
         yield from h5py_obj_attrs_gen(f, h5_path)
 
 
 def h5py_obj_dataset_gen(
     h5py_obj: Union[File, Group], h5_path: str = ""
 ) -> Iterable[Tuple[str, Dataset]]:
-    """Recursive h5 datset generator.
+    """Recursive h5 dataset generator.
 
     Given an h5 group, which is what one gets after loading an h5 file
     via h5py, this function yields tuples containing (1.) a path (h5_path) to
     a dataset in the group, and (2.) the dataset itself as a numpy array.
 
     Args:
         h5py_obj: h5-h5py group object
```

### Comparing `h5-0.8.8/h5/dev.py` & `h5-0.8.9/h5/dev.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.8/h5/legacy.py` & `h5-0.8.9/h5/legacy.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.8/h5/testing.py` & `h5-0.8.9/h5/testing.py`

 * *Files identical despite different names*

### Comparing `h5-0.8.8/LICENSE` & `h5-0.8.9/LICENSE`

 * *Files identical despite different names*

### Comparing `h5-0.8.8/pyproject.toml` & `h5-0.8.9/pyproject.toml`

 * *Files 3% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 [tool.poetry]
 name = "h5"
-version = "0.8.8"
+version = "0.8.9"
 description = "H5py utils"
 license = "MIT"
 authors = ["jesse <jesse@dgi.com>"]
 repository = "https://github.com/dynamic-graphics-inc/dgpy-libs"
 homepage = "https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/h5"
 readme = 'README.md'
 packages = [
@@ -30,22 +30,21 @@
 [tool.poetry.dependencies]
 python = ">=3.8.0"
 h5py = ">=3.7.0"
 numpy = ">=1.23.2"
 typing-extensions = "^4.5.0"
 click = { version = "^8.1.3", optional = true }
 rich = { version = "^13.3.3", optional = true }
-globsters = { version = "^0.0.2", optional = true }
+globsters = { version = ">=0.0.2,<0.0.4", optional = true }
 
 [tool.poetry.extras]
 cli = ["click", "rich", "globsters"]
 
-
 [tool.poetry.dev-dependencies]
-pytest = "^7.3.0"
+pytest = "^7.3.1"
 
 # coverage config
 # [tool.coverage.run]
 # omit = ["*/tests/*", "*/__init__.py", "h5/__main__.py",]
 [tool.poetry.scripts]
 h5 = "h5.cli:main"
 
@@ -54,15 +53,15 @@
 branch = true
 context = '${CONTEXT}'
 
 [tool.coverage.report]
 show_missing = true
 precision = 2
 omit = [
-  "*/legacy.py"
+  "*/legacy.py",
 ]
 exclude_lines = [
   'pragma: no cover',
   'raise NotImplementedError',
   'if TYPE_CHECKING:',
   '@overload',
   '\(Protocol\):$',
```

### Comparing `h5-0.8.8/README.md` & `h5-0.8.9/README.md`

 * *Files identical despite different names*

### Comparing `h5-0.8.8/PKG-INFO` & `h5-0.8.9/PKG-INFO`

 * *Files 6% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: h5
-Version: 0.8.8
+Version: 0.8.9
 Summary: H5py utils
 Home-page: https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/h5
 License: MIT
 Keywords: hdf5,h5py,h5,numpy
 Author: jesse
 Author-email: jesse@dgi.com
 Requires-Python: >=3.8.0
@@ -19,15 +19,15 @@
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Typing :: Typed
 Provides-Extra: cli
 Requires-Dist: click (>=8.1.3,<9.0.0) ; extra == "cli"
-Requires-Dist: globsters (>=0.0.2,<0.0.3) ; extra == "cli"
+Requires-Dist: globsters (>=0.0.2,<0.0.4) ; extra == "cli"
 Requires-Dist: h5py (>=3.7.0)
 Requires-Dist: numpy (>=1.23.2)
 Requires-Dist: rich (>=13.3.3,<14.0.0) ; extra == "cli"
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0)
 Project-URL: Repository, https://github.com/dynamic-graphics-inc/dgpy-libs
 Description-Content-Type: text/markdown
```

#### html2text {}

```diff
@@ -1,21 +1,21 @@
-Metadata-Version: 2.1 Name: h5 Version: 0.8.8 Summary: H5py utils Home-page:
+Metadata-Version: 2.1 Name: h5 Version: 0.8.9 Summary: H5py utils Home-page:
 https://github.com/dynamic-graphics-inc/dgpy-libs/tree/main/libs/h5 License:
 MIT Keywords: hdf5,h5py,h5,numpy Author: jesse Author-email: jesse@dgi.com
 Requires-Python: >=3.8.0 Classifier: Development Status :: 5 - Production/
 Stable Classifier: Intended Audience :: Developers Classifier: License :: OSI
 Approved :: MIT License Classifier: Programming Language :: Python Classifier:
 Programming Language :: Python :: 3 Classifier: Programming Language :: Python
 :: 3.8 Classifier: Programming Language :: Python :: 3.9 Classifier:
 Programming Language :: Python :: 3.10 Classifier: Programming Language ::
 Python :: 3.11 Classifier: Programming Language :: Python :: 3.10 Classifier:
 Programming Language :: Python :: 3.8 Classifier: Programming Language ::
 Python :: 3.9 Classifier: Typing :: Typed Provides-Extra: cli Requires-Dist:
 click (>=8.1.3,<9.0.0) ; extra == "cli" Requires-Dist: globsters
-(>=0.0.2,<0.0.3) ; extra == "cli" Requires-Dist: h5py (>=3.7.0) Requires-Dist:
+(>=0.0.2,<0.0.4) ; extra == "cli" Requires-Dist: h5py (>=3.7.0) Requires-Dist:
 numpy (>=1.23.2) Requires-Dist: rich (>=13.3.3,<14.0.0) ; extra == "cli"
 Requires-Dist: typing-extensions (>=4.5.0,<5.0.0) Project-URL: Repository,
 https://github.com/dynamic-graphics-inc/dgpy-libs Description-Content-Type:
 text/markdown [drawing] # h5 [![Wheel](https://img.shields.io/pypi/wheel/
 h5.svg)](https://img.shields.io/pypi/wheel/h5.svg) [![Version](https://
 img.shields.io/pypi/v/h5.svg)](https://img.shields.io/pypi/v/h5.svg) [!
 [py_versions](https://img.shields.io/pypi/pyversions/h5.svg)](https://
```

