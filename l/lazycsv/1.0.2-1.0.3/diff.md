# Comparing `tmp/lazycsv-1.0.2.tar.gz` & `tmp/lazycsv-1.0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "lazycsv-1.0.2.tar", last modified: Tue Apr 18 01:18:20 2023, max compression
+gzip compressed data, was "lazycsv-1.0.3.tar", last modified: Fri Apr 21 01:33:16 2023, max compression
```

## Comparing `lazycsv-1.0.2.tar` & `lazycsv-1.0.3.tar`

### file list

```diff
@@ -1,18 +1,18 @@
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/
--rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.0.2/LICENSE
--rw-r--r--   0 michael   (1000) michael   (1000)     8548 2023-04-18 01:18:20.654179 lazycsv-1.0.2/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)     7867 2023-04-18 01:17:52.000000 lazycsv-1.0.2/README.md
--rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-18 01:18:20.654179 lazycsv-1.0.2/setup.cfg
--rw-r--r--   0 michael   (1000) michael   (1000)     2042 2023-04-18 01:14:43.000000 lazycsv-1.0.2/setup.py
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/src/
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/src/lazycsv/
--rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.0.2/src/lazycsv/__init__.py
--rw-r--r--   0 michael   (1000) michael   (1000)    32804 2023-04-18 01:12:36.000000 lazycsv-1.0.2/src/lazycsv/lazycsv.c
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/src/lazycsv.egg-info/
--rw-r--r--   0 michael   (1000) michael   (1000)     8548 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/PKG-INFO
--rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/SOURCES.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/dependency_links.txt
--rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/requires.txt
--rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-04-18 01:18:20.000000 lazycsv-1.0.2/src/lazycsv.egg-info/top_level.txt
-drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-18 01:18:20.654179 lazycsv-1.0.2/tests/
--rw-r--r--   0 michael   (1000) michael   (1000)    20036 2023-04-15 01:06:00.000000 lazycsv-1.0.2/tests/test_lazycsv.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.534634 lazycsv-1.0.3/
+-rw-r--r--   0 michael   (1000) michael   (1000)     1066 2023-04-01 16:11:40.000000 lazycsv-1.0.3/LICENSE
+-rw-r--r--   0 michael   (1000) michael   (1000)     8560 2023-04-21 01:33:16.534634 lazycsv-1.0.3/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)     7879 2023-04-18 16:19:33.000000 lazycsv-1.0.3/README.md
+-rw-r--r--   0 michael   (1000) michael   (1000)       38 2023-04-21 01:33:16.534634 lazycsv-1.0.3/setup.cfg
+-rw-r--r--   0 michael   (1000) michael   (1000)     2042 2023-04-21 01:32:31.000000 lazycsv-1.0.3/setup.py
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.531301 lazycsv-1.0.3/src/
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.531301 lazycsv-1.0.3/src/lazycsv/
+-rw-r--r--   0 michael   (1000) michael   (1000)        0 2023-04-01 16:11:40.000000 lazycsv-1.0.3/src/lazycsv/__init__.py
+-rw-r--r--   0 michael   (1000) michael   (1000)    35127 2023-04-21 01:31:44.000000 lazycsv-1.0.3/src/lazycsv/lazycsv.c
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.534634 lazycsv-1.0.3/src/lazycsv.egg-info/
+-rw-r--r--   0 michael   (1000) michael   (1000)     8560 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/PKG-INFO
+-rw-r--r--   0 michael   (1000) michael   (1000)      268 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/SOURCES.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        1 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/dependency_links.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)       61 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/requires.txt
+-rw-r--r--   0 michael   (1000) michael   (1000)        8 2023-04-21 01:33:16.000000 lazycsv-1.0.3/src/lazycsv.egg-info/top_level.txt
+drwxr-xr-x   0 michael   (1000) michael   (1000)        0 2023-04-21 01:33:16.534634 lazycsv-1.0.3/tests/
+-rw-r--r--   0 michael   (1000) michael   (1000)    21311 2023-04-20 23:50:41.000000 lazycsv-1.0.3/tests/test_lazycsv.py
```

### Comparing `lazycsv-1.0.2/LICENSE` & `lazycsv-1.0.3/LICENSE`

 * *Files identical despite different names*

### Comparing `lazycsv-1.0.2/PKG-INFO` & `lazycsv-1.0.3/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.0.2
+Version: 1.0.3
 Summary: an OOM csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: benchmarks
 License-File: LICENSE
 
-# lazycsv - an OOM csv parser
+# lazycsv - a memory-efficient csv parser
 
 ###### Developers: Michael Green, Chris Perkins
 
 lazycsv is a C implementation of a csv parser for python. The aim of this
 parser is to provide for fast extraction of sequences of data from a CSV file
 in a memory-efficient manner, with zero dependencies.
 
@@ -32,17 +32,17 @@
 
 The parser works as follows:
 
 First, The user file is memory-mapped internally to the LazyCSV object. That
 file is used to generate three indexes. The first is an index of values which
 correspond to the position in the user file where a given CSV field starts.
 This value is always a `uint16_t` which we found to be the optimal bit size for
-disk usage and execution performance. (This type can however be changed by
+disk usage and execution performance (This type can however be changed by
 setting the `LAZYCSV_INDEX_DTYPE` environment variable to any unsigned integer
-type) For index values outside the range of an unsigned short, An "anchor
+type). For index values outside the range of an unsigned short, An "anchor
 point" is created, which is a pair of `size_t` values that mark both the value
 which is subtracted from the index value such that the index value fits within
 16 bits, and the first column of the CSV where the anchor value applies. This
 anchor point is periodically written to the second index file when required for
 a given comma index. Finally, the third index writes the index of the first
 anchor point for each row of the file.
```

### Comparing `lazycsv-1.0.2/README.md` & `lazycsv-1.0.3/README.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,8 +1,8 @@
-# lazycsv - an OOM csv parser
+# lazycsv - a memory-efficient csv parser
 
 ###### Developers: Michael Green, Chris Perkins
 
 lazycsv is a C implementation of a csv parser for python. The aim of this
 parser is to provide for fast extraction of sequences of data from a CSV file
 in a memory-efficient manner, with zero dependencies.
 
@@ -12,17 +12,17 @@
 
 The parser works as follows:
 
 First, The user file is memory-mapped internally to the LazyCSV object. That
 file is used to generate three indexes. The first is an index of values which
 correspond to the position in the user file where a given CSV field starts.
 This value is always a `uint16_t` which we found to be the optimal bit size for
-disk usage and execution performance. (This type can however be changed by
+disk usage and execution performance (This type can however be changed by
 setting the `LAZYCSV_INDEX_DTYPE` environment variable to any unsigned integer
-type) For index values outside the range of an unsigned short, An "anchor
+type). For index values outside the range of an unsigned short, An "anchor
 point" is created, which is a pair of `size_t` values that mark both the value
 which is subtracted from the index value such that the index value fits within
 16 bits, and the first column of the CSV where the anchor value applies. This
 anchor point is periodically written to the second index file when required for
 a given comma index. Finally, the third index writes the index of the first
 anchor point for each row of the file.
```

### Comparing `lazycsv-1.0.2/setup.py` & `lazycsv-1.0.3/setup.py`

 * *Files 4% similar despite different names*

```diff
@@ -36,15 +36,15 @@
 ]
 
 with open("README.md", "r") as f:
     long_description = f.read()
 
 setup(
     name="lazycsv",
-    version="1.0.2",
+    version="1.0.3",
     author="Michael Green, Chris Perkins",
     author_email="dev@crunch.io",
     description="an OOM csv parser",
     long_description=long_description,
     long_description_content_type="text/markdown",
     packages=find_packages(where="src"),
     extras_require={
```

### Comparing `lazycsv-1.0.2/src/lazycsv/lazycsv.c` & `lazycsv-1.0.3/src/lazycsv/lazycsv.c`

 * *Files 2% similar despite different names*

```diff
@@ -1,9 +1,10 @@
 #include <stdlib.h>
 #include <stdio.h>
+#include <stdint.h>
 #include <fcntl.h>
 #include <sys/mman.h>
 #include <sys/types.h>
 #include <sys/stat.h>
 #include <unistd.h>
 #include <limits.h>
 
@@ -112,14 +113,16 @@
 
 typedef struct {
     PyObject_HEAD
     PyObject* lazy;
     size_t row;
     size_t col;
     size_t position;
+    size_t stop;
+    size_t step;
     char reversed;
     char skip_header;
 } LazyCSV_Iter;
 
 
 static inline void _BufferWrite(int fd, LazyCSV_Buffer *buffer, void *data,
                                 size_t size) {
@@ -220,26 +223,26 @@
 }
 
 
 static inline void LazyCSV_IterCol(LazyCSV_Iter *iter, size_t *offset,
                                    size_t *len) {
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
 
-    if (iter->position < lazy->rows) {
+    if (iter->position < iter->stop) {
 
         size_t position;
 
         if (iter->reversed) {
             position = lazy->rows - 1 - iter->position + !lazy->_skip_headers;
         }
         else {
             position = iter->position + !lazy->_skip_headers;
         }
 
-        iter->position += 1;
+        iter->position += iter->step;
 
         char* newlines = lazy->_index->newlines->data;
         char* anchors = lazy->_index->anchors->data;
         char* commas = lazy->_index->commas->data;
 
         LazyCSV_RowIndex* ridx =
             (LazyCSV_RowIndex*)
@@ -257,19 +260,19 @@
 }
 
 
 static inline void LazyCSV_IterRow(LazyCSV_Iter *iter, size_t *offset,
                                    size_t *len) {
     LazyCSV *lazy = (LazyCSV *)iter->lazy;
 
-    if (iter->position < lazy->cols) {
+    if (iter->position < iter->stop) {
         size_t position = iter->reversed ?
             lazy->cols - iter->position - 1 : iter->position;
 
-        iter->position += 1;
+        iter->position += iter->step;
 
         char* newlines = lazy->_index->newlines->data;
         char* anchors = lazy->_index->anchors->data;
         char* commas = lazy->_index->commas->data;
 
         size_t row = iter->row + !lazy->_skip_headers;
 
@@ -1105,26 +1108,113 @@
         PyErr_SetString(
             PyExc_MemoryError,
             "unable to allocate memory for iterable"
         );
         return NULL;
     }
 
+    LazyCSV* lazy = (LazyCSV*)self;
+
     iter->row = row;
     iter->col = col;
     iter->reversed = reversed;
     iter->position = 0;
+    iter->step = 1;
+    iter->stop = col == SIZE_MAX ? lazy->cols : lazy->rows;
     iter->lazy = self;
 
     Py_INCREF(self);
 
     return (PyObject*)iter;
 }
 
 
+static PyObject* LazyCSV_GetValue(PyObject* self, PyObject* r, PyObject* c) {
+
+    Py_ssize_t row = PyLong_AsSsize_t(r);
+    Py_ssize_t col = PyLong_AsSsize_t(c);
+
+    LazyCSV* lazy = (LazyCSV*)self;
+
+    if (row < 0) {
+        row = lazy->rows + row;
+    }
+
+    if (col < 0) {
+        col = lazy->cols + col;
+    }
+
+    int row_in_bounds = (
+        0 <= row && row < lazy->rows
+    );
+
+    int col_in_bounds = (
+        0 <= col && col < lazy->cols
+    );
+
+    if (!row_in_bounds || !col_in_bounds) {
+        PyErr_SetString(
+            PyExc_ValueError,
+            "provided value not in bounds of index"
+        );
+        return NULL;
+    }
+
+    row += !lazy->_skip_headers;
+
+    char* newlines = lazy->_index->newlines->data;
+    char* anchors = lazy->_index->anchors->data;
+    char* commas = lazy->_index->commas->data;
+
+    LazyCSV_RowIndex* ridx =
+        (LazyCSV_RowIndex*)
+        (newlines + row*sizeof(LazyCSV_RowIndex));
+
+    char* aidx = anchors+ridx->index;
+    char* cidx = commas+((lazy->cols+1)*row*sizeof(INDEX_DTYPE));
+
+    size_t cs = _Value_FromIndex((size_t)col, ridx, cidx, aidx);
+    size_t ce = _Value_FromIndex((size_t)col + 1, ridx, cidx, aidx);
+
+    size_t len = ce - cs - 1;
+
+    return PyBytes_FromOffsetAndLen(lazy, cs, len);
+}
+
+
+static PyObject* LazyCSV_GetItem(PyObject* self, PyObject* key) {
+    if (!PyTuple_Check(key)) {
+        PyErr_SetString(
+            PyExc_ValueError,
+            "index must contain both a row and column value"
+        );
+        return NULL;
+    }
+
+    PyObject *row, *col;
+
+    if (!PyArg_ParseTuple(key, "OO", &row, &col)) {
+        PyErr_SetString(
+            PyExc_RuntimeError,
+            "unable to parse index key"
+        );
+        return NULL;
+    }
+
+    if (PyLong_Check(row) && PyLong_Check(col))
+        return LazyCSV_GetValue(self, row, col);
+
+    PyErr_SetString(
+        PyExc_ValueError,
+        "given indexing schema is not supported"
+    );
+    return NULL;
+}
+
+
 static PyMemberDef LazyCSV_Members[] = {
     {"headers", T_OBJECT, offsetof(LazyCSV, headers), READONLY, "header tuple"},
     {"rows", T_LONG, offsetof(LazyCSV, rows), READONLY, "row length"},
     {"cols", T_LONG, offsetof(LazyCSV, cols), READONLY, "col length"},
     {"name", T_OBJECT, offsetof(LazyCSV, name), READONLY, "file name"},
     {NULL, }
 };
@@ -1136,14 +1226,20 @@
         (PyCFunction)LazyCSV_Seq,
         METH_VARARGS|METH_KEYWORDS,
         "get column iterator"
     },
     {NULL, }
 };
 
+static PyMappingMethods LazyCSV_MappingMembers[] = {
+    (lenfunc)NULL,
+    (binaryfunc)LazyCSV_GetItem,
+    (objobjargproc)NULL,
+};
+
 PyDoc_STRVAR(
     LazyCSV_Docstring,
     "lazycsv.LazyCSV(\n"
     "    filepath,\n"
     "    /\n"
     "    unquoted: bool=True,\n"
     "    skip_headers: bool=False,\n"
@@ -1182,14 +1278,15 @@
     .tp_name = "lazycsv.LazyCSV",
     .tp_doc = LazyCSV_Docstring,
     .tp_basicsize = sizeof(LazyCSV),
     .tp_dealloc = (destructor)LazyCSV_Destruct,
     .tp_flags = Py_TPFLAGS_DEFAULT|Py_TPFLAGS_BASETYPE,
     .tp_methods = LazyCSV_Methods,
     .tp_members = LazyCSV_Members,
+    .tp_as_mapping = LazyCSV_MappingMembers,
     .tp_new = LazyCSV_New,
 };
 
 
 static PyModuleDef LazyCSVModule = {
     PyModuleDef_HEAD_INIT,
     "lazycsv",
```

### Comparing `lazycsv-1.0.2/src/lazycsv.egg-info/PKG-INFO` & `lazycsv-1.0.3/src/lazycsv.egg-info/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: lazycsv
-Version: 1.0.2
+Version: 1.0.3
 Summary: an OOM csv parser
 Author: Michael Green, Chris Perkins
 Author-email: dev@crunch.io
 Classifier: Development Status :: 5 - Production/Stable
 Classifier: Intended Audience :: Developers
 Classifier: License :: OSI Approved :: MIT License
 Classifier: Natural Language :: English
@@ -14,15 +14,15 @@
 Classifier: Programming Language :: Python :: Implementation :: CPython
 Classifier: Topic :: Utilities
 Description-Content-Type: text/markdown
 Provides-Extra: test
 Provides-Extra: benchmarks
 License-File: LICENSE
 
-# lazycsv - an OOM csv parser
+# lazycsv - a memory-efficient csv parser
 
 ###### Developers: Michael Green, Chris Perkins
 
 lazycsv is a C implementation of a csv parser for python. The aim of this
 parser is to provide for fast extraction of sequences of data from a CSV file
 in a memory-efficient manner, with zero dependencies.
 
@@ -32,17 +32,17 @@
 
 The parser works as follows:
 
 First, The user file is memory-mapped internally to the LazyCSV object. That
 file is used to generate three indexes. The first is an index of values which
 correspond to the position in the user file where a given CSV field starts.
 This value is always a `uint16_t` which we found to be the optimal bit size for
-disk usage and execution performance. (This type can however be changed by
+disk usage and execution performance (This type can however be changed by
 setting the `LAZYCSV_INDEX_DTYPE` environment variable to any unsigned integer
-type) For index values outside the range of an unsigned short, An "anchor
+type). For index values outside the range of an unsigned short, An "anchor
 point" is created, which is a pair of `size_t` values that mark both the value
 which is subtracted from the index value such that the index value fits within
 16 bits, and the first column of the CSV where the anchor value applies. This
 anchor point is periodically written to the second index file when required for
 a given comma index. Finally, the third index writes the index of the first
 anchor point for each row of the file.
```

### Comparing `lazycsv-1.0.2/tests/test_lazycsv.py` & `lazycsv-1.0.3/tests/test_lazycsv.py`

 * *Files 3% similar despite different names*

```diff
@@ -146,14 +146,42 @@
         with prepped_file(actual) as tempf:
             lazy = lazycsv.LazyCSV(tempf.name, skip_headers=True)
             actual = list(list(lazy.sequence(col=i)) for i in range(lazy.cols))
         assert lazy.rows, lazy.cols == (3, 2)
         assert actual == [[b"", b"", b""], [b"", b"", b""]]
         assert lazy.headers == ()
 
+    def test_getitem(self, lazy):
+        data = b",,\n0x0,0x1,0x2\n1x0,1x1,1x2\n2x0,2x1,2x2\n"
+        with prepped_file(data) as tempf:
+            lazy = lazycsv.LazyCSV(tempf.name)
+            assert lazy[0, 0] == lazy[-3, -3] == b"0x0"
+            assert lazy[1, 1] == lazy[-2, -2] == b"1x1"
+            assert lazy[2, 2] == lazy[-1, -1] == b"2x2"
+            with pytest.raises(ValueError) as err:
+                lazy[3, 3]
+            assert ('provided value not in bounds of index',) == err.value.args
+
+    def test_getitem_empty(self, lazy):
+        data = b",,\n0x0,0x1,0x2\n1x0,,1x2\n2x0,2x1,2x2\n"
+        with prepped_file(data) as tempf:
+            lazy = lazycsv.LazyCSV(tempf.name)
+            assert lazy[1, 1] == b""
+
+    def test_getitem_skipped_headers(self):
+        data = b"0x0,0x1,0x2\n1x0,1x1,1x2\n2x0,2x1,2x2\n"
+        with prepped_file(data) as tempf:
+            lazy = lazycsv.LazyCSV(tempf.name, skip_headers=True)
+            assert lazy[0, 0] == lazy[-3, -3] == b"0x0"
+            assert lazy[1, 1] == lazy[-2, -2] == b"1x1"
+            assert lazy[2, 2] == lazy[-1, -1] == b"2x2"
+            with pytest.raises(ValueError) as err:
+                lazy[3, 3]
+            assert ('provided value not in bounds of index',) == err.value.args
+
 
 class TestLazyCSVIter:
     def test_to_list(self, lazy):
         _iter = lazy.sequence(col=0)
         assert _iter.to_list() == [b"0", b"1"]
 
     def test_to_numpy(self):
```

