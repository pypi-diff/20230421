# Comparing `tmp/antibiotics-0.3.tar.gz` & `tmp/antibiotics-0.4.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "antibiotics-0.3.tar", last modified: Fri Apr 21 03:37:09 2023, max compression
+gzip compressed data, was "antibiotics-0.4.tar", last modified: Fri Apr 21 05:19:59 2023, max compression
```

## Comparing `antibiotics-0.3.tar` & `antibiotics-0.4.tar`

### file list

```diff
@@ -1,15 +1,15 @@
-drwxrwxrwx   0        0        0        0 2023-04-21 03:37:09.230186 antibiotics-0.3/
--rw-rw-rw-   0        0        0    11357 2020-08-18 15:48:29.000000 antibiotics-0.3/LICENSE
--rw-rw-rw-   0        0        0     4706 2023-04-21 03:37:09.230186 antibiotics-0.3/PKG-INFO
--rw-rw-rw-   0        0        0     3961 2023-04-21 03:37:06.000000 antibiotics-0.3/README.md
-drwxrwxrwx   0        0        0        0 2023-04-21 03:37:09.230186 antibiotics-0.3/antibiotics/
--rw-rw-rw-   0        0        0    12192 2023-04-21 03:27:11.000000 antibiotics-0.3/antibiotics/__init__.py
--rw-rw-rw-   0        0        0        0 2020-08-18 15:41:22.000000 antibiotics-0.3/antibiotics/py.typed
-drwxrwxrwx   0        0        0        0 2023-04-21 03:37:09.230186 antibiotics-0.3/antibiotics.egg-info/
--rw-rw-rw-   0        0        0     4706 2023-04-21 03:37:09.000000 antibiotics-0.3/antibiotics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      245 2023-04-21 03:37:09.000000 antibiotics-0.3/antibiotics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2023-04-21 03:37:09.000000 antibiotics-0.3/antibiotics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-08-18 15:46:17.000000 antibiotics-0.3/antibiotics.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2023-04-21 03:37:09.000000 antibiotics-0.3/antibiotics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2023-04-21 03:37:09.230186 antibiotics-0.3/setup.cfg
--rw-rw-rw-   0        0        0      848 2023-04-21 03:27:11.000000 antibiotics-0.3/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 05:19:59.924325 antibiotics-0.4/
+-rw-rw-rw-   0        0        0    11357 2020-08-18 15:48:29.000000 antibiotics-0.4/LICENSE
+-rw-rw-rw-   0        0        0     4834 2023-04-21 05:19:59.924325 antibiotics-0.4/PKG-INFO
+-rw-rw-rw-   0        0        0     4177 2023-04-21 05:17:03.000000 antibiotics-0.4/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 05:19:59.914262 antibiotics-0.4/antibiotics/
+-rw-rw-rw-   0        0        0    13962 2023-04-21 05:12:49.000000 antibiotics-0.4/antibiotics/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-08-18 15:41:22.000000 antibiotics-0.4/antibiotics/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-21 05:19:59.924325 antibiotics-0.4/antibiotics.egg-info/
+-rw-rw-rw-   0        0        0     4834 2023-04-21 05:19:59.000000 antibiotics-0.4/antibiotics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-04-21 05:19:59.000000 antibiotics-0.4/antibiotics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 05:19:59.000000 antibiotics-0.4/antibiotics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-08-18 15:46:17.000000 antibiotics-0.4/antibiotics.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-04-21 05:19:59.000000 antibiotics-0.4/antibiotics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 05:19:59.924325 antibiotics-0.4/setup.cfg
+-rw-rw-rw-   0        0        0      800 2023-04-21 05:19:27.000000 antibiotics-0.4/setup.py
```

### Comparing `antibiotics-0.3/LICENSE` & `antibiotics-0.4/LICENSE`

 * *Files identical despite different names*

### Comparing `antibiotics-0.3/PKG-INFO` & `antibiotics-0.4/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: antibiotics
-Version: 0.3
+Version: 0.4
 Summary: a treatment for PANDAS
 Home-page: https://github.com/derrickturk/antibiotics
 Author: Derrick W. Turk
 Author-email: dwt@terminusdatascience.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # antibiotics
 ### NamedTuple / dataclasses <-> delimited text
 
 > "The best treatment for acute episodes of PANDAS is to treat the strep
@@ -42,14 +39,17 @@
 to preserve the expected behavior when deserializing null/missing values
 of types whose deserializers do not throw when receiving `''` as an argument.
 
 A type `ExternalName` is also provided which may be used with `typing.Annotated`
 to specify the name which should be used for a member when serializing or
 deserializing (e.g. to match CSV headers).
 
+Please note that as with the built-in `csv` module, file-like objects used
+with this library should be opened with `newline=''`.
+
 ### Basic example
 ```python
 from antibiotics import Delimited
 from dataclasses import dataclass
 from typing import NamedTuple, Optional
 
 @dataclass
@@ -80,26 +80,26 @@
             i * 3.5 if even else None,
             i,
             not even,
             f'_",\t_{i}'
         ))
 
     csv = Delimited()
-    with open('dcs.csv', 'w') as f:
+    with open('dcs.csv', 'w', newline='') as f:
         csv.write(SampleDC, dcs, f)
 
-    tsv = Delimited(sep='\t', escape='\\')
-    with open('nts.tsv', 'w') as f:
+    tsv = Delimited(sep='\t', escape='\\', newline='\n')
+    with open('nts.tsv', 'w', newline='') as f:
         tsv.write(SampleNT, dcs, f, header=False)
 
-    with open('dcs.csv', 'r') as f:
+    with open('dcs.csv', 'r', newline='') as f:
         for r in csv.read(SampleDC, f):
             print(r)
 
-    with open('nts.tsv', 'r') as f:
+    with open('nts.tsv', 'r', newline='') as f:
         for r in tsv.read(SampleNT, f, header=False):
             print(r)
 ```
 
 ### Example with custom external names
 ```python
 from antibiotics import Delimited, ExternalName
@@ -121,18 +121,18 @@
             i * 3.5 if even else None,
             i,
             not even,
             f'_",\t_{i}'
         ))
 
     csv = Delimited()
-    with open('dcs.csv', 'w') as f:
+    with open('dcs.csv', 'w', newline='') as f:
         csv.write(SampleDC, dcs, f)
 
-    with open('dcs.csv', 'r') as f:
+    with open('dcs.csv', 'r', newline='') as f:
         for dc in csv.read(SampleDC, f):
             print(dc)
 ```
 
 ### Documentation
 
 Documentation strings and type annotations are provided for public types and
@@ -147,9 +147,7 @@
 
     pip install antibiotics
 
 Or download directly [from PyPI](https://pypi.org/project/antibiotics/).
 
 #### (c) 2023 dwt | terminus data science, LLC
 #### available under the Apache License 2.0
-
-
```

### Comparing `antibiotics-0.3/README.md` & `antibiotics-0.4/README.md`

 * *Files 18% similar despite different names*

```diff
@@ -24,14 +24,17 @@
 to preserve the expected behavior when deserializing null/missing values
 of types whose deserializers do not throw when receiving `''` as an argument.
 
 A type `ExternalName` is also provided which may be used with `typing.Annotated`
 to specify the name which should be used for a member when serializing or
 deserializing (e.g. to match CSV headers).
 
+Please note that as with the built-in `csv` module, file-like objects used
+with this library should be opened with `newline=''`.
+
 ### Basic example
 ```python
 from antibiotics import Delimited
 from dataclasses import dataclass
 from typing import NamedTuple, Optional
 
 @dataclass
@@ -62,26 +65,26 @@
             i * 3.5 if even else None,
             i,
             not even,
             f'_",\t_{i}'
         ))
 
     csv = Delimited()
-    with open('dcs.csv', 'w') as f:
+    with open('dcs.csv', 'w', newline='') as f:
         csv.write(SampleDC, dcs, f)
 
-    tsv = Delimited(sep='\t', escape='\\')
-    with open('nts.tsv', 'w') as f:
+    tsv = Delimited(sep='\t', escape='\\', newline='\n')
+    with open('nts.tsv', 'w', newline='') as f:
         tsv.write(SampleNT, dcs, f, header=False)
 
-    with open('dcs.csv', 'r') as f:
+    with open('dcs.csv', 'r', newline='') as f:
         for r in csv.read(SampleDC, f):
             print(r)
 
-    with open('nts.tsv', 'r') as f:
+    with open('nts.tsv', 'r', newline='') as f:
         for r in tsv.read(SampleNT, f, header=False):
             print(r)
 ```
 
 ### Example with custom external names
 ```python
 from antibiotics import Delimited, ExternalName
@@ -103,18 +106,18 @@
             i * 3.5 if even else None,
             i,
             not even,
             f'_",\t_{i}'
         ))
 
     csv = Delimited()
-    with open('dcs.csv', 'w') as f:
+    with open('dcs.csv', 'w', newline='') as f:
         csv.write(SampleDC, dcs, f)
 
-    with open('dcs.csv', 'r') as f:
+    with open('dcs.csv', 'r', newline='') as f:
         for dc in csv.read(SampleDC, f):
             print(dc)
 ```
 
 ### Documentation
 
 Documentation strings and type annotations are provided for public types and
```

### Comparing `antibiotics-0.3/antibiotics/__init__.py` & `antibiotics-0.4/antibiotics/__init__.py`

 * *Files 5% similar despite different names*

```diff
@@ -8,17 +8,18 @@
 
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
+import types
 import typing
 from typing import cast, Annotated, Any, Callable, Dict, Iterable, List
-from typing import NamedTuple, Optional, TextIO, Tuple, Type, TypeVar, Union
+from typing import NamedTuple, Optional, TextIO, Tuple, Type, TypeVar
 
 import dataclasses as dc
 
 _T = TypeVar('_T')
 
 TypeSerDeMap = Dict[
     Type[Any],
@@ -66,22 +67,27 @@
     float: (str, float),
     complex: (str, complex),
     str: (_id, _id),
     bytes: (lambda b: cast(str, b.decode('utf8')), lambda s: s.encode('utf8')),
     type(None): (lambda _: '', _none_from_str),
 }
 
+_BUF_SIZE: int = 1024
+
 @dc.dataclass
 class Delimited():
     '''a reader and writer for delimited data
 
     parameters may be specified when initializing a Delimited object as either
     positional or named arguments; the `__init__` signature is more-or-less:
 
-        Delimited(sep=',', quote='"', escape='"', type_serde_ext=None)
+    ```
+    Delimited(sep=',', quote='"', escape='"', newline='\r\n',
+      type_serde_ext=None)
+    ```
 
     the default values are suitable for reading and writing "standard" CSV files
 
     the core concept behind antibiotics is the type-driven
       serialization/deserialization map
 
     this map is a dictionary from types `T` to tuples of a serialization
@@ -96,27 +102,35 @@
 
     antibiotics automatically handles serialization/deserialization for types
       which are unions of types with map entries - for example, `Optional[T]`
       will use either the `None` serializer/deserializer or the `T`
       serializer/deserializer, depending on the runtime value; deserializers
       for union types are tried in order of declaration until one runs without
       raising an exception
+
+    much like the `csv` module, files opened for use with `antibiotics` should
+      be opened with `newline=''`
     '''
 
     sep: str = ','
-    '''the separator between delimited entries [default ,]'''
+    '''the separator between delimited entries [default `','`]'''
 
     quote: Optional[str] = '"'
     '''the character, if any, used to introduce and close quoted entries (which
-      may include the delimiter verbatim) [default "]
+      may include the delimiter verbatim) [default `'"'`]
     '''
 
     escape: Optional[str] = '"'
     '''the character, if any, used to escape verbatim quote characters occurring
-      inside quoted entries [default "]
+      inside quoted entries [default `'"'`]
+    '''
+
+    newline: str = '\r\n'
+    '''the character used to terminate lines; may occur inside quoted entries
+      [default `'\r\n'`]
     '''
 
     type_serde_ext: dc.InitVar[Optional[TypeSerDeMap]] = None
     '''optionally, a dictionary containing additional entries for the
       type-driven serialization/deserialization map
     '''
 
@@ -136,37 +150,37 @@
             self.write_header(cls, stream)
         for r in recs:
             self.write_record(r, stream)
 
     def write_header(self, cls: Type[Any], stream: TextIO) -> None:
         '''write an appropriate header for a given record type to a stream'''
         stream.write(self._delimit(_field_names(cls)))
-        stream.write('\n')
+        stream.write(self.newline)
 
     def write_record(self, rec: _T, stream: TextIO) -> None:
         '''write a single typed record to a stream'''
         stream.write(self._delimit(self._render(rec)))
-        stream.write('\n')
+        stream.write(self.newline)
 
     def read_header(self, cls: Type[Any], stream: TextIO) -> None:
         '''read a header for a given record type from a stream, and check it
           against the expected field names, raising a `ValueError` on failure
         '''
-        hdr = self._split(stream.readline().rstrip('\n'))
+        hdr = self._line(stream)
         expected = _field_names(cls)
         if hdr != expected:
             raise ValueError(
                 f'Invalid header for provided type: expected {expected}, found {hdr}.')
 
     def read_record(self, cls: Type[_T], stream: TextIO) -> Optional[_T]:
         '''read a single typed record from a stream'''
-        line = stream.readline()
-        if line == '':
+        line = self._line(stream)
+        if line is None:
             return None
-        return self._parse(cls, self._split(line.rstrip('\n')))
+        return self._parse(cls, line)
 
     def read(self, cls: Type[_T], stream: TextIO,
             header: bool = True) -> Iterable[_T]:
         '''lazily read a sequence of typed records from a stream, with or
           without a header
         '''
         if header:
@@ -217,50 +231,81 @@
                     elems.append(self.type_serde[ty][0](v))
                 except KeyError as ex:
                     raise TypeError(
                         f'Unsupported type in serialization: {v} as {ty}.'
                     ) from ex
         return elems
 
-    def _split(self, line: str) -> List[str]:
+    def _line(self, stream: TextIO) -> Optional[List[str]]:
         elems = list()
-        this_elem = list()
+        this_elem: List[str] = list()
         in_quote = False
         in_escape = False
-        for c in line:
-            if in_escape:
-                this_elem.append(c)
-                in_escape = False
-                continue
-
-            if in_quote:
-                if c == self.escape:
-                    in_escape = True
+        nl_len = len(self.newline)
+        did_nl_seek = False
+
+        while True:
+            pos = stream.tell()
+            buf = stream.read(_BUF_SIZE)
+            n = len(buf)
+            if n == 0:
+                # missing final terminator
+                if this_elem:
+                    elems.append(''.join(this_elem))
+                    return elems
+                return None
+
+            for i in range(n):
+                if in_escape and self.escape == self.quote:
+                    if buf[i] == self.quote:
+                        in_escape = False
+                        this_elem.append(buf[i])
+                        continue
+                    else:
+                        # that "escape" was a closing quote!
+                        in_escape = False
+                        in_quote = False
+                elif in_escape:
+                    this_elem.append(buf[i])
+                    in_escape = False
                     continue
-                if c == self.quote:
-                    in_quote = False
+
+                if in_quote:
+                    if buf[i] == self.escape:
+                        in_escape = True
+                        continue
+                    if buf[i] == self.quote:
+                        in_quote = False
+                        continue
+                    this_elem.append(buf[i])
                     continue
-                this_elem.append(c)
-                continue
 
-            if c == self.sep:
-                elems.append(''.join(this_elem))
-                this_elem = list()
-            elif c == self.quote:
-                in_quote = True
-            else:
-                this_elem.append(c)
-        elems.append(''.join(this_elem))
-        return elems
+                if buf[i] == self.sep:
+                    elems.append(''.join(this_elem))
+                    this_elem = list()
+                elif buf[i] == self.quote:
+                    in_quote = True
+                # handle the case where we can't check for newline because it's
+                #   potentially split across reads by seeking to current
+                #   position and trying again...
+                elif i + nl_len > n and not did_nl_seek:
+                    stream.seek(pos + i, 0)
+                    did_nl_seek = True
+                    break # to continue the while
+                elif buf[i:i + nl_len] == self.newline:
+                    did_nl_seek = False
+                    elems.append(''.join(this_elem))
+                    stream.seek(pos + i + nl_len, 0)
+                    return elems
+                else:
+                    this_elem.append(buf[i])
 
     def _parse(self, cls: Type[_T], elems: List[str]) -> _T:
         tys = _field_types(cls)
         if len(elems) != len(tys):
-            print(elems)
-            print(tys)
             raise ValueError(
                 f'Record length {len(elems)} does not match required field count ({len(tys)}).')
         vals: List[Any] = list()
         for ty, e in zip(tys, elems):
             un_tys = _union_types(ty)
             if un_tys:
                 found = False
@@ -321,25 +366,25 @@
         return list(dc.astuple(rec)) # type: ignore
     except:
         pass
     raise ValueError("This type is not a NamedTuple or @dataclass.")
 
 def _union_types(ty: Type[Any]) -> Optional[List[Type[Any]]]:
     # see: https://stackoverflow.com/questions/49171189/whats-the-correct-way-to-check-if-an-object-is-a-typing-generic
-    try:
-        if ty.__origin__ == Union:
-            # move NoneType to front of list, so it gets tried
-            #   first in deserialization, ensuring "correct" behavior when
-            #   deserializing types Optional[T] where the deserializer for T
-            #   does not fail on a '' argument - that is, ensure we prioritize
-            #   deserializing None for empty strings when necessary.
-            return ([a for a in ty.__args__ if a == type(None)] +
-                    [a for a in ty.__args__ if a != type(None)])
-        return None
-    except:
+    origin = typing.get_origin(ty)
+    if origin in (typing.Union, types.UnionType):
+        args = typing.get_args(ty)
+        # move NoneType to front of list, so it gets tried
+        #   first in deserialization, ensuring "correct" behavior when
+        #   deserializing types Optional[T] where the deserializer for T
+        #   does not fail on a '' argument - that is, ensure we prioritize
+        #   deserializing None for empty strings when necessary.
+        return ([a for a in args if a is type(None)] +
+                [a for a in args if a is not type(None)])
+    else:
         return None
 
 __all__ = [
     'TypeSerDeMap',
     'ExternalName',
     'Delimited',
 ]
```

### Comparing `antibiotics-0.3/antibiotics.egg-info/PKG-INFO` & `antibiotics-0.4/antibiotics.egg-info/PKG-INFO`

 * *Files 10% similar despite different names*

```diff
@@ -1,22 +1,19 @@
 Metadata-Version: 2.1
 Name: antibiotics
-Version: 0.3
+Version: 0.4
 Summary: a treatment for PANDAS
 Home-page: https://github.com/derrickturk/antibiotics
 Author: Derrick W. Turk
 Author-email: dwt@terminusdatascience.com
-License: UNKNOWN
-Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.9
 Classifier: Programming Language :: Python :: 3.10
 Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.9
+Requires-Python: >=3.10
 Description-Content-Type: text/markdown
 License-File: LICENSE
 
 # antibiotics
 ### NamedTuple / dataclasses <-> delimited text
 
 > "The best treatment for acute episodes of PANDAS is to treat the strep
@@ -42,14 +39,17 @@
 to preserve the expected behavior when deserializing null/missing values
 of types whose deserializers do not throw when receiving `''` as an argument.
 
 A type `ExternalName` is also provided which may be used with `typing.Annotated`
 to specify the name which should be used for a member when serializing or
 deserializing (e.g. to match CSV headers).
 
+Please note that as with the built-in `csv` module, file-like objects used
+with this library should be opened with `newline=''`.
+
 ### Basic example
 ```python
 from antibiotics import Delimited
 from dataclasses import dataclass
 from typing import NamedTuple, Optional
 
 @dataclass
@@ -80,26 +80,26 @@
             i * 3.5 if even else None,
             i,
             not even,
             f'_",\t_{i}'
         ))
 
     csv = Delimited()
-    with open('dcs.csv', 'w') as f:
+    with open('dcs.csv', 'w', newline='') as f:
         csv.write(SampleDC, dcs, f)
 
-    tsv = Delimited(sep='\t', escape='\\')
-    with open('nts.tsv', 'w') as f:
+    tsv = Delimited(sep='\t', escape='\\', newline='\n')
+    with open('nts.tsv', 'w', newline='') as f:
         tsv.write(SampleNT, dcs, f, header=False)
 
-    with open('dcs.csv', 'r') as f:
+    with open('dcs.csv', 'r', newline='') as f:
         for r in csv.read(SampleDC, f):
             print(r)
 
-    with open('nts.tsv', 'r') as f:
+    with open('nts.tsv', 'r', newline='') as f:
         for r in tsv.read(SampleNT, f, header=False):
             print(r)
 ```
 
 ### Example with custom external names
 ```python
 from antibiotics import Delimited, ExternalName
@@ -121,18 +121,18 @@
             i * 3.5 if even else None,
             i,
             not even,
             f'_",\t_{i}'
         ))
 
     csv = Delimited()
-    with open('dcs.csv', 'w') as f:
+    with open('dcs.csv', 'w', newline='') as f:
         csv.write(SampleDC, dcs, f)
 
-    with open('dcs.csv', 'r') as f:
+    with open('dcs.csv', 'r', newline='') as f:
         for dc in csv.read(SampleDC, f):
             print(dc)
 ```
 
 ### Documentation
 
 Documentation strings and type annotations are provided for public types and
@@ -147,9 +147,7 @@
 
     pip install antibiotics
 
 Or download directly [from PyPI](https://pypi.org/project/antibiotics/).
 
 #### (c) 2023 dwt | terminus data science, LLC
 #### available under the Apache License 2.0
-
-
```

### Comparing `antibiotics-0.3/setup.py` & `antibiotics-0.4/setup.py`

 * *Files 9% similar despite different names*

```diff
@@ -7,20 +7,19 @@
     name='antibiotics',
     description='a treatment for PANDAS',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Derrick W. Turk',
     author_email='dwt@terminusdatascience.com',
     url='https://github.com/derrickturk/antibiotics',
-    version='0.3',
+    version='0.4',
     packages=setuptools.find_packages(),
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.9',
         'Programming Language :: Python :: 3.10',
         'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.9',
+    python_requires='>=3.10',
     package_data={'antibiotics': ['py.typed']},
     zip_safe=False,
 )
```

