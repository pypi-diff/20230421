# Comparing `tmp/arc4-0.3.0.tar.gz` & `tmp/arc4-0.4.0.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "arc4-0.3.0.tar", last modified: Fri Aug 19 21:14:07 2022, max compression
+gzip compressed data, was "arc4-0.4.0.tar", last modified: Fri Apr 21 20:03:58 2023, max compression
```

## Comparing `arc4-0.3.0.tar` & `arc4-0.4.0.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 21:14:07.722499 arc4-0.3.0/
--rw-r--r--   0 runner    (1001) docker     (121)     1073 2022-08-19 21:14:06.000000 arc4-0.3.0/LICENSE
--rw-r--r--   0 runner    (1001) docker     (121)       19 2022-08-19 21:14:06.000000 arc4-0.3.0/MANIFEST.in
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-08-19 21:14:07.722499 arc4-0.3.0/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)     2198 2022-08-19 21:14:06.000000 arc4-0.3.0/README.rst
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 21:14:07.722499 arc4-0.3.0/arc4-stubs/
--rw-r--r--   0 runner    (1001) docker     (121)      211 2022-08-19 21:14:06.000000 arc4-0.3.0/arc4-stubs/__init__.pyi
--rw-r--r--   0 runner    (1001) docker     (121)    12875 2022-08-19 21:14:06.000000 arc4-0.3.0/arc4.c
-drwxr-xr-x   0 runner    (1001) docker     (121)        0 2022-08-19 21:14:07.722499 arc4-0.3.0/arc4.egg-info/
--rw-r--r--   0 runner    (1001) docker     (121)     3172 2022-08-19 21:14:07.000000 arc4-0.3.0/arc4.egg-info/PKG-INFO
--rw-r--r--   0 runner    (1001) docker     (121)      182 2022-08-19 21:14:07.000000 arc4-0.3.0/arc4.egg-info/SOURCES.txt
--rw-r--r--   0 runner    (1001) docker     (121)        1 2022-08-19 21:14:07.000000 arc4-0.3.0/arc4.egg-info/dependency_links.txt
--rw-r--r--   0 runner    (1001) docker     (121)       16 2022-08-19 21:14:07.000000 arc4-0.3.0/arc4.egg-info/top_level.txt
--rw-r--r--   0 runner    (1001) docker     (121)       38 2022-08-19 21:14:07.722499 arc4-0.3.0/setup.cfg
--rw-r--r--   0 runner    (1001) docker     (121)     1768 2022-08-19 21:14:06.000000 arc4-0.3.0/setup.py
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 20:03:58.005778 arc4-0.4.0/
+-rw-r--r--   0 runner    (1001) docker     (122)     1073 2023-04-21 20:03:57.000000 arc4-0.4.0/LICENSE
+-rw-r--r--   0 runner    (1001) docker     (122)       19 2023-04-21 20:03:57.000000 arc4-0.4.0/MANIFEST.in
+-rw-r--r--   0 runner    (1001) docker     (122)     3073 2023-04-21 20:03:58.005778 arc4-0.4.0/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)     2198 2023-04-21 20:03:57.000000 arc4-0.4.0/README.rst
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 20:03:58.001778 arc4-0.4.0/arc4-stubs/
+-rw-r--r--   0 runner    (1001) docker     (122)      211 2023-04-21 20:03:57.000000 arc4-0.4.0/arc4-stubs/__init__.pyi
+-rw-r--r--   0 runner    (1001) docker     (122)    11677 2023-04-21 20:03:57.000000 arc4-0.4.0/arc4.c
+drwxr-xr-x   0 runner    (1001) docker     (122)        0 2023-04-21 20:03:58.005778 arc4-0.4.0/arc4.egg-info/
+-rw-r--r--   0 runner    (1001) docker     (122)     3073 2023-04-21 20:03:57.000000 arc4-0.4.0/arc4.egg-info/PKG-INFO
+-rw-r--r--   0 runner    (1001) docker     (122)      182 2023-04-21 20:03:58.000000 arc4-0.4.0/arc4.egg-info/SOURCES.txt
+-rw-r--r--   0 runner    (1001) docker     (122)        1 2023-04-21 20:03:57.000000 arc4-0.4.0/arc4.egg-info/dependency_links.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       16 2023-04-21 20:03:57.000000 arc4-0.4.0/arc4.egg-info/top_level.txt
+-rw-r--r--   0 runner    (1001) docker     (122)       38 2023-04-21 20:03:58.005778 arc4-0.4.0/setup.cfg
+-rw-r--r--   0 runner    (1001) docker     (122)     1663 2023-04-21 20:03:57.000000 arc4-0.4.0/setup.py
```

### Comparing `arc4-0.3.0/LICENSE` & `arc4-0.4.0/LICENSE`

 * *Files identical despite different names*

### Comparing `arc4-0.3.0/PKG-INFO` & `arc4-0.4.0/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: arc4
-Version: 0.3.0
+Version: 0.4.0
 Summary: A small and insanely fast ARCFOUR (RC4) cipher implementation of Python
 Home-page: https://github.com/manicmaniac/arc4
 Author: Ryosuke Ito
 Author-email: rito.0305@gmail.com
 Keywords: ARCFOUR,cipher,cryptography,RC4
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security :: Cryptography
 License-File: LICENSE
 
 arc4
 ====
```

### Comparing `arc4-0.3.0/README.rst` & `arc4-0.4.0/README.rst`

 * *Files identical despite different names*

### Comparing `arc4-0.3.0/arc4.c` & `arc4-0.4.0/arc4.c`

 * *Files 3% similar despite different names*

```diff
@@ -15,22 +15,14 @@
 #ifdef __inline__
 #define inline __inline__
 #else
 #define inline
 #endif /* __inline__ */
 #endif /* __STDC_VERSION__ < 199901L */
 
-/* Backport of the convenience macro introduced in Python 3.5
- * See https://github.com/python/cpython/blob/v3.5.0/Include/pymacro.h#L19
- */
-#ifndef Py_STRINGIFY
-#define ARC4_XSTRINGIFY(x) #x
-#define Py_STRINGIFY(x) ARC4_XSTRINGIFY(x)
-#endif /* Py_STRINGIFY */
-
 struct arc4_state {
     unsigned char x, y, s[256];
 };
 
 static const struct arc4_state arc4_initial_state = {
     0, /* x */
     0, /* y */
@@ -131,15 +123,15 @@
      * This behavior looks intended as document says:
      * > a few corner cases don’t raise the same exception
      * https://doc.pypy.org/en/latest/cpython_differences.html#miscellaneous
      */
     if (!(is_bytes || PyUnicode_Check(args))) {
         PyErr_Format(PyExc_TypeError,
                      "argument 1 must be read-only bytes-like object, not %s",
-                     args->ob_type->tp_name);
+                     Py_TYPE(args)->tp_name);
         return -1;
     }
 #endif /* PYPY_VERSION */
     if (key_size <= 0) {
         PyErr_Format(PyExc_ValueError, "invalid key length: %zd", key_size);
         return -1;
     }
@@ -172,28 +164,18 @@
         size = PyBytes_GET_SIZE(arg);
     }
     else if (PyUnicode_Check(arg)) {
         if (PyErr_WarnEx(PyExc_DeprecationWarning,
                          arc4_str_deprecation_warning, 1) == -1) {
             return NULL;
         }
-#if PY_MAJOR_VERSION >= 3
         input = (char *)PyUnicode_AsUTF8AndSize(arg, &size);
         if (input == NULL) {
             return NULL;
         }
-#else
-        arg = PyUnicode_AsASCIIString(arg);
-        if (arg == NULL) {
-            return NULL;
-        }
-        outputBytes = arc4_ARC4_crypt(self, arg);
-        Py_DECREF(arg);
-        return outputBytes;
-#endif /* PY_MAJOR_VERSION >= 3 */
     }
     else {
         return PyErr_Format(PyExc_TypeError,
                             "crypt() argument 1 must be read-only bytes-like "
                             "object, not %s",
                             Py_TYPE(arg)->tp_name);
     }
@@ -323,15 +305,14 @@
     0,                             /* tp_descr_set */
     0,                             /* tp_dictoffset */
     (initproc)arc4_ARC4_init,      /* tp_init */
     0,                             /* tp_alloc */
     PyType_GenericNew,             /* tp_new */
 };
 
-#if PY_MAJOR_VERSION >= 3
 static struct PyModuleDef arc4_module = {
     PyModuleDef_HEAD_INIT, /* m_base */
     "arc4",                /* m_name */
     arc4_doc,              /* m_doc */
     -1,                    /* m_size */
     NULL                   /* m_methods */
 };
@@ -357,33 +338,7 @@
     if (PyModule_AddObject(module, "ARC4", (PyObject *)&arc4_ARC4Type) < 0) {
         Py_DECREF(&arc4_ARC4Type);
         Py_DECREF(module);
         return NULL;
     }
     return module;
 }
-#else
-PyMODINIT_FUNC
-initarc4(void)
-{
-    PyObject *module;
-
-    if (PyType_Ready(&arc4_ARC4Type) < 0) {
-        return;
-    }
-    module = Py_InitModule3("arc4", NULL, arc4_doc);
-    if (module == NULL) {
-        return;
-    }
-    if (PyModule_AddStringConstant(module, "__version__",
-                                   Py_STRINGIFY(ARC4_VERSION)) < 0) {
-        Py_DECREF(module);
-        return;
-    }
-    Py_INCREF(&arc4_ARC4Type);
-    if (PyModule_AddObject(module, "ARC4", (PyObject *)&arc4_ARC4Type) < 0) {
-        Py_DECREF(&arc4_ARC4Type);
-        Py_DECREF(module);
-        return;
-    }
-}
-#endif /* PY_MAJOR_VERSION >= 3 */
```

### Comparing `arc4-0.3.0/arc4.egg-info/PKG-INFO` & `arc4-0.4.0/arc4.egg-info/PKG-INFO`

 * *Files 4% similar despite different names*

```diff
@@ -1,25 +1,23 @@
 Metadata-Version: 2.1
 Name: arc4
-Version: 0.3.0
+Version: 0.4.0
 Summary: A small and insanely fast ARCFOUR (RC4) cipher implementation of Python
 Home-page: https://github.com/manicmaniac/arc4
 Author: Ryosuke Ito
 Author-email: rito.0305@gmail.com
 Keywords: ARCFOUR,cipher,cryptography,RC4
 Classifier: Development Status :: 4 - Beta
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Operating System :: OS Independent
-Classifier: Programming Language :: Python :: 2.7
-Classifier: Programming Language :: Python :: 3.5
-Classifier: Programming Language :: Python :: 3.6
 Classifier: Programming Language :: Python :: 3.7
 Classifier: Programming Language :: Python :: 3.8
 Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Programming Language :: Python :: Implementation :: PyPy
 Classifier: Topic :: Security :: Cryptography
 License-File: LICENSE
 
 arc4
 ====
```

### Comparing `arc4-0.3.0/setup.py` & `arc4-0.4.0/setup.py`

 * *Files 14% similar despite different names*

```diff
@@ -1,14 +1,14 @@
 try:
     from setuptools import Extension, setup
 except ImportError:
     from distutils.core import Extension, setup
 
 
-VERSION = '0.3.0'
+VERSION = '0.4.0'
 
 
 def read_file(path):
     with open(path) as f:
         return f.read()
 
 
@@ -39,19 +39,17 @@
             'cryptography',
             'RC4',
         ],
         classifiers=[
             'Development Status :: 4 - Beta',
             'License :: OSI Approved :: MIT License',
             'Operating System :: OS Independent',
-            'Programming Language :: Python :: 2.7',
-            'Programming Language :: Python :: 3.5',
-            'Programming Language :: Python :: 3.6',
             'Programming Language :: Python :: 3.7',
             'Programming Language :: Python :: 3.8',
             'Programming Language :: Python :: 3.9',
             'Programming Language :: Python :: 3.10',
+            'Programming Language :: Python :: 3.11',
             'Programming Language :: Python :: Implementation :: CPython',
             'Programming Language :: Python :: Implementation :: PyPy',
             'Topic :: Security :: Cryptography',
         ],
     )
```

