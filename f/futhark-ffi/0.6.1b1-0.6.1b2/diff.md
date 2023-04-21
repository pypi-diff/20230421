# Comparing `tmp/futhark_ffi-0.6.1b1.tar.gz` & `tmp/futhark_ffi-0.6.1b2.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist/futhark_ffi-0.6.1b1.tar", last modified: Wed Jul  4 15:55:40 2018, max compression
+gzip compressed data, was "dist/futhark_ffi-0.6.1b2.tar", last modified: Wed Jul 11 19:15:04 2018, max compression
```

## Comparing `futhark_ffi-0.6.1b1.tar` & `futhark_ffi-0.6.1b2.tar`

### file list

```diff
@@ -1,16 +1,16 @@
-drwxr-xr-x   0 pepijn    (1000) pepijn    (1000)        0 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/
-drwxr-xr-x   0 pepijn    (1000) pepijn    (1000)        0 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/futhark_ffi.egg-info/
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)       12 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/futhark_ffi.egg-info/top_level.txt
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)     1623 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/futhark_ffi.egg-info/PKG-INFO
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)        1 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/futhark_ffi.egg-info/dependency_links.txt
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)       62 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/futhark_ffi.egg-info/entry_points.txt
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)      297 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/futhark_ffi.egg-info/SOURCES.txt
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)       11 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/futhark_ffi.egg-info/requires.txt
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)       38 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/setup.cfg
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)     1102 2018-07-03 08:10:14.000000 futhark_ffi-0.6.1b1/README.md
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)     1623 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/PKG-INFO
--rw-rw-r--   0 pepijn    (1000) pepijn    (1000)     1157 2018-07-04 15:54:53.000000 futhark_ffi-0.6.1b1/setup.py
-drwxr-xr-x   0 pepijn    (1000) pepijn    (1000)        0 2018-07-04 15:55:40.000000 futhark_ffi-0.6.1b1/futhark_ffi/
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)     4803 2018-07-04 15:51:06.000000 futhark_ffi-0.6.1b1/futhark_ffi/__init__.py
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)     1285 2018-07-04 15:46:03.000000 futhark_ffi-0.6.1b1/futhark_ffi/compat.py
--rw-r--r--   0 pepijn    (1000) pepijn    (1000)      492 2018-07-04 15:09:11.000000 futhark_ffi-0.6.1b1/futhark_ffi/build.py
+drwxr-xr-x   0 pepijn    (1000) pepijn    (1000)        0 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/
+drwxr-xr-x   0 pepijn    (1000) pepijn    (1000)        0 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/futhark_ffi.egg-info/
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)       12 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/futhark_ffi.egg-info/top_level.txt
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)     1918 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/futhark_ffi.egg-info/PKG-INFO
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)        1 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/futhark_ffi.egg-info/dependency_links.txt
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)       62 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/futhark_ffi.egg-info/entry_points.txt
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)      297 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/futhark_ffi.egg-info/SOURCES.txt
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)       11 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/futhark_ffi.egg-info/requires.txt
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)       38 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/setup.cfg
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)     1325 2018-07-05 06:37:05.000000 futhark_ffi-0.6.1b2/README.md
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)     1918 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/PKG-INFO
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)     1170 2018-07-11 19:14:50.000000 futhark_ffi-0.6.1b2/setup.py
+drwxr-xr-x   0 pepijn    (1000) pepijn    (1000)        0 2018-07-11 19:15:04.000000 futhark_ffi-0.6.1b2/futhark_ffi/
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)     4852 2018-07-05 06:36:42.000000 futhark_ffi-0.6.1b2/futhark_ffi/__init__.py
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)     1285 2018-07-04 15:46:03.000000 futhark_ffi-0.6.1b2/futhark_ffi/compat.py
+-rw-r--r--   0 pepijn    (1000) pepijn    (1000)      555 2018-07-05 06:36:42.000000 futhark_ffi-0.6.1b2/futhark_ffi/build.py
```

### Comparing `futhark_ffi-0.6.1b1/futhark_ffi.egg-info/PKG-INFO` & `futhark_ffi-0.6.1b2/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
-Name: futhark-ffi
-Version: 0.6.1b1
+Name: futhark_ffi
+Version: 0.6.1b2
 Summary: A Python library using the Futhark C backend via CFFI 
 Home-page: https://github.com/pepijndevos/futhark-pycffi
 Author: Pepijn de Vos
 License: UNKNOWN
-Description: # futhark-pycffi
+Description: # futhark-ffi
+        [![Build Status](https://travis-ci.org/pepijndevos/futhark-pycffi.svg?branch=master)](https://travis-ci.org/pepijndevos/futhark-pycffi)
+        
         Python library using the Futhark C backend via CFFI
         
         Futhark provides several compilers, `futhark-opencl` which is a C backend, and `futhark-pyopencl` which is a Python backend based on PyOpenCL. However, the host-side code of the Python backend is quite slow, leading to a lot of overhead when small, frequent kernels are used.
         
         A solution to reduce this overhead is to use CFFI to used the C backend from Python, greatly reducing the calling overhead. The OpenCL code is the same, so this is not interesting for long-running kernels.
         
-        This library supports both `futhark-opencl` and `futhark-c`. Futhark arrays are mapped to and from Numpy arrays. Multiple outputs and multi-dimensional arrays are supported. Input arrays should be in contiguous C order.
+        This library supports both `futhark-opencl` and `futhark-c`. Futhark arrays are mapped to and from Numpy arrays. Multiple outputs and multi-dimensional arrays are supported.
+        
+        ## Installation
+        
+        [Install Futhark](https://futhark.readthedocs.io/en/latest/installation.html), then simply
+        ```bash
+        pip install futhark-ffi
+        ```
         
         ## Usage
         
         Generate a C library, and build a Python binding for it
         
         ```bash
         futhark-opencl --library test.fut
-        python build_futhark_ffi.py test
+        build_futhark_ffi test
         ```
         
         Use the Python wrapper
         
         ```python
         import numpy as np
         import _test
```

### Comparing `futhark_ffi-0.6.1b1/README.md` & `futhark_ffi-0.6.1b2/README.md`

 * *Files 16% similar despite different names*

```diff
@@ -1,23 +1,32 @@
-# futhark-pycffi
+# futhark-ffi
+[![Build Status](https://travis-ci.org/pepijndevos/futhark-pycffi.svg?branch=master)](https://travis-ci.org/pepijndevos/futhark-pycffi)
+
 Python library using the Futhark C backend via CFFI
 
 Futhark provides several compilers, `futhark-opencl` which is a C backend, and `futhark-pyopencl` which is a Python backend based on PyOpenCL. However, the host-side code of the Python backend is quite slow, leading to a lot of overhead when small, frequent kernels are used.
 
 A solution to reduce this overhead is to use CFFI to used the C backend from Python, greatly reducing the calling overhead. The OpenCL code is the same, so this is not interesting for long-running kernels.
 
-This library supports both `futhark-opencl` and `futhark-c`. Futhark arrays are mapped to and from Numpy arrays. Multiple outputs and multi-dimensional arrays are supported. Input arrays should be in contiguous C order.
+This library supports both `futhark-opencl` and `futhark-c`. Futhark arrays are mapped to and from Numpy arrays. Multiple outputs and multi-dimensional arrays are supported.
+
+## Installation
+
+[Install Futhark](https://futhark.readthedocs.io/en/latest/installation.html), then simply
+```bash
+pip install futhark-ffi
+```
 
 ## Usage
 
 Generate a C library, and build a Python binding for it
 
 ```bash
 futhark-opencl --library test.fut
-python build_futhark_ffi.py test
+build_futhark_ffi test
 ```
 
 Use the Python wrapper
 
 ```python
 import numpy as np
 import _test
```

### Comparing `futhark_ffi-0.6.1b1/PKG-INFO` & `futhark_ffi-0.6.1b2/futhark_ffi.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,30 +1,39 @@
 Metadata-Version: 2.1
-Name: futhark_ffi
-Version: 0.6.1b1
+Name: futhark-ffi
+Version: 0.6.1b2
 Summary: A Python library using the Futhark C backend via CFFI 
 Home-page: https://github.com/pepijndevos/futhark-pycffi
 Author: Pepijn de Vos
 License: UNKNOWN
-Description: # futhark-pycffi
+Description: # futhark-ffi
+        [![Build Status](https://travis-ci.org/pepijndevos/futhark-pycffi.svg?branch=master)](https://travis-ci.org/pepijndevos/futhark-pycffi)
+        
         Python library using the Futhark C backend via CFFI
         
         Futhark provides several compilers, `futhark-opencl` which is a C backend, and `futhark-pyopencl` which is a Python backend based on PyOpenCL. However, the host-side code of the Python backend is quite slow, leading to a lot of overhead when small, frequent kernels are used.
         
         A solution to reduce this overhead is to use CFFI to used the C backend from Python, greatly reducing the calling overhead. The OpenCL code is the same, so this is not interesting for long-running kernels.
         
-        This library supports both `futhark-opencl` and `futhark-c`. Futhark arrays are mapped to and from Numpy arrays. Multiple outputs and multi-dimensional arrays are supported. Input arrays should be in contiguous C order.
+        This library supports both `futhark-opencl` and `futhark-c`. Futhark arrays are mapped to and from Numpy arrays. Multiple outputs and multi-dimensional arrays are supported.
+        
+        ## Installation
+        
+        [Install Futhark](https://futhark.readthedocs.io/en/latest/installation.html), then simply
+        ```bash
+        pip install futhark-ffi
+        ```
         
         ## Usage
         
         Generate a C library, and build a Python binding for it
         
         ```bash
         futhark-opencl --library test.fut
-        python build_futhark_ffi.py test
+        build_futhark_ffi test
         ```
         
         Use the Python wrapper
         
         ```python
         import numpy as np
         import _test
```

### Comparing `futhark_ffi-0.6.1b1/setup.py` & `futhark_ffi-0.6.1b2/setup.py`

 * *Files 10% similar despite different names*

```diff
@@ -1,19 +1,20 @@
 from setuptools import setup
 from os import path
+import io
 
 here = path.abspath(path.dirname(__file__))
 
 # Get the long description from the README file
-with open(path.join(here, 'README.md'), encoding='utf-8') as f:
+with io.open(path.join(here, 'README.md'), encoding='utf-8') as f:
     long_description = f.read()
 
 setup(
     name='futhark_ffi',
-    version='0.6.1b1',
+    version='0.6.1b2',
     description='A Python library using the Futhark C backend via CFFI ',
     long_description=long_description,
     long_description_content_type='text/markdown',
     url='https://github.com/pepijndevos/futhark-pycffi',
     author='Pepijn de Vos',
     packages=['futhark_ffi'],
     install_requires=['numpy', 'cffi'],  # Optional
```

### Comparing `futhark_ffi-0.6.1b1/futhark_ffi/__init__.py` & `futhark_ffi-0.6.1b2/futhark_ffi/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -1,9 +1,8 @@
 from functools import partial, wraps
-from types import SimpleNamespace
 import numpy as np
 
 np_types = {
     'int8_t': 'int8',
     'int16_t': 'int16',
     'int32_t': 'int32',
     'int64_t': 'int64',
@@ -13,15 +12,16 @@
     'uint64_t': 'uint64',
     'float': 'float32',
     'double': 'float64',
 }
 
 c_types = {v: k for k, v in np_types.items()}
 
-Type = SimpleNamespace
+# SimpleNamespace does not exist in Python 2.7, unfortunately.
+class Type: pass
 
 class Futhark(object):
     """
     A CFFI wrapper for the Futhark C API.
     Takes a CFFI-generated module.
     Entrypoints return arrays as raw C types.
     Use `from_futhark` to convert to Numpy arrays.
@@ -64,15 +64,15 @@
                 setattr(self, fn[14:], self.make_wrapper(ff))
 
     def to_futhark(self, fut_type, data):
         "Convert a Numpy array to a Futhark C type"
         if isinstance(data, self.ffi.CData):
             return data # opaque type
         else:
-            datat = data.astype(np_types[fut_type.itemtype.item.cname], copy=False)
+            datat = data.astype(np_types[fut_type.itemtype.item.cname], copy=False, order='C')
             ptr = self.ffi.cast(fut_type.itemtype, self.ffi.from_buffer(datat))
             constr = fut_type.new
             destr = fut_type.free
             return self.ffi.gc(constr(self.ctx, ptr, *data.shape), partial(destr, self.ctx))
 
     def _from_futhark(self, data):
         cname = self.ffi.typeof(data)
@@ -114,16 +114,16 @@
                     converters.append(partial(self.to_futhark, fut_type))
                 else:
                     converters.append(lambda x: x)
 
         @wraps(ff)
         def wrapper(*args):
             out_args = [self.ffi.new(t) for t in out_types]
-            ff(self.ctx, *out_args,
-               *(f(a) for f, a in zip(converters, args)))
+            in_args = [f(a) for f, a in zip(converters, args)]
+            ff(self.ctx, *(out_args+in_args))
             results = []
             for out_t, out in zip(out_types, out_args):
                 if out_t.item in self.types:
                     ptr = self.ffi.gc(out[0], partial(self.types[out_t.item].free, self.ctx))
                     results.append(ptr)
                 else:
                     results.append(out[0])
```

### Comparing `futhark_ffi-0.6.1b1/futhark_ffi/compat.py` & `futhark_ffi-0.6.1b2/futhark_ffi/compat.py`

 * *Files identical despite different names*

