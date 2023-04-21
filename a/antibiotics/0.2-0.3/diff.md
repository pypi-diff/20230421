# Comparing `tmp/antibiotics-0.2.tar.gz` & `tmp/antibiotics-0.3.tar.gz`

## filetype from file(1)

```diff
@@ -1 +1 @@
-gzip compressed data, was "dist\antibiotics-0.2.tar", last modified: Tue Aug 18 16:26:48 2020, max compression
+gzip compressed data, was "antibiotics-0.3.tar", last modified: Fri Apr 21 03:37:09 2023, max compression
```

## Comparing `antibiotics-0.2.tar` & `antibiotics-0.3.tar`

### file list

```diff
@@ -1,14 +1,15 @@
-drwxrwxrwx   0        0        0        0 2020-08-18 16:26:48.889788 antibiotics-0.2/
--rw-rw-rw-   0        0        0     4245 2020-08-18 16:26:48.889788 antibiotics-0.2/PKG-INFO
--rw-rw-rw-   0        0        0     2841 2020-08-18 15:54:25.000000 antibiotics-0.2/README.md
-drwxrwxrwx   0        0        0        0 2020-08-18 16:26:48.881774 antibiotics-0.2/antibiotics/
--rw-rw-rw-   0        0        0    11360 2020-08-18 16:16:27.000000 antibiotics-0.2/antibiotics/__init__.py
--rw-rw-rw-   0        0        0        0 2020-08-18 15:41:22.000000 antibiotics-0.2/antibiotics/py.typed
-drwxrwxrwx   0        0        0        0 2020-08-18 16:26:48.889788 antibiotics-0.2/antibiotics.egg-info/
--rw-rw-rw-   0        0        0     4245 2020-08-18 16:26:48.000000 antibiotics-0.2/antibiotics.egg-info/PKG-INFO
--rw-rw-rw-   0        0        0      237 2020-08-18 16:26:48.000000 antibiotics-0.2/antibiotics.egg-info/SOURCES.txt
--rw-rw-rw-   0        0        0        1 2020-08-18 16:26:48.000000 antibiotics-0.2/antibiotics.egg-info/dependency_links.txt
--rw-rw-rw-   0        0        0        2 2020-08-18 15:46:17.000000 antibiotics-0.2/antibiotics.egg-info/not-zip-safe
--rw-rw-rw-   0        0        0       12 2020-08-18 16:26:48.000000 antibiotics-0.2/antibiotics.egg-info/top_level.txt
--rw-rw-rw-   0        0        0       42 2020-08-18 16:26:48.889788 antibiotics-0.2/setup.cfg
--rw-rw-rw-   0        0        0      831 2020-08-18 16:26:00.000000 antibiotics-0.2/setup.py
+drwxrwxrwx   0        0        0        0 2023-04-21 03:37:09.230186 antibiotics-0.3/
+-rw-rw-rw-   0        0        0    11357 2020-08-18 15:48:29.000000 antibiotics-0.3/LICENSE
+-rw-rw-rw-   0        0        0     4706 2023-04-21 03:37:09.230186 antibiotics-0.3/PKG-INFO
+-rw-rw-rw-   0        0        0     3961 2023-04-21 03:37:06.000000 antibiotics-0.3/README.md
+drwxrwxrwx   0        0        0        0 2023-04-21 03:37:09.230186 antibiotics-0.3/antibiotics/
+-rw-rw-rw-   0        0        0    12192 2023-04-21 03:27:11.000000 antibiotics-0.3/antibiotics/__init__.py
+-rw-rw-rw-   0        0        0        0 2020-08-18 15:41:22.000000 antibiotics-0.3/antibiotics/py.typed
+drwxrwxrwx   0        0        0        0 2023-04-21 03:37:09.230186 antibiotics-0.3/antibiotics.egg-info/
+-rw-rw-rw-   0        0        0     4706 2023-04-21 03:37:09.000000 antibiotics-0.3/antibiotics.egg-info/PKG-INFO
+-rw-rw-rw-   0        0        0      245 2023-04-21 03:37:09.000000 antibiotics-0.3/antibiotics.egg-info/SOURCES.txt
+-rw-rw-rw-   0        0        0        1 2023-04-21 03:37:09.000000 antibiotics-0.3/antibiotics.egg-info/dependency_links.txt
+-rw-rw-rw-   0        0        0        2 2020-08-18 15:46:17.000000 antibiotics-0.3/antibiotics.egg-info/not-zip-safe
+-rw-rw-rw-   0        0        0       12 2023-04-21 03:37:09.000000 antibiotics-0.3/antibiotics.egg-info/top_level.txt
+-rw-rw-rw-   0        0        0       42 2023-04-21 03:37:09.230186 antibiotics-0.3/setup.cfg
+-rw-rw-rw-   0        0        0      848 2023-04-21 03:27:11.000000 antibiotics-0.3/setup.py
```

### Comparing `antibiotics-0.2/PKG-INFO` & `antibiotics-0.3/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,155 @@
 Metadata-Version: 2.1
 Name: antibiotics
-Version: 0.2
+Version: 0.3
 Summary: a treatment for PANDAS
 Home-page: https://github.com/derrickturk/antibiotics
 Author: Derrick W. Turk
 Author-email: dwt@terminusdatascience.com
 License: UNKNOWN
-Description: # antibiotics
-        ### NamedTuple / dataclasses <-> delimited text
-        
-        > "The best treatment for acute episodes of PANDAS is to treat the strep
-        infection causing the symptoms, if it is still present, with antibiotics."  
-        -- [National Institute of Mental Health](https://www.nimh.nih.gov/health/publications/pandas/index.shtml)
-        
-        `antibiotics` is a minimalist type-driven serialization/deserialization library
-        inspired by [Serde](https://serde.rs/) and
-        [cassava](http://hackage.haskell.org/package/cassava).
-        
-        It uses type annotations to automatically read and write `NamedTuple` or
-        `@dataclass` objects to or from delimited text files.
-        
-        Out of the box, it only knows about Python scalar types and `typing.Union`s
-        of them (including `typing.Optional`), but an extension mechanism for
-        arbitrary type-directed serialization and deserialization is provided
-        through the `type_serde_ext` argument to the `Delimited` constructor - see
-        `examples/advanced.py`.
-        
-        For `Union` types, serialization is driven by the runtime type,
-        and deserialization is attempted in the order of declaration of the
-        `Union` arguments - except that `NoneType` is tried first if present,
-        to preserve the expected behavior when deserializing null/missing values
-        of types whose deserializers do not throw when receiving `''` as an argument.
-        
-        ### Basic example
-        ```python
-        from antibiotics import Delimited
-        from dataclasses import dataclass
-        from typing import NamedTuple, Optional
-        
-        @dataclass
-        class SampleDC():
-            w: Optional[float]
-            x: int
-            y: bool
-            z: str
-        
-        class SampleNT(NamedTuple):
-            w: Optional[float]
-            x: int
-            y: bool
-            z: str
-        
-        if __name__ == '__main__':
-            dcs = list()
-            nts = list()
-            for i in range(10):
-                even = i % 2 == 0
-                dcs.append(SampleDC(
-                    i * 3.5 if even else None,
-                    i,
-                    not even,
-                    f'_",\t_{i}'
-                ))
-                nts.append(SampleNT(
-                    i * 3.5 if even else None,
-                    i,
-                    not even,
-                    f'_",\t_{i}'
-                ))
-        
-            csv = Delimited()
-            with open('dcs.csv', 'w') as f:
-                csv.write(SampleDC, dcs, f)
-        
-            tsv = Delimited(sep='\t', escape='\\')
-            with open('nts.tsv', 'w') as f:
-                tsv.write(SampleNT, dcs, f, header=False)
-        
-            with open('dcs.csv', 'r') as f:
-                for r in csv.read(SampleDC, f):
-                    print(r)
-        
-            with open('nts.tsv', 'r') as f:
-                for r in tsv.read(SampleNT, f, header=False):
-                    print(r)
-        ```
-        
-        View the full [pdoc3-generated API documentation](https://ghcdn.rawgit.org/derrickturk/antibiotics/master/doc/antibiotics/index.html).
-        
-        Install with:
-        
-            pip install --index-url https://test.pypi.org/simple/ antibiotics
-        
-        Or download directly [from Test PyPI](https://test.pypi.org/project/antibiotics/0.1/).
-        
-        #### (c) 2020 dwt | terminus data science, LLC
-        #### available under the Apache License 2.0
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# antibiotics
+### NamedTuple / dataclasses <-> delimited text
+
+> "The best treatment for acute episodes of PANDAS is to treat the strep
+infection causing the symptoms, if it is still present, with antibiotics."  
+-- [National Institute of Mental Health](https://www.nimh.nih.gov/health/publications/pandas/index.shtml)
+
+`antibiotics` is a minimalist type-driven serialization/deserialization library
+inspired by [Serde](https://serde.rs/) and
+[cassava](http://hackage.haskell.org/package/cassava).
+
+It uses type annotations to automatically read and write `NamedTuple` or
+`@dataclass` objects to or from delimited text files.
+
+Out of the box, it only knows about Python scalar types and `typing.Union`s
+of them (including `typing.Optional`), but an extension mechanism for
+arbitrary type-directed serialization and deserialization is provided
+through the `type_serde_ext` argument to the `Delimited` constructor - see
+`examples/advanced.py`.
+
+For `Union` types, serialization is driven by the runtime type,
+and deserialization is attempted in the order of declaration of the
+`Union` arguments - except that `NoneType` is tried first if present,
+to preserve the expected behavior when deserializing null/missing values
+of types whose deserializers do not throw when receiving `''` as an argument.
+
+A type `ExternalName` is also provided which may be used with `typing.Annotated`
+to specify the name which should be used for a member when serializing or
+deserializing (e.g. to match CSV headers).
+
+### Basic example
+```python
+from antibiotics import Delimited
+from dataclasses import dataclass
+from typing import NamedTuple, Optional
+
+@dataclass
+class SampleDC():
+    w: Optional[float]
+    x: int
+    y: bool
+    z: str
+
+class SampleNT(NamedTuple):
+    w: Optional[float]
+    x: int
+    y: bool
+    z: str
+
+if __name__ == '__main__':
+    dcs = list()
+    nts = list()
+    for i in range(10):
+        even = i % 2 == 0
+        dcs.append(SampleDC(
+            i * 3.5 if even else None,
+            i,
+            not even,
+            f'_",\t_{i}'
+        ))
+        nts.append(SampleNT(
+            i * 3.5 if even else None,
+            i,
+            not even,
+            f'_",\t_{i}'
+        ))
+
+    csv = Delimited()
+    with open('dcs.csv', 'w') as f:
+        csv.write(SampleDC, dcs, f)
+
+    tsv = Delimited(sep='\t', escape='\\')
+    with open('nts.tsv', 'w') as f:
+        tsv.write(SampleNT, dcs, f, header=False)
+
+    with open('dcs.csv', 'r') as f:
+        for r in csv.read(SampleDC, f):
+            print(r)
+
+    with open('nts.tsv', 'r') as f:
+        for r in tsv.read(SampleNT, f, header=False):
+            print(r)
+```
+
+### Example with custom external names
+```python
+from antibiotics import Delimited, ExternalName
+from dataclasses import dataclass
+from typing import Annotated, Optional
+
+@dataclass
+class SampleDC():
+    w: Annotated[Optional[float], ExternalName('BigW')]
+    x: Annotated[int, ExternalName('Fancy X')]
+    y: bool
+    z: str
+
+if __name__ == '__main__':
+    dcs = list()
+    for i in range(10):
+        even = i % 2 == 0
+        dcs.append(SampleDC(
+            i * 3.5 if even else None,
+            i,
+            not even,
+            f'_",\t_{i}'
+        ))
+
+    csv = Delimited()
+    with open('dcs.csv', 'w') as f:
+        csv.write(SampleDC, dcs, f)
+
+    with open('dcs.csv', 'r') as f:
+        for dc in csv.read(SampleDC, f):
+            print(dc)
+```
+
+### Documentation
+
+Documentation strings and type annotations are provided for public types and
+functions. We recommend viewing "nice" documentation pages using
+[`pdoc`](https://pdoc.dev/docs/pdoc.html); e.g. in the same environment as the
+`antibiotics` package is installed, install `pdoc` with `pip install pdoc`,
+then run `pdoc antibiotics`.
+
+---
+
+Install with:
+
+    pip install antibiotics
+
+Or download directly [from PyPI](https://pypi.org/project/antibiotics/).
+
+#### (c) 2023 dwt | terminus data science, LLC
+#### available under the Apache License 2.0
+
+
```

### Comparing `antibiotics-0.2/README.md` & `antibiotics-0.3/README.md`

 * *Files 21% similar despite different names*

```diff
@@ -20,14 +20,18 @@
 
 For `Union` types, serialization is driven by the runtime type,
 and deserialization is attempted in the order of declaration of the
 `Union` arguments - except that `NoneType` is tried first if present,
 to preserve the expected behavior when deserializing null/missing values
 of types whose deserializers do not throw when receiving `''` as an argument.
 
+A type `ExternalName` is also provided which may be used with `typing.Annotated`
+to specify the name which should be used for a member when serializing or
+deserializing (e.g. to match CSV headers).
+
 ### Basic example
 ```python
 from antibiotics import Delimited
 from dataclasses import dataclass
 from typing import NamedTuple, Optional
 
 @dataclass
@@ -74,17 +78,58 @@
             print(r)
 
     with open('nts.tsv', 'r') as f:
         for r in tsv.read(SampleNT, f, header=False):
             print(r)
 ```
 
-View the full [pdoc3-generated API documentation](https://ghcdn.rawgit.org/derrickturk/antibiotics/master/doc/antibiotics/index.html).
+### Example with custom external names
+```python
+from antibiotics import Delimited, ExternalName
+from dataclasses import dataclass
+from typing import Annotated, Optional
+
+@dataclass
+class SampleDC():
+    w: Annotated[Optional[float], ExternalName('BigW')]
+    x: Annotated[int, ExternalName('Fancy X')]
+    y: bool
+    z: str
+
+if __name__ == '__main__':
+    dcs = list()
+    for i in range(10):
+        even = i % 2 == 0
+        dcs.append(SampleDC(
+            i * 3.5 if even else None,
+            i,
+            not even,
+            f'_",\t_{i}'
+        ))
+
+    csv = Delimited()
+    with open('dcs.csv', 'w') as f:
+        csv.write(SampleDC, dcs, f)
+
+    with open('dcs.csv', 'r') as f:
+        for dc in csv.read(SampleDC, f):
+            print(dc)
+```
+
+### Documentation
+
+Documentation strings and type annotations are provided for public types and
+functions. We recommend viewing "nice" documentation pages using
+[`pdoc`](https://pdoc.dev/docs/pdoc.html); e.g. in the same environment as the
+`antibiotics` package is installed, install `pdoc` with `pip install pdoc`,
+then run `pdoc antibiotics`.
+
+---
 
 Install with:
 
-    pip install --index-url https://test.pypi.org/simple/ antibiotics
+    pip install antibiotics
 
-Or download directly [from Test PyPI](https://test.pypi.org/project/antibiotics/0.1/).
+Or download directly [from PyPI](https://pypi.org/project/antibiotics/).
 
-#### (c) 2020 dwt | terminus data science, LLC
+#### (c) 2023 dwt | terminus data science, LLC
 #### available under the Apache License 2.0
```

### Comparing `antibiotics-0.2/antibiotics/__init__.py` & `antibiotics-0.3/antibiotics/__init__.py`

 * *Files 14% similar despite different names*

```diff
@@ -8,25 +8,45 @@
 
 #  Unless required by applicable law or agreed to in writing, software
 #  distributed under the License is distributed on an "AS IS" BASIS,
 #  WITHOUT WARRANTIES OR CONDITIONS OF ANY KIND, either express or implied.
 #  See the License for the specific language governing permissions and
 #  limitations under the License.
 
-from typing import cast, Any, Callable, Dict, Iterable, List, Optional, TextIO
-from typing import Tuple, Type, TypeVar, Union
+import typing
+from typing import cast, Annotated, Any, Callable, Dict, Iterable, List
+from typing import NamedTuple, Optional, TextIO, Tuple, Type, TypeVar, Union
 
 import dataclasses as dc
 
 _T = TypeVar('_T')
 
 TypeSerDeMap = Dict[
     Type[Any],
     Tuple[Callable[[Any], str], Callable[[str], Any]]
 ]
+'''A serialization/deserialization function map by type.'''
+
+class ExternalName(NamedTuple):
+    '''Use with `typing.Annotated` to specify an external name for a member.
+
+    For example, given:
+
+    ```
+    class Example(NamedTuple):
+        x: Annotated[int, ExternalName('Fancy_X')]
+    ```
+
+    Objects of class `Example` will be read and written assuming the name
+    "Fancy_X" appears in delimited-file headers for the column corresponding
+    to the `x` data member.
+    '''
+
+    name: str
+    '''The external name.'''
 
 def _id(x: _T) -> _T:
     return x
 
 def _bool_from_str(s: str) -> bool:
     if s == 'False':
         return False
@@ -265,42 +285,44 @@
                             f'Unsupported type in deserialization: "{e}" as {ty}.'
                     ) from ex
                 except Exception as ex:
                     raise ValueError('Unable to parse "{e}" as {ty}.') from ex
         return cls(*vals)
 
 def _field_names(cls: Type[Any]) -> List[str]:
-    try:
-        return list(cls._fields)
-    except:
-        pass
-    try:
-        return [f.name for f in dc.fields(cls)]
-    except:
-        pass
-    raise ValueError("This type is not a NamedTuple or @dataclass.")
+    annots = typing.get_type_hints(cls, include_extras=True)
+    names = []
+    for name, annot in annots.items():
+        if typing.get_origin(annot) is Annotated:
+            ext_names = [
+              n.name for n in typing.get_args(annot)
+              if isinstance(n, ExternalName)
+            ]
+
+            if len(ext_names) == 0:
+                names.append(name)
+            elif len(ext_names) > 1:
+                raise TypeError(
+                  f'Too many ExternalName annotations for field {name}.')
+            else:
+                names.append(ext_names[0])
+        else:
+            names.append(name)
+    return names
 
 def _field_types(cls: Type[Any]) -> List[Type[Any]]:
-    try:
-        return [ty for _, ty in cls._field_types.items()]
-    except:
-        pass
-    try:
-        return [f.type for f in dc.fields(cls)]
-    except:
-        pass
-    raise ValueError("This type is not a NamedTuple or @dataclass.")
+    return list(typing.get_type_hints(cls).values())
 
 def _field_vals(cls: Type[_T], rec: _T) -> List[Any]:
     try:
         return list(rec) # type: ignore
     except:
         pass
     try:
-        return list(dc.astuple(rec))
+        return list(dc.astuple(rec)) # type: ignore
     except:
         pass
     raise ValueError("This type is not a NamedTuple or @dataclass.")
 
 def _union_types(ty: Type[Any]) -> Optional[List[Type[Any]]]:
     # see: https://stackoverflow.com/questions/49171189/whats-the-correct-way-to-check-if-an-object-is-a-typing-generic
     try:
@@ -314,9 +336,10 @@
                     [a for a in ty.__args__ if a != type(None)])
         return None
     except:
         return None
 
 __all__ = [
     'TypeSerDeMap',
+    'ExternalName',
     'Delimited',
 ]
```

### Comparing `antibiotics-0.2/antibiotics.egg-info/PKG-INFO` & `antibiotics-0.3/antibiotics.egg-info/PKG-INFO`

 * *Files 14% similar despite different names*

```diff
@@ -1,107 +1,155 @@
 Metadata-Version: 2.1
 Name: antibiotics
-Version: 0.2
+Version: 0.3
 Summary: a treatment for PANDAS
 Home-page: https://github.com/derrickturk/antibiotics
 Author: Derrick W. Turk
 Author-email: dwt@terminusdatascience.com
 License: UNKNOWN
-Description: # antibiotics
-        ### NamedTuple / dataclasses <-> delimited text
-        
-        > "The best treatment for acute episodes of PANDAS is to treat the strep
-        infection causing the symptoms, if it is still present, with antibiotics."  
-        -- [National Institute of Mental Health](https://www.nimh.nih.gov/health/publications/pandas/index.shtml)
-        
-        `antibiotics` is a minimalist type-driven serialization/deserialization library
-        inspired by [Serde](https://serde.rs/) and
-        [cassava](http://hackage.haskell.org/package/cassava).
-        
-        It uses type annotations to automatically read and write `NamedTuple` or
-        `@dataclass` objects to or from delimited text files.
-        
-        Out of the box, it only knows about Python scalar types and `typing.Union`s
-        of them (including `typing.Optional`), but an extension mechanism for
-        arbitrary type-directed serialization and deserialization is provided
-        through the `type_serde_ext` argument to the `Delimited` constructor - see
-        `examples/advanced.py`.
-        
-        For `Union` types, serialization is driven by the runtime type,
-        and deserialization is attempted in the order of declaration of the
-        `Union` arguments - except that `NoneType` is tried first if present,
-        to preserve the expected behavior when deserializing null/missing values
-        of types whose deserializers do not throw when receiving `''` as an argument.
-        
-        ### Basic example
-        ```python
-        from antibiotics import Delimited
-        from dataclasses import dataclass
-        from typing import NamedTuple, Optional
-        
-        @dataclass
-        class SampleDC():
-            w: Optional[float]
-            x: int
-            y: bool
-            z: str
-        
-        class SampleNT(NamedTuple):
-            w: Optional[float]
-            x: int
-            y: bool
-            z: str
-        
-        if __name__ == '__main__':
-            dcs = list()
-            nts = list()
-            for i in range(10):
-                even = i % 2 == 0
-                dcs.append(SampleDC(
-                    i * 3.5 if even else None,
-                    i,
-                    not even,
-                    f'_",\t_{i}'
-                ))
-                nts.append(SampleNT(
-                    i * 3.5 if even else None,
-                    i,
-                    not even,
-                    f'_",\t_{i}'
-                ))
-        
-            csv = Delimited()
-            with open('dcs.csv', 'w') as f:
-                csv.write(SampleDC, dcs, f)
-        
-            tsv = Delimited(sep='\t', escape='\\')
-            with open('nts.tsv', 'w') as f:
-                tsv.write(SampleNT, dcs, f, header=False)
-        
-            with open('dcs.csv', 'r') as f:
-                for r in csv.read(SampleDC, f):
-                    print(r)
-        
-            with open('nts.tsv', 'r') as f:
-                for r in tsv.read(SampleNT, f, header=False):
-                    print(r)
-        ```
-        
-        View the full [pdoc3-generated API documentation](https://ghcdn.rawgit.org/derrickturk/antibiotics/master/doc/antibiotics/index.html).
-        
-        Install with:
-        
-            pip install --index-url https://test.pypi.org/simple/ antibiotics
-        
-        Or download directly [from Test PyPI](https://test.pypi.org/project/antibiotics/0.1/).
-        
-        #### (c) 2020 dwt | terminus data science, LLC
-        #### available under the Apache License 2.0
-        
 Platform: UNKNOWN
 Classifier: License :: OSI Approved :: Apache Software License
-Classifier: Programming Language :: Python :: 3.6
-Classifier: Programming Language :: Python :: 3.7
-Classifier: Programming Language :: Python :: 3.8
+Classifier: Programming Language :: Python :: 3.9
+Classifier: Programming Language :: Python :: 3.10
+Classifier: Programming Language :: Python :: 3.11
 Classifier: Operating System :: OS Independent
-Requires-Python: >=3.7
+Requires-Python: >=3.9
 Description-Content-Type: text/markdown
+License-File: LICENSE
+
+# antibiotics
+### NamedTuple / dataclasses <-> delimited text
+
+> "The best treatment for acute episodes of PANDAS is to treat the strep
+infection causing the symptoms, if it is still present, with antibiotics."  
+-- [National Institute of Mental Health](https://www.nimh.nih.gov/health/publications/pandas/index.shtml)
+
+`antibiotics` is a minimalist type-driven serialization/deserialization library
+inspired by [Serde](https://serde.rs/) and
+[cassava](http://hackage.haskell.org/package/cassava).
+
+It uses type annotations to automatically read and write `NamedTuple` or
+`@dataclass` objects to or from delimited text files.
+
+Out of the box, it only knows about Python scalar types and `typing.Union`s
+of them (including `typing.Optional`), but an extension mechanism for
+arbitrary type-directed serialization and deserialization is provided
+through the `type_serde_ext` argument to the `Delimited` constructor - see
+`examples/advanced.py`.
+
+For `Union` types, serialization is driven by the runtime type,
+and deserialization is attempted in the order of declaration of the
+`Union` arguments - except that `NoneType` is tried first if present,
+to preserve the expected behavior when deserializing null/missing values
+of types whose deserializers do not throw when receiving `''` as an argument.
+
+A type `ExternalName` is also provided which may be used with `typing.Annotated`
+to specify the name which should be used for a member when serializing or
+deserializing (e.g. to match CSV headers).
+
+### Basic example
+```python
+from antibiotics import Delimited
+from dataclasses import dataclass
+from typing import NamedTuple, Optional
+
+@dataclass
+class SampleDC():
+    w: Optional[float]
+    x: int
+    y: bool
+    z: str
+
+class SampleNT(NamedTuple):
+    w: Optional[float]
+    x: int
+    y: bool
+    z: str
+
+if __name__ == '__main__':
+    dcs = list()
+    nts = list()
+    for i in range(10):
+        even = i % 2 == 0
+        dcs.append(SampleDC(
+            i * 3.5 if even else None,
+            i,
+            not even,
+            f'_",\t_{i}'
+        ))
+        nts.append(SampleNT(
+            i * 3.5 if even else None,
+            i,
+            not even,
+            f'_",\t_{i}'
+        ))
+
+    csv = Delimited()
+    with open('dcs.csv', 'w') as f:
+        csv.write(SampleDC, dcs, f)
+
+    tsv = Delimited(sep='\t', escape='\\')
+    with open('nts.tsv', 'w') as f:
+        tsv.write(SampleNT, dcs, f, header=False)
+
+    with open('dcs.csv', 'r') as f:
+        for r in csv.read(SampleDC, f):
+            print(r)
+
+    with open('nts.tsv', 'r') as f:
+        for r in tsv.read(SampleNT, f, header=False):
+            print(r)
+```
+
+### Example with custom external names
+```python
+from antibiotics import Delimited, ExternalName
+from dataclasses import dataclass
+from typing import Annotated, Optional
+
+@dataclass
+class SampleDC():
+    w: Annotated[Optional[float], ExternalName('BigW')]
+    x: Annotated[int, ExternalName('Fancy X')]
+    y: bool
+    z: str
+
+if __name__ == '__main__':
+    dcs = list()
+    for i in range(10):
+        even = i % 2 == 0
+        dcs.append(SampleDC(
+            i * 3.5 if even else None,
+            i,
+            not even,
+            f'_",\t_{i}'
+        ))
+
+    csv = Delimited()
+    with open('dcs.csv', 'w') as f:
+        csv.write(SampleDC, dcs, f)
+
+    with open('dcs.csv', 'r') as f:
+        for dc in csv.read(SampleDC, f):
+            print(dc)
+```
+
+### Documentation
+
+Documentation strings and type annotations are provided for public types and
+functions. We recommend viewing "nice" documentation pages using
+[`pdoc`](https://pdoc.dev/docs/pdoc.html); e.g. in the same environment as the
+`antibiotics` package is installed, install `pdoc` with `pip install pdoc`,
+then run `pdoc antibiotics`.
+
+---
+
+Install with:
+
+    pip install antibiotics
+
+Or download directly [from PyPI](https://pypi.org/project/antibiotics/).
+
+#### (c) 2023 dwt | terminus data science, LLC
+#### available under the Apache License 2.0
+
+
```

### Comparing `antibiotics-0.2/setup.py` & `antibiotics-0.3/setup.py`

 * *Files 15% similar despite different names*

```diff
@@ -1,26 +1,26 @@
-import setuptools
+import setuptools # type: ignore
 
 with open('README.md', 'r') as f:
     long_description = f.read()
 
 setuptools.setup(
     name='antibiotics',
     description='a treatment for PANDAS',
     long_description=long_description,
     long_description_content_type='text/markdown',
     author='Derrick W. Turk',
     author_email='dwt@terminusdatascience.com',
     url='https://github.com/derrickturk/antibiotics',
-    version='0.2',
+    version='0.3',
     packages=setuptools.find_packages(),
     classifiers=[
         'License :: OSI Approved :: Apache Software License',
-        'Programming Language :: Python :: 3.6',
-        'Programming Language :: Python :: 3.7',
-        'Programming Language :: Python :: 3.8',
+        'Programming Language :: Python :: 3.9',
+        'Programming Language :: Python :: 3.10',
+        'Programming Language :: Python :: 3.11',
         'Operating System :: OS Independent',
     ],
-    python_requires='>=3.7',
+    python_requires='>=3.9',
     package_data={'antibiotics': ['py.typed']},
     zip_safe=False,
 )
```

